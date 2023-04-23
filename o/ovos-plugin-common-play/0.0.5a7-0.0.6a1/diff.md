# Comparing `tmp/ovos_plugin_common_play-0.0.5a7.tar.gz` & `tmp/ovos_plugin_common_play-0.0.6a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos_plugin_common_play-0.0.5a7.tar", last modified: Thu Apr 20 00:32:57 2023, max compression
+gzip compressed data, was "ovos_plugin_common_play-0.0.6a1.tar", last modified: Sun Apr 23 00:23:04 2023, max compression
```

## Comparing `ovos_plugin_common_play-0.0.5a7.tar` & `ovos_plugin_common_play-0.0.6a1.tar`

### file list

```diff
@@ -1,861 +1,861 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:57.692029 ovos_plugin_common_play-0.0.5a7/
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-20 00:32:57.692029 ovos_plugin_common_play-0.0.5a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:57.608028 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/
--rw-r--r--   0 runner    (1001) docker     (123)    10556 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:57.612028 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/
--rw-r--r--   0 runner    (1001) docker     (123)    16591 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/base.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    20851 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)    22068 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/media.py
--rw-r--r--   0 runner    (1001) docker     (123)    23111 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/mpris.py
--rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/mycroft_cps.py
--rw-r--r--   0 runner    (1001) docker     (123)    37856 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/player.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:57.608028 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:57.612028 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/desktop/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/desktop/OCP.desktop
--rw-r--r--   0 runner    (1001) docker     (123)    34972 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/desktop/OCP.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:57.608028 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:57.620028 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/Music.voc
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/Next.voc
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/Pause.voc
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/PlayResume.voc
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/Prev.voc
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/Resume.voc
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/Track.voc
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/audio.intent
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/audio_only.voc
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/audiobook.intent
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/behind_scenes.intent
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/behind_scenes.voc
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/bw_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/cant.play.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/comic.intent
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/converse_resume.voc
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/documentaries.intent
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/featured.intent
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/game.intent
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/hentai.intent
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/just.one.moment.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/movietrailer.intent
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/music.intent
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/news.intent
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/next.intent
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/open.intent
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/pause.intent
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/phrase.rx
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/play.intent
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/play.what.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/podcast.intent
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/porn.intent
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/prev.intent
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/radio.intent
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/radio_drama.intent
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/read.intent
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/resume.intent
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/setup.hints.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/short_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/silent_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/trailer.voc
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/tv.intent
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/video.intent
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/video_only.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:57.628028 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/Music.voc
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/Next.voc
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/Pause.voc
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/PlayResume.voc
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/Prev.voc
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/Resume.voc
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/Track.voc
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/audio.intent
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/audio_only.voc
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/audiobook.intent
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/behind_scenes.intent
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/behind_scenes.voc
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/bw_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/cant.play.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/comic.intent
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/converse_resume.voc
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/documentaries.intent
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/featured.intent
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/game.intent
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/hentai.intent
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/just.one.moment.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/movietrailer.intent
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/music.intent
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/news.intent
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/next.intent
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/open.intent
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/pause.intent
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/play.intent
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/play.what.dialog
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/podcast.intent
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/porn.intent
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/prev.intent
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/radio.intent
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/radio_drama.intent
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/read.intent
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/resume.intent
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/setup.hints.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/short_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/silent_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/trailer.voc
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/tv.intent
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/video.intent
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/video_only.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:57.636028 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/Music.voc
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/Next.voc
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/Pause.voc
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/PlayResume.voc
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/Prev.voc
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/Resume.voc
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/Track.voc
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/audio.intent
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/audio_only.voc
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/audiobook.intent
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/behind_scenes.intent
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/behind_scenes.voc
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/bw_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/cant.play.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/comic.intent
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/converse_resume.voc
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/documentaries.intent
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/featured.intent
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/game.intent
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/hentai.intent
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/just.one.moment.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/movietrailer.intent
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/music.intent
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/news.intent
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/next.intent
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/open.intent
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/pause.intent
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/play.intent
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/play.what.dialog
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/podcast.intent
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/porn.intent
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/prev.intent
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/radio.intent
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/radio_drama.intent
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/read.intent
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/resume.intent
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/setup.hints.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/short_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/silent_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/trailer.voc
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/tv.intent
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/video.intent
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/video_only.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:57.640028 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/Music.voc
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/Next.voc
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/Pause.voc
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/Prev.voc
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/Resume.voc
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/Track.voc
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/audio.intent
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/audio_only.voc
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/audiobook.intent
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/behind_scenes.intent
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/bw_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/cant.play.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/comic.intent
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/converse_resume.voc
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/documentaries.intent
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/game.intent
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/just.one.moment.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/movietrailer.intent
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/music.intent
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/news.intent
--rwxr-xr-x   0 runner    (1001) docker     (123)     1350 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/next.intent
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/open.intent
--rwxr-xr-x   0 runner    (1001) docker     (123)      554 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/pause.intent
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/phrase.rx
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/play.intent
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/play.what.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/podcast.intent
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/porn.intent
--rwxr-xr-x   0 runner    (1001) docker     (123)     2937 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/prev.intent
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/radio.intent
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/radio_drama.intent
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/read.intent
--rwxr-xr-x   0 runner    (1001) docker     (123)      233 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/resume.intent
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/setup.hints.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/short_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/silent_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/tv.intent
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/video.intent
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/video_only.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:57.640028 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/Music.voc
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/Next.voc
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/Pause.voc
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/PlayResume.voc
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/Prev.voc
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/Resume.voc
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/Track.voc
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/audio.intent
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/audio_only.voc
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/audiobook.intent
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/behind_scenes.intent
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/behind_scenes.voc
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/bw_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/cant.play.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/comic.intent
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/converse_resume.voc
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/documentaries.intent
--rwxr-xr-x   0 runner    (1001) docker     (123)      106 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/featured.intent
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/game.intent
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/hentai.intent
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/just.one.moment.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/movietrailer.intent
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/music.intent
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/news.intent
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/next.intent
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/open.intent
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/pause.intent
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/phrase.rx
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/play.intent
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/play.what.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/podcast.intent
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/porn.intent
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/prev.intent
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/radio.intent
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/radio_drama.intent
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/read.intent
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/resume.intent
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/setup.hints.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/short_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/silent_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/trailer.voc
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/tv.intent
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/video.intent
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/video_only.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:57.644028 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/Music.voc
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/Next.voc
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/Pause.voc
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/PlayResume.voc
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/Prev.voc
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/Resume.voc
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/Track.voc
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/audio.intent
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/audio_only.voc
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/audiobook.intent
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/behind_scenes.intent
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/behind_scenes.voc
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/bw_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/cant.play.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/comic.intent
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/converse_resume.voc
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/documentaries.intent
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/featured.intent
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/game.intent
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/hentai.intent
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/just.one.moment.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/movietrailer.intent
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/music.intent
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/news.intent
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/next.intent
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/open.intent
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/pause.intent
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/play.intent
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/play.what.dialog
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/podcast.intent
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/porn.intent
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/prev.intent
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/radio.intent
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/radio_drama.intent
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/read.intent
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/resume.intent
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/setup.hints.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/short_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/silent_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/trailer.voc
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/tv.intent
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/video.intent
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/video_only.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:57.648028 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/Music.voc
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/Next.voc
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/Pause.voc
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/PlayResume.voc
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/Prev.voc
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/Resume.voc
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/Track.voc
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/audio.intent
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/audio_only.voc
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/audiobook.intent
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/behind_scenes.intent
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/behind_scenes.voc
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/bw_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/cant.play.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/comic.intent
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/converse_resume.voc
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/documentaries.intent
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/featured.intent
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/game.intent
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/hentai.intent
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/just.one.moment.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/movietrailer.intent
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/music.intent
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/news.intent
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/next.intent
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/open.intent
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/pause.intent
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/play.intent
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/play.what.dialog
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/podcast.intent
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/porn.intent
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/prev.intent
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/radio.intent
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/radio_drama.intent
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/read.intent
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/resume.intent
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/setup.hints.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/short_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/silent_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/trailer.voc
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/tv.intent
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/video.intent
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/video_only.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:57.652028 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/Music.voc
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/Next.voc
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/Pause.voc
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/PlayResume.voc
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/Prev.voc
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/Resume.voc
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/Track.voc
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/audio.intent
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/audio_only.voc
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/audiobook.intent
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/behind_scenes.intent
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/behind_scenes.voc
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/bw_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/cant.play.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/comic.intent
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/converse_resume.voc
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/documentaries.intent
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/featured.intent
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/game.intent
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/hentai.intent
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/just.one.moment.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/movietrailer.intent
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/music.intent
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/news.intent
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/next.intent
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/open.intent
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/pause.intent
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/play.intent
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/play.what.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/podcast.intent
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/porn.intent
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/prev.intent
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/radio.intent
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/radio_drama.intent
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/read.intent
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/resume.intent
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/setup.hints.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/short_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/silent_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/trailer.voc
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/tv.intent
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/video.intent
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/video_only.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:57.656028 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/Music.voc
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/Next.voc
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/Pause.voc
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/PlayResume.voc
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/Prev.voc
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/Resume.voc
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/Track.voc
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/audio.intent
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/audio_only.voc
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/audiobook.intent
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/behind_scenes.intent
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/behind_scenes.voc
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/bw_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/cant.play.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/comic.intent
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/converse_resume.voc
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/documentaries.intent
--rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/featured.intent
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/game.intent
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/hentai.intent
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/just.one.moment.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/movietrailer.intent
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/music.intent
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/news.intent
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/next.intent
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/open.intent
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/pause.intent
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/phrase.rx
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/play.intent
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/play.what.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/podcast.intent
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/porn.intent
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/prev.intent
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/radio.intent
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/radio_drama.intent
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/read.intent
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/resume.intent
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/setup.hints.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/short_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/silent_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/trailer.voc
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/tv.intent
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/video.intent
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/it-it/video_only.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:57.660028 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/Music.voc
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/Next.voc
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/Pause.voc
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/PlayResume.voc
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/Prev.voc
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/Resume.voc
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/Track.voc
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/audio.intent
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/audio_only.voc
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/audiobook.intent
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/behind_scenes.intent
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/behind_scenes.voc
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/bw_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/cant.play.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/comic.intent
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/converse_resume.voc
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/documentaries.intent
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/featured.intent
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/game.intent
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/just.one.moment.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/movietrailer.intent
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/music.intent
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/news.intent
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/next.intent
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/open.intent
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/pause.intent
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/play.intent
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/play.what.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/podcast.intent
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/porn.intent
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/prev.intent
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/radio.intent
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/radio_drama.intent
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/read.intent
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/resume.intent
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/setup.hints.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/short_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/silent_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/trailer.voc
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/tv.intent
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/video.intent
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/video_only.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:57.664028 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/Music.voc
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/Next.voc
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/Pause.voc
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/PlayResume.voc
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/Prev.voc
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/Resume.voc
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/Track.voc
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/audio.intent
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/audio_only.voc
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/audiobook.intent
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/behind_scenes.intent
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/behind_scenes.voc
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/bw_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/cant.play.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/comic.intent
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/converse_resume.voc
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/documentaries.intent
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/featured.intent
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/game.intent
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/hentai.intent
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/just.one.moment.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/movietrailer.intent
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/music.intent
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/news.intent
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/next.intent
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/open.intent
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/pause.intent
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/play.intent
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/play.what.dialog
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/podcast.intent
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/porn.intent
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/prev.intent
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/radio.intent
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/radio_drama.intent
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/read.intent
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/resume.intent
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/setup.hints.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/short_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/silent_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/trailer.voc
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/tv.intent
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/video.intent
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/video_only.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:57.668028 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/Music.voc
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/Next.voc
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/Pause.voc
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/PlayResume.voc
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/Prev.voc
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/Resume.voc
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/Track.voc
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/audio.intent
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/audio_only.voc
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/audiobook.intent
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/behind_scenes.intent
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/behind_scenes.voc
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/bw_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/cant.play.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/comic.intent
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/converse_resume.voc
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/documentaries.intent
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/featured.intent
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/game.intent
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/hentai.intent
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/just.one.moment.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/movietrailer.intent
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/music.intent
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/news.intent
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/next.intent
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/open.intent
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/pause.intent
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/play.intent
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/play.what.dialog
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/podcast.intent
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/porn.intent
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/prev.intent
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/radio.intent
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/radio_drama.intent
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/read.intent
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/resume.intent
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/setup.hints.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/short_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/silent_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/trailer.voc
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/tv.intent
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/video.intent
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/video_only.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:57.672028 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/Music.voc
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/Next.voc
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/Pause.voc
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/PlayResume.voc
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/Prev.voc
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/Resume.voc
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/Track.voc
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/audio.intent
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/audio_only.voc
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/audiobook.intent
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/behind_scenes.intent
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/behind_scenes.voc
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/bw_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/cant.play.dialog
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/comic.intent
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/converse_resume.voc
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/documentaries.intent
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/featured.intent
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/game.intent
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/hentai.intent
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/just.one.moment.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/movietrailer.intent
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/music.intent
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/news.intent
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/next.intent
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/open.intent
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/pause.intent
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/play.intent
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/play.what.dialog
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/podcast.intent
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/porn.intent
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/prev.intent
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/radio.intent
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/radio_drama.intent
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/read.intent
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/resume.intent
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/setup.hints.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/short_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/silent_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/trailer.voc
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/tv.intent
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/video.intent
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/video_only.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:57.676029 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/Music.voc
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/Next.voc
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/Pause.voc
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/PlayResume.voc
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/Prev.voc
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/Resume.voc
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/Track.voc
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/audio.intent
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/audio_only.voc
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/audiobook.intent
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/behind_scenes.intent
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/behind_scenes.voc
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/bw_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/cant.play.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/comic.intent
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/converse_resume.voc
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/documentaries.intent
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/featured.intent
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/game.intent
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/hentai.intent
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/just.one.moment.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/movietrailer.intent
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/music.intent
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/news.intent
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/next.intent
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/open.intent
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/pause.intent
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/play.intent
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/play.what.dialog
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/podcast.intent
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/porn.intent
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/prev.intent
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/radio.intent
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/radio_drama.intent
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/read.intent
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/resume.intent
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/setup.hints.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/short_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/silent_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/trailer.voc
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/tv.intent
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/video.intent
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/video_only.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:57.680029 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/Music.voc
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/Next.voc
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/Pause.voc
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/PlayResume.voc
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/Prev.voc
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/Resume.voc
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/Track.voc
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/audio.intent
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/audio_only.voc
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/audiobook.intent
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/behind_scenes.intent
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/behind_scenes.voc
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/bw_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/cant.play.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/comic.intent
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/converse_resume.voc
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/documentaries.intent
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/featured.intent
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/game.intent
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/hentai.intent
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/just.one.moment.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/movietrailer.intent
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/music.intent
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/news.intent
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/next.intent
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/open.intent
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/pause.intent
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/play.intent
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/play.what.dialog
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/podcast.intent
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/porn.intent
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/prev.intent
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/radio.intent
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/radio_drama.intent
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/read.intent
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/resume.intent
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/setup.hints.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/short_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/silent_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/trailer.voc
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/tv.intent
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/video.intent
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/video_only.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:57.684029 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/Music.voc
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/Next.voc
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/Pause.voc
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/PlayResume.voc
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/Prev.voc
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/Resume.voc
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/Track.voc
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/audio.intent
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/audio_only.voc
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/audiobook.intent
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/behind_scenes.intent
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/behind_scenes.voc
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/bw_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/cant.play.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/comic.intent
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/converse_resume.voc
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/documentaries.intent
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/featured.intent
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/game.intent
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/hentai.intent
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/just.one.moment.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/movietrailer.intent
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/music.intent
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/news.intent
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/next.intent
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/open.intent
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/pause.intent
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/play.intent
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/play.what.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/podcast.intent
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/porn.intent
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/prev.intent
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/radio.intent
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/radio_drama.intent
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/read.intent
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/resume.intent
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/setup.hints.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/short_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/silent_movie.intent
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/trailer.voc
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/tv.intent
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/video.intent
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/video_only.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:57.688029 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:57.688029 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/AudioPlayerControl.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/Disambiguation.qml
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/Home.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/NowPlayingHomeBar.qml
--rwxr-xr-x   0 runner    (1001) docker     (123)     2896 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OCPSkillsView.qml
--rw-r--r--   0 runner    (1001) docker     (123)    21593 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSAudioPlayer.qml
--rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSSeekControl.qml
--rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSSeekControlQtAv.qml
--rw-r--r--   0 runner    (1001) docker     (123)    11467 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSSyncPlayer.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSVideoPlayer.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSVideoPlayerQtAv.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSWebPlayer.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/PlayerLoader.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/Playlist.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/Search.qml
--rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/SpectrumWaveDelegate.qml
--rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/SuggestionsView.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/VideoPlayerControl.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/AudioPlayerControl.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/ConfigDelegateLayoutItem.qml
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/ConfigOptionDelegate.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/ConfigSliderDelegate.qml
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/ConfigSwitchDelegate.qml
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/Disambiguation.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/GenericCloseControl.qml
--rw-r--r--   0 runner    (1001) docker     (123)     9888 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/Home.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/NowPlayingHomeBar.qml
--rwxr-xr-x   0 runner    (1001) docker     (123)     2788 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/OCPSkillsView.qml
--rw-r--r--   0 runner    (1001) docker     (123)    21245 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/OVOSAudioPlayer.qml
--rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/OVOSSeekControl.qml
--rw-r--r--   0 runner    (1001) docker     (123)    11549 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/OVOSSeekControlQtAv.qml
--rw-r--r--   0 runner    (1001) docker     (123)     9988 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/OVOSSyncPlayer.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/OVOSVideoPlayer.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/OVOSVideoPlayerQtAv.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/OVOSWebPlayer.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/PlayerLoader.qml
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/Playlist.qml
--rw-r--r--   0 runner    (1001) docker     (123)    15057 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/Search.qml
--rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/SpectrumWaveDelegate.qml
--rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/SuggestionsView.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/VideoPlayerControl.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:57.688029 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/animations/
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/animations/status-fail.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:57.688029 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/code/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/code/helper.js
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/code/nav.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:57.688029 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/delegates/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4508 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/delegates/GridSkillCard.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:57.692029 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/back.png
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/back.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/history.png
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/home.png
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/information.png
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-album-track.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-fullscreen.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-mute.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-next.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-pause.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-play.svg
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-playback-pause.svg
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-playback-start.svg
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-playback-stop.svg
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-playlist-play.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-playlist-repeat-track.svg
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-playlist-repeat.svg
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-playlist-shuffle.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-previous.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-repeat-playlist.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-repeat-track.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-repeat.svg
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-seek-backward.svg
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-seek-forward.svg
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-skip-backward.svg
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-skip-forward.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-stop.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-unmute.svg
--rw-r--r--   0 runner    (1001) docker     (123)    34972 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/ocp-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    36598 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/ocp-light.png
--rw-r--r--   0 runner    (1001) docker     (123)    48707 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/ocp.png
--rw-r--r--   0 runner    (1001) docker     (123)    74222 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/ocp_bg.png
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/search.png
--rw-r--r--   0 runner    (1001) docker     (123)    97623 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/spinner.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:57.692029 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/views/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3171 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/views/GridTileView.qml
--rwxr-xr-x   0 runner    (1001) docker     (123)     4927 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/views/TileView.qml
--rw-r--r--   0 runner    (1001) docker     (123)    19474 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:32:57.608028 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-20 00:32:57.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    48631 2023-04-20 00:32:57.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 00:32:57.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-20 00:32:57.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-20 00:32:57.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-20 00:32:57.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 00:32:57.000000 ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 00:32:57.692029 ovos_plugin_common_play-0.0.5a7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3471 2023-04-20 00:32:56.000000 ovos_plugin_common_play-0.0.5a7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:04.575835 ovos_plugin_common_play-0.0.6a1/
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-23 00:23:04.571835 ovos_plugin_common_play-0.0.6a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:04.431834 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/
+-rw-r--r--   0 runner    (1001) docker     (123)    10556 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:04.435834 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/
+-rw-r--r--   0 runner    (1001) docker     (123)    16591 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20851 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22072 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23111 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/mpris.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/mycroft_cps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37856 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/player.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:04.431834 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:04.435834 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/desktop/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/desktop/OCP.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)    34972 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/desktop/OCP.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:04.431834 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:04.443834 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/Music.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/Next.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/Pause.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/PlayResume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/Prev.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/Resume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/Track.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/audio.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/audio_only.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/audiobook.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/behind_scenes.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/behind_scenes.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/bw_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/cant.play.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/comic.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/converse_resume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/documentaries.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/featured.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/game.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/hentai.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/just.one.moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/movietrailer.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/music.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/news.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/next.intent
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/open.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/pause.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/phrase.rx
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/play.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/play.what.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/podcast.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/porn.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/prev.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/radio.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/radio_drama.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/read.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/resume.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/setup.hints.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/short_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/silent_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/trailer.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/tv.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/video.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/video_only.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:04.447834 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/Music.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/Next.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/Pause.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/PlayResume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/Prev.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/Resume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/Track.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/audio.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/audio_only.voc
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/audiobook.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/behind_scenes.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/behind_scenes.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/bw_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/cant.play.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/comic.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/converse_resume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/documentaries.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/featured.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/game.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/hentai.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/just.one.moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/movietrailer.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/music.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/news.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/next.intent
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/open.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/pause.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/play.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/play.what.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/podcast.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/porn.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/prev.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/radio.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/radio_drama.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/read.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/resume.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/setup.hints.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/short_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/silent_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/trailer.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/tv.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/video.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/video_only.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:04.455834 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/Music.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/Next.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/Pause.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/PlayResume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/Prev.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/Resume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/Track.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/audio.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/audio_only.voc
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/audiobook.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/behind_scenes.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/behind_scenes.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/bw_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/cant.play.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/comic.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/converse_resume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/documentaries.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/featured.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/game.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/hentai.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/just.one.moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/movietrailer.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/music.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/news.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/next.intent
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/open.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/pause.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/play.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/play.what.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/podcast.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/porn.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/prev.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/radio.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/radio_drama.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/read.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/resume.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/setup.hints.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/short_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/silent_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/trailer.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/tv.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/video.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/video_only.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:04.463834 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/Music.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/Next.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/Pause.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/Prev.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/Resume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/Track.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/audio.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/audio_only.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/audiobook.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/behind_scenes.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/bw_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/cant.play.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/comic.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/converse_resume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/documentaries.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/game.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/just.one.moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/movietrailer.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/music.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/news.intent
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1350 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/next.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/open.intent
+-rwxr-xr-x   0 runner    (1001) docker     (123)      554 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/pause.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/phrase.rx
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/play.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/play.what.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/podcast.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/porn.intent
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2937 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/prev.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/radio.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/radio_drama.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/read.intent
+-rwxr-xr-x   0 runner    (1001) docker     (123)      233 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/resume.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/setup.hints.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/short_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/silent_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/tv.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/video.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/video_only.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:04.471834 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/Music.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/Next.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/Pause.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/PlayResume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/Prev.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/Resume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/Track.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/audio.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/audio_only.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/audiobook.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/behind_scenes.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/behind_scenes.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/bw_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/cant.play.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/comic.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/converse_resume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/documentaries.intent
+-rwxr-xr-x   0 runner    (1001) docker     (123)      106 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/featured.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/game.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/hentai.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/just.one.moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/movietrailer.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/music.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/news.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/next.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/open.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/pause.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/phrase.rx
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/play.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/play.what.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/podcast.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/porn.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/prev.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/radio.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/radio_drama.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/read.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/resume.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/setup.hints.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/short_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/silent_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/trailer.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/tv.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/video.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/video_only.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:04.475834 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/Music.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/Next.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/Pause.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/PlayResume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/Prev.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/Resume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/Track.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/audio.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/audio_only.voc
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/audiobook.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/behind_scenes.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/behind_scenes.voc
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/bw_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/cant.play.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/comic.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/converse_resume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/documentaries.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/featured.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/game.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/hentai.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/just.one.moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/movietrailer.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/music.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/news.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/next.intent
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/open.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/pause.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/play.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/play.what.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/podcast.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/porn.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/prev.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/radio.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/radio_drama.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/read.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/resume.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/setup.hints.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/short_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/silent_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/trailer.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/tv.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/video.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/video_only.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:04.483834 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/Music.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/Next.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/Pause.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/PlayResume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/Prev.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/Resume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/Track.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/audio.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/audio_only.voc
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/audiobook.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/behind_scenes.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/behind_scenes.voc
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/bw_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/cant.play.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/comic.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/converse_resume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/documentaries.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/featured.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/game.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/hentai.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/just.one.moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/movietrailer.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/music.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/news.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/next.intent
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/open.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/pause.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/play.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/play.what.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/podcast.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/porn.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/prev.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/radio.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/radio_drama.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/read.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/resume.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/setup.hints.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/short_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/silent_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/trailer.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/tv.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/video.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/video_only.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:04.491834 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/Music.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/Next.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/Pause.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/PlayResume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/Prev.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/Resume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/Track.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/audio.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/audio_only.voc
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/audiobook.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/behind_scenes.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/behind_scenes.voc
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/bw_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/cant.play.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/comic.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/converse_resume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/documentaries.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/featured.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/game.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/hentai.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/just.one.moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/movietrailer.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/music.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/news.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/next.intent
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/open.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/pause.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/play.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/play.what.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/podcast.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/porn.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/prev.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/radio.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/radio_drama.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/read.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/resume.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/setup.hints.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/short_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/silent_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/trailer.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/tv.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/video.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/video_only.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:04.503834 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/Music.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/Next.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/Pause.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/PlayResume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/Prev.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/Resume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/Track.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/audio.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/audio_only.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/audiobook.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/behind_scenes.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/behind_scenes.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/bw_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/cant.play.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/comic.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/converse_resume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/documentaries.intent
+-rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/featured.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/game.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/hentai.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/just.one.moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/movietrailer.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/music.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/news.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/next.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/open.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/pause.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/phrase.rx
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/play.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/play.what.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/podcast.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/porn.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/prev.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/radio.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/radio_drama.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/read.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/resume.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/setup.hints.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/short_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/silent_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/trailer.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/tv.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/video.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/it-it/video_only.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:04.511834 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/Music.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/Next.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/Pause.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/PlayResume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/Prev.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/Resume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/Track.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/audio.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/audio_only.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/audiobook.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/behind_scenes.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/behind_scenes.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/bw_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/cant.play.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/comic.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/converse_resume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/documentaries.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/featured.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/game.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/just.one.moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/movietrailer.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/music.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/news.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/next.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/open.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/pause.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/play.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/play.what.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/podcast.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/porn.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/prev.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/radio.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/radio_drama.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/read.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/resume.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/setup.hints.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/short_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/silent_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/trailer.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/tv.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/video.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/video_only.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:04.515834 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/Music.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/Next.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/Pause.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/PlayResume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/Prev.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/Resume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/Track.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/audio.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/audio_only.voc
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/audiobook.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/behind_scenes.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/behind_scenes.voc
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/bw_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/cant.play.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/comic.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/converse_resume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/documentaries.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/featured.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/game.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/hentai.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/just.one.moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/movietrailer.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/music.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/news.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/next.intent
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/open.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/pause.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/play.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/play.what.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/podcast.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/porn.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/prev.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/radio.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/radio_drama.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/read.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/resume.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/setup.hints.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/short_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/silent_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/trailer.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/tv.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/video.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/video_only.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:04.523834 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/Music.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/Next.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/Pause.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/PlayResume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/Prev.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/Resume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/Track.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/audio.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/audio_only.voc
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/audiobook.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/behind_scenes.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/behind_scenes.voc
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/bw_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/cant.play.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/comic.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/converse_resume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/documentaries.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/featured.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/game.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/hentai.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/just.one.moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/movietrailer.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/music.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/news.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/next.intent
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/open.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/pause.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/play.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/play.what.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/podcast.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/porn.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/prev.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/radio.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/radio_drama.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/read.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/resume.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/setup.hints.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/short_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/silent_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/trailer.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/tv.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/video.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/video_only.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:04.531834 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/Music.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/Next.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/Pause.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/PlayResume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/Prev.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/Resume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/Track.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/audio.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/audio_only.voc
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/audiobook.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/behind_scenes.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/behind_scenes.voc
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/bw_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/cant.play.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/comic.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/converse_resume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/documentaries.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/featured.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/game.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/hentai.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/just.one.moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/movietrailer.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/music.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/news.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/next.intent
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/open.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/pause.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/play.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/play.what.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/podcast.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/porn.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/prev.intent
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/radio.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/radio_drama.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/read.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/resume.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/setup.hints.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/short_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/silent_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/trailer.voc
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/tv.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/video.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/video_only.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:04.539834 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/Music.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/Next.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/Pause.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/PlayResume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/Prev.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/Resume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/Track.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/audio.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/audio_only.voc
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/audiobook.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/behind_scenes.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/behind_scenes.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/bw_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/cant.play.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/comic.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/converse_resume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/documentaries.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/featured.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/game.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/hentai.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/just.one.moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/movietrailer.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/music.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/news.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/next.intent
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/open.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/pause.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/play.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/play.what.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/podcast.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/porn.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/prev.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/radio.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/radio_drama.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/read.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/resume.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/setup.hints.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/short_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/silent_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/trailer.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/tv.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/video.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/video_only.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:04.551834 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/Music.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/Next.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/Pause.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/PlayResume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/Prev.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/Resume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/Track.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/audio.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/audio_only.voc
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/audiobook.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/behind_scenes.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/behind_scenes.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/bw_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/cant.play.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/comic.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/converse_resume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/documentaries.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/featured.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/game.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/hentai.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/just.one.moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/movietrailer.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/music.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/news.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/next.intent
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/open.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/pause.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/play.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/play.what.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/podcast.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/porn.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/prev.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/radio.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/radio_drama.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/read.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/resume.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/setup.hints.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/short_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/silent_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/trailer.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/tv.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/video.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/video_only.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:04.559835 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/Music.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/Next.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/Pause.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/PlayResume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/Prev.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/Resume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/Track.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/audio.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/audio_only.voc
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/audiobook.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/behind_scenes.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/behind_scenes.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/bw_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/cant.play.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/comic.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/converse_resume.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/documentaries.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/featured.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/game.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/hentai.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/just.one.moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/movietrailer.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/music.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/news.intent
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/next.intent
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/open.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/pause.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/play.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/play.what.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/podcast.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/porn.intent
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/prev.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/radio.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/radio_drama.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/read.intent
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/resume.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/setup.hints.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/short_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/silent_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/trailer.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/tv.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/video.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/video_only.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:04.563835 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:04.567834 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/AudioPlayerControl.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/Disambiguation.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/Home.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/NowPlayingHomeBar.qml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2896 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OCPSkillsView.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    21593 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSAudioPlayer.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSSeekControl.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSSeekControlQtAv.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    11467 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSSyncPlayer.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSVideoPlayer.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSVideoPlayerQtAv.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSWebPlayer.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/PlayerLoader.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/Playlist.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/Search.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/SpectrumWaveDelegate.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/SuggestionsView.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/VideoPlayerControl.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/AudioPlayerControl.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/ConfigDelegateLayoutItem.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/ConfigOptionDelegate.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/ConfigSliderDelegate.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/ConfigSwitchDelegate.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/Disambiguation.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/GenericCloseControl.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     9888 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/Home.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/NowPlayingHomeBar.qml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2788 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/OCPSkillsView.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    21245 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/OVOSAudioPlayer.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/OVOSSeekControl.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    11549 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/OVOSSeekControlQtAv.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     9988 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/OVOSSyncPlayer.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/OVOSVideoPlayer.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/OVOSVideoPlayerQtAv.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/OVOSWebPlayer.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/PlayerLoader.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/Playlist.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    15057 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/Search.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/SpectrumWaveDelegate.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/SuggestionsView.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/VideoPlayerControl.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:04.567834 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/animations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/animations/status-fail.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:04.567834 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/code/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/code/helper.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/code/nav.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:04.567834 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/delegates/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4508 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/delegates/GridSkillCard.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:04.571835 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/back.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/back.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/history.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/home.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/information.png
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-album-track.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-fullscreen.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-mute.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-next.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-pause.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-play.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-playback-pause.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-playback-start.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-playback-stop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-playlist-play.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-playlist-repeat-track.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-playlist-repeat.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-playlist-shuffle.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-previous.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-repeat-playlist.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-repeat-track.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-repeat.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-seek-backward.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-seek-forward.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-skip-backward.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-skip-forward.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-stop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-unmute.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    34972 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/ocp-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36598 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/ocp-light.png
+-rw-r--r--   0 runner    (1001) docker     (123)    48707 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/ocp.png
+-rw-r--r--   0 runner    (1001) docker     (123)    74222 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/ocp_bg.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/search.png
+-rw-r--r--   0 runner    (1001) docker     (123)    97623 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/spinner.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:04.571835 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/views/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3171 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/views/GridTileView.qml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4927 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/views/TileView.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    19474 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 00:23:04.435834 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-23 00:23:04.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    48631 2023-04-23 00:23:04.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 00:23:04.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-23 00:23:04.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-23 00:23:04.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-23 00:23:04.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 00:23:04.000000 ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 00:23:04.575835 ovos_plugin_common_play-0.0.6a1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3471 2023-04-23 00:23:03.000000 ovos_plugin_common_play-0.0.6a1/setup.py
```

### Comparing `ovos_plugin_common_play-0.0.5a7/LICENSE` & `ovos_plugin_common_play-0.0.6a1/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/PKG-INFO` & `ovos_plugin_common_play-0.0.6a1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos_plugin_common_play
-Version: 0.0.5a7
+Version: 0.0.6a1
 Summary: OVOS common play audio service adapter plugin
 Home-page: https://github.com/OpenVoiceOS/ovos-ocp-audio-plugin
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: ovos audio plugin
 Platform: UNKNOWN
```

### Comparing `ovos_plugin_common_play-0.0.5a7/README.md` & `ovos_plugin_common_play-0.0.6a1/README.md`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/__init__.py` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/__init__.py` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/base.py` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/base.py`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/gui.py` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/gui.py`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/media.py` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/media.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional, Tuple, List, Union
 
-from mycroft_bus_client import MessageBusClient
+from ovos_bus_client.client import MessageBusClient
 from ovos_plugin_common_play.ocp import OCP_ID
 from ovos_plugin_common_play.ocp.status import *
 from ovos_plugin_common_play.ocp.utils import ocp_plugins, find_mime
 from ovos_utils.json_helper import merge_dict
 from ovos_utils.log import LOG
 from ovos_utils.messagebus import Message
 from os.path import join, dirname
```

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/mpris.py` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/mpris.py`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/mycroft_cps.py` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/mycroft_cps.py`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/player.py` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/player.py`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/desktop/OCP.png` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/desktop/OCP.png`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/audiobook.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/audiobook.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/bw_movie.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/bw_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/comic.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/comic.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/documentaries.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/documentaries.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/open.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/open.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/short_movie.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/short_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/silent_movie.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/silent_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ca-es/tv.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ca-es/tv.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/audiobook.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/audiobook.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/bw_movie.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/bw_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/comic.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/comic.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/featured.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/featured.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/hentai.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/hentai.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/movietrailer.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/movietrailer.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/open.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/open.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/play.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/play.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/podcast.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/podcast.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/radio.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/radio.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/tv.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/cs-cz/tv.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/audiobook.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/audiobook.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/bw_movie.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/bw_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/comic.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/comic.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/documentaries.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/documentaries.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/hentai.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/hentai.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/open.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/open.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/play.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/play.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/podcast.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/podcast.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/radio.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/radio.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/da-dk/tv.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/da-dk/tv.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/audiobook.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/audiobook.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/bw_movie.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/bw_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/next.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/next.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/pause.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/pause.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/de-de/prev.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/de-de/prev.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/en-us/audiobook.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/en-us/audiobook.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/audiobook.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/audiobook.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/behind_scenes.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/behind_scenes.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/bw_movie.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/bw_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/comic.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/comic.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/featured.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/featured.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/hentai.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/hentai.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/movietrailer.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/movietrailer.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/open.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/open.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/podcast.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/podcast.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/radio.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/radio.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/resume.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/resume.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/short_movie.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/short_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/silent_movie.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/silent_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/es-es/tv.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/es-es/tv.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/audiobook.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/audiobook.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/bw_movie.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/bw_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/comic.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/comic.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/documentaries.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/documentaries.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/featured.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/featured.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/hentai.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/hentai.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/movietrailer.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/movietrailer.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/open.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/open.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/play.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/play.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/podcast.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/podcast.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/radio.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/radio.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/short_movie.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/short_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/tv.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/fr-fr/tv.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/audiobook.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/audiobook.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/bw_movie.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/bw_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/comic.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/comic.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/featured.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/featured.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/hentai.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/hentai.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/movietrailer.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/movietrailer.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/open.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/open.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/play.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/play.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/podcast.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/podcast.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/radio.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/radio.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/short_movie.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/short_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/tv.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/hu-hu/tv.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/audiobook.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/audiobook.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/next.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/next.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/prev.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/nl-nl/prev.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/audiobook.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/audiobook.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/bw_movie.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/bw_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/movie.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/open.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/open.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/play.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/play.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/podcast.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/podcast.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/short_movie.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/short_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/tv.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pl-pl/tv.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/audiobook.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/audiobook.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/bw_movie.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/bw_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/comic.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/comic.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/featured.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/featured.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/hentai.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/hentai.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/movietrailer.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/movietrailer.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/open.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/open.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/play.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/play.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/podcast.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/podcast.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/radio.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/radio.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/short_movie.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/short_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/silent_movie.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/silent_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/tv.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/pt-pt/tv.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/audiobook.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/audiobook.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/behind_scenes.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/behind_scenes.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/bw_movie.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/bw_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/comic.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/comic.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/documentaries.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/documentaries.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/featured.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/featured.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/hentai.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/hentai.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/movietrailer.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/movietrailer.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/next.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/next.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/open.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/open.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/play.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/play.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/podcast.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/podcast.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/prev.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/prev.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/radio.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/radio.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/resume.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/resume.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/setup.hints.dialog` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/setup.hints.dialog`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/short_movie.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/short_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/silent_movie.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/silent_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/tv.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/ru-ru/tv.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/audiobook.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/audiobook.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/bw_movie.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/bw_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/comic.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/comic.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/hentai.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/hentai.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/movietrailer.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/movietrailer.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/open.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/open.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/play.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/play.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/podcast.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/podcast.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/radio.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/radio.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/tv.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-fi/tv.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/audiobook.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/audiobook.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/bw_movie.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/bw_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/comic.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/comic.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/hentai.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/hentai.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/movietrailer.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/movietrailer.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/open.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/open.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/play.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/play.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/podcast.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/podcast.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/radio.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/radio.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/sv-se/tv.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/sv-se/tv.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/Music.voc` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/Music.voc`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/Next.voc` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/Next.voc`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/Play.voc` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/Play.voc`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/Prev.voc` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/Prev.voc`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/audiobook.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/audiobook.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/bw_movie.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/bw_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/comic.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/comic.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/featured.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/featured.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/hentai.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/hentai.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/next.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/next.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/open.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/open.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/podcast.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/podcast.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/prev.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/prev.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/radio.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/radio.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/resume.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/resume.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/tv.intent` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/locale/tr-tr/tv.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/AudioPlayerControl.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/AudioPlayerControl.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/Disambiguation.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/Disambiguation.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/Home.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/Home.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/NowPlayingHomeBar.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/NowPlayingHomeBar.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OCPSkillsView.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OCPSkillsView.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSAudioPlayer.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSAudioPlayer.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSSeekControl.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSSeekControl.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSSeekControlQtAv.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSSeekControlQtAv.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSSyncPlayer.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSSyncPlayer.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSVideoPlayer.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSVideoPlayer.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSVideoPlayerQtAv.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSVideoPlayerQtAv.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSWebPlayer.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSWebPlayer.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/PlayerLoader.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/PlayerLoader.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/Playlist.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/Playlist.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/Search.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/Search.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/SpectrumWaveDelegate.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/SpectrumWaveDelegate.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/SuggestionsView.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/SuggestionsView.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/VideoPlayerControl.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/+mediacenter/VideoPlayerControl.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/AudioPlayerControl.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/AudioPlayerControl.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/ConfigDelegateLayoutItem.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/ConfigDelegateLayoutItem.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/ConfigSliderDelegate.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/ConfigSliderDelegate.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/ConfigSwitchDelegate.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/ConfigSwitchDelegate.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/Disambiguation.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/Disambiguation.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/GenericCloseControl.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/GenericCloseControl.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/Home.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/Home.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/NowPlayingHomeBar.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/NowPlayingHomeBar.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/OCPSkillsView.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/OCPSkillsView.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/OVOSAudioPlayer.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/OVOSAudioPlayer.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/OVOSSeekControl.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/OVOSSeekControl.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/OVOSSeekControlQtAv.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/OVOSSeekControlQtAv.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/OVOSSyncPlayer.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/OVOSSyncPlayer.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/OVOSVideoPlayer.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/OVOSVideoPlayer.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/OVOSVideoPlayerQtAv.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/OVOSVideoPlayerQtAv.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/OVOSWebPlayer.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/OVOSWebPlayer.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/PlayerLoader.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/PlayerLoader.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/Playlist.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/Playlist.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/Search.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/Search.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/SpectrumWaveDelegate.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/SpectrumWaveDelegate.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/SuggestionsView.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/SuggestionsView.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/VideoPlayerControl.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/VideoPlayerControl.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/animations/status-fail.json` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/animations/status-fail.json`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/code/nav.js` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/code/nav.js`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/delegates/GridSkillCard.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/delegates/GridSkillCard.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/back.png` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/back.png`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/back.svg` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/back.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/history.png` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/history.png`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/home.png` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/home.png`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/information.png` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/information.png`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-album-track.svg` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-album-track.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-fullscreen.svg` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-fullscreen.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-mute.svg` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-mute.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-next.svg` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-next.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-pause.svg` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-pause.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-play.svg` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-play.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-playlist-play.svg` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-playlist-play.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-playlist-repeat-track.svg` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-playlist-repeat-track.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-playlist-repeat.svg` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-playlist-repeat.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-playlist-shuffle.svg` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-playlist-shuffle.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-previous.svg` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-previous.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-repeat-playlist.svg` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-repeat-playlist.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-repeat-track.svg` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-repeat-track.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-repeat.svg` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-repeat.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-stop.svg` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-stop.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/media-unmute.svg` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/media-unmute.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/ocp-dark.png` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/ocp-dark.png`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/ocp-light.png` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/ocp-light.png`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/ocp.png` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/ocp.png`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/ocp_bg.png` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/ocp_bg.png`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/search.png` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/search.png`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/images/spinner.gif` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/images/spinner.gif`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/views/GridTileView.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/views/GridTileView.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/res/ui/views/TileView.qml` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/res/ui/views/TileView.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/search.py` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/search.py`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/status.py` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/status.py`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play/ocp/utils.py` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play/ocp/utils.py`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play.egg-info/PKG-INFO` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-plugin-common-play
-Version: 0.0.5a7
+Version: 0.0.6a1
 Summary: OVOS common play audio service adapter plugin
 Home-page: https://github.com/OpenVoiceOS/ovos-ocp-audio-plugin
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: ovos audio plugin
 Platform: UNKNOWN
```

### Comparing `ovos_plugin_common_play-0.0.5a7/ovos_plugin_common_play.egg-info/SOURCES.txt` & `ovos_plugin_common_play-0.0.6a1/ovos_plugin_common_play.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.5a7/setup.py` & `ovos_plugin_common_play-0.0.6a1/setup.py`

 * *Files identical despite different names*

