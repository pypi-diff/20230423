# Comparing `tmp/charidotella-0.7.tar.gz` & `tmp/charidotella-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charidotella-0.7.tar", last modified: Tue Apr  4 21:10:57 2023, max compression
+gzip compressed data, was "charidotella-0.8.tar", last modified: Sun Apr 23 18:53:36 2023, max compression
```

## Comparing `charidotella-0.7.tar` & `charidotella-0.8.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:10:57.197999 charidotella-0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-04 21:10:57.000000 charidotella-0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-04 21:10:57.197999 charidotella-0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-04 21:09:46.000000 charidotella-0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:10:57.185999 charidotella-0.7/charidotella/
--rw-r--r--   0 runner    (1001) docker     (123)    39536 2023-04-04 21:09:46.000000 charidotella-0.7/charidotella/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-04 21:09:46.000000 charidotella-0.7/charidotella/animals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:10:57.189999 charidotella-0.7/charidotella/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    18323 2023-04-04 21:09:46.000000 charidotella-0.7/charidotella/assets/configuration-schema.json
--rwxr-xr-x   0 runner    (1001) docker     (123)  1035600 2023-04-04 21:10:43.000000 charidotella-0.7/charidotella/assets/es_to_frames
--rwxr-xr-x   0 runner    (1001) docker     (123)   281936 2023-04-04 21:10:54.000000 charidotella-0.7/charidotella/assets/event_rate
--rwxr-xr-x   0 runner    (1001) docker     (123)    63800 2023-04-04 21:10:56.000000 charidotella-0.7/charidotella/assets/size
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-04 21:09:46.000000 charidotella-0.7/charidotella/charidotella_extension_placeholder.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:10:57.193999 charidotella-0.7/charidotella/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-04 21:09:46.000000 charidotella-0.7/charidotella/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-04 21:09:46.000000 charidotella-0.7/charidotella/filters/arbiter_saturation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-04 21:09:46.000000 charidotella-0.7/charidotella/filters/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-04 21:09:46.000000 charidotella-0.7/charidotella/filters/hot_pixels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-04 21:09:46.000000 charidotella-0.7/charidotella/filters/transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 21:09:46.000000 charidotella-0.7/charidotella/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:10:57.193999 charidotella-0.7/charidotella/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-04 21:09:46.000000 charidotella-0.7/charidotella/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-04 21:09:46.000000 charidotella-0.7/charidotella/tasks/colourtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-04 21:09:46.000000 charidotella-0.7/charidotella/tasks/event_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-04 21:09:46.000000 charidotella-0.7/charidotella/tasks/video.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-04 21:09:46.000000 charidotella-0.7/charidotella/tasks/wiggle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-04 21:09:46.000000 charidotella-0.7/charidotella/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-04 21:09:46.000000 charidotella-0.7/charidotella/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:10:57.189999 charidotella-0.7/charidotella.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-04 21:10:57.000000 charidotella-0.7/charidotella.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-04 21:10:57.000000 charidotella-0.7/charidotella.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 21:10:57.000000 charidotella-0.7/charidotella.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-04 21:10:57.000000 charidotella-0.7/charidotella.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-04 21:10:57.000000 charidotella-0.7/charidotella.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-04 21:10:57.000000 charidotella-0.7/charidotella.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:10:57.193999 charidotella-0.7/command_line_tools/
--rw-r--r--   0 runner    (1001) docker     (123)     9588 2023-04-04 21:09:47.000000 charidotella-0.7/command_line_tools/premake4.lua
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:10:57.197999 charidotella-0.7/command_line_tools/source/
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-04 21:09:47.000000 charidotella-0.7/command_line_tools/source/crop.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-04-04 21:09:47.000000 charidotella-0.7/command_line_tools/source/cut.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-04-04 21:09:47.000000 charidotella-0.7/command_line_tools/source/dat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-04 21:09:47.000000 charidotella-0.7/command_line_tools/source/dat_to_es.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-04-04 21:09:47.000000 charidotella-0.7/command_line_tools/source/es_to_csv.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    49088 2023-04-04 21:09:47.000000 charidotella-0.7/command_line_tools/source/es_to_frames.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-04-04 21:09:47.000000 charidotella-0.7/command_line_tools/source/es_to_ply.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    23197 2023-04-04 21:09:47.000000 charidotella-0.7/command_line_tools/source/event_rate.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-04-04 21:09:47.000000 charidotella-0.7/command_line_tools/source/evt3.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-04 21:09:47.000000 charidotella-0.7/command_line_tools/source/evt3_to_es.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-04 21:09:47.000000 charidotella-0.7/command_line_tools/source/font.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    22250 2023-04-04 21:09:47.000000 charidotella-0.7/command_line_tools/source/html.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9692 2023-04-04 21:09:47.000000 charidotella-0.7/command_line_tools/source/rainbow.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21863 2023-04-04 21:09:47.000000 charidotella-0.7/command_line_tools/source/rainmaker.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-04 21:09:47.000000 charidotella-0.7/command_line_tools/source/size.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-04-04 21:09:47.000000 charidotella-0.7/command_line_tools/source/statistics.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    18045 2023-04-04 21:09:47.000000 charidotella-0.7/command_line_tools/source/synth.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-04 21:09:47.000000 charidotella-0.7/command_line_tools/source/timecode.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:10:57.197999 charidotella-0.7/command_line_tools/third_party/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:10:57.181999 charidotella-0.7/command_line_tools/third_party/pontella/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:10:57.197999 charidotella-0.7/command_line_tools/third_party/pontella/source/
--rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-04-04 21:09:51.000000 charidotella-0.7/command_line_tools/third_party/pontella/source/pontella.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:10:57.181999 charidotella-0.7/command_line_tools/third_party/sepia/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:10:57.197999 charidotella-0.7/command_line_tools/third_party/sepia/source/
--rw-r--r--   0 runner    (1001) docker     (123)   104459 2023-04-04 21:09:53.000000 charidotella-0.7/command_line_tools/third_party/sepia/source/sepia.hpp
--rw-r--r--   0 runner    (1001) docker     (123)   213770 2023-04-04 21:09:47.000000 charidotella-0.7/command_line_tools/third_party/stb_truetype.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:10:57.181999 charidotella-0.7/command_line_tools/third_party/tarsier/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:10:57.197999 charidotella-0.7/command_line_tools/third_party/tarsier/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-04 21:09:57.000000 charidotella-0.7/command_line_tools/third_party/tarsier/source/replicate.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-04 21:09:57.000000 charidotella-0.7/command_line_tools/third_party/tarsier/source/stitch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    18323 2023-04-04 21:09:46.000000 charidotella-0.7/configuration-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-04 21:09:46.000000 charidotella-0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 21:10:57.197999 charidotella-0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-04-04 21:09:46.000000 charidotella-0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:53:36.595095 charidotella-0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-23 18:53:36.000000 charidotella-0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-23 18:53:36.595095 charidotella-0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-23 18:52:34.000000 charidotella-0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:53:36.583095 charidotella-0.8/charidotella/
+-rw-r--r--   0 runner    (1001) docker     (123)    40036 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/animals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:53:36.587095 charidotella-0.8/charidotella/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    18323 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/assets/configuration-schema.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1035600 2023-04-23 18:53:23.000000 charidotella-0.8/charidotella/assets/es_to_frames
+-rwxr-xr-x   0 runner    (1001) docker     (123)   281936 2023-04-23 18:53:33.000000 charidotella-0.8/charidotella/assets/event_rate
+-rwxr-xr-x   0 runner    (1001) docker     (123)    63800 2023-04-23 18:53:36.000000 charidotella-0.8/charidotella/assets/size
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/charidotella_extension_placeholder.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:53:36.587095 charidotella-0.8/charidotella/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/filters/arbiter_saturation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/filters/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/filters/hot_pixels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/filters/transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:53:36.587095 charidotella-0.8/charidotella/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/tasks/colourtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/tasks/event_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/tasks/video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/tasks/wiggle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 18:52:34.000000 charidotella-0.8/charidotella/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:53:36.583095 charidotella-0.8/charidotella.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-23 18:53:36.000000 charidotella-0.8/charidotella.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-23 18:53:36.000000 charidotella-0.8/charidotella.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:53:36.000000 charidotella-0.8/charidotella.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-23 18:53:36.000000 charidotella-0.8/charidotella.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-23 18:53:36.000000 charidotella-0.8/charidotella.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-23 18:53:36.000000 charidotella-0.8/charidotella.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:53:36.587095 charidotella-0.8/command_line_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     9588 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/premake4.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:53:36.591095 charidotella-0.8/command_line_tools/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/crop.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/cut.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/dat.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/dat_to_es.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/es_to_csv.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    49088 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/es_to_frames.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/es_to_ply.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23197 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/event_rate.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/evt3.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/evt3_to_es.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/font.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22250 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/html.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9692 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/rainbow.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21863 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/rainmaker.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/size.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/statistics.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18045 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/synth.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/source/timecode.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:53:36.595095 charidotella-0.8/command_line_tools/third_party/
+-rw-r--r--   0 runner    (1001) docker     (123)   730079 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/third_party/monaco.ttf.base64.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:53:36.579095 charidotella-0.8/command_line_tools/third_party/pontella/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:53:36.595095 charidotella-0.8/command_line_tools/third_party/pontella/source/
+-rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-04-23 18:52:40.000000 charidotella-0.8/command_line_tools/third_party/pontella/source/pontella.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:53:36.579095 charidotella-0.8/command_line_tools/third_party/sepia/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:53:36.595095 charidotella-0.8/command_line_tools/third_party/sepia/source/
+-rw-r--r--   0 runner    (1001) docker     (123)   104459 2023-04-23 18:52:42.000000 charidotella-0.8/command_line_tools/third_party/sepia/source/sepia.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)   213770 2023-04-23 18:52:35.000000 charidotella-0.8/command_line_tools/third_party/stb_truetype.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:53:36.579095 charidotella-0.8/command_line_tools/third_party/tarsier/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:53:36.595095 charidotella-0.8/command_line_tools/third_party/tarsier/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-23 18:52:47.000000 charidotella-0.8/command_line_tools/third_party/tarsier/source/replicate.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-23 18:52:47.000000 charidotella-0.8/command_line_tools/third_party/tarsier/source/stitch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18323 2023-04-23 18:52:34.000000 charidotella-0.8/configuration-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-23 18:52:34.000000 charidotella-0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 18:53:36.595095 charidotella-0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-23 18:52:34.000000 charidotella-0.8/setup.py
```

### Comparing `charidotella-0.7/PKG-INFO` & `charidotella-0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: charidotella
-Version: 0.7
+Version: 0.8
 Summary: Charidotella is a toolbox to organise and visualise Event Stream (.es) recordings
 Home-page: https://github.com/neuromorphicsystems/charidotella
 Author: Alexandre Marcireau
 Author-email: alexandre.marcireau@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 Charidotella (https://en.wikipedia.org/wiki/Charidotella_sexpunctata) is a toolbox to organise and visualise Event Stream (.es) recordings.
 
+It supports Python 3.9, 3.10, and 3.11.
+
 - [Dependencies](#dependencies)
 - [Get started](#get-started)
 - [Contribute](#contribute)
 
-
 ## Dependencies
 
 -   **Debian / Ubuntu**
 
     ```sh
     sudo apt install ffmpeg
     ```
@@ -59,30 +60,30 @@
         └── file_n.es
     ```
 
 3. Generate a configuration file
 
     ```sh
     cd my-wonderful-project
-    charidotella configure ./recordings
+    charidotella init 'recordings/*.es'
     ```
 
     The directory now has the following structure
 
     ```txt
     my-wonderful-project
     ├── recordings
     │   ├── file_1.es
     │   ├── file_2.es
     │   ├── ...
     │   └── file_n.es
     └── charidotella-configuration.toml
     ```
 
-4. (Optional) Edit `charidotella-coniguration.toml` to change the jobs' parameters
+4. (Optional) Edit `charidotella-configuration.toml` to change the jobs' parameters
 
 5. Run the jobs
 
     ```
     charidotella run
     ```
 
@@ -103,15 +104,15 @@
     │   │    └── rendered-file-m.es
     │   ├── adjective-animal-2
     │   ├── ...
     │   └── adjective-animal-n
     └── charidotella-configuration.toml
     ```
 
-6. (Optional) Edit `charidotella-coniguration.toml` and run `charidotella run` again (job that have already been completed will be skipped unless `--force` is used)
+6. (Optional) Edit `charidotella-configuration.toml` and run `charidotella run` again (job that have already been completed will be skipped unless `--force` is used)
 
 See `charidotella --help` for a list of other options.
 
 ## Contribute
 
 After code edits, run the formatters and linters.
```

### Comparing `charidotella-0.7/README.md` & `charidotella-0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Charidotella (https://en.wikipedia.org/wiki/Charidotella_sexpunctata) is a toolbox to organise and visualise Event Stream (.es) recordings.
 
+It supports Python 3.9, 3.10, and 3.11.
+
 - [Dependencies](#dependencies)
 - [Get started](#get-started)
 - [Contribute](#contribute)
 
-
 ## Dependencies
 
 -   **Debian / Ubuntu**
 
     ```sh
     sudo apt install ffmpeg
     ```
@@ -47,30 +48,30 @@
         └── file_n.es
     ```
 
 3. Generate a configuration file
 
     ```sh
     cd my-wonderful-project
-    charidotella configure ./recordings
+    charidotella init 'recordings/*.es'
     ```
 
     The directory now has the following structure
 
     ```txt
     my-wonderful-project
     ├── recordings
     │   ├── file_1.es
     │   ├── file_2.es
     │   ├── ...
     │   └── file_n.es
     └── charidotella-configuration.toml
     ```
 
-4. (Optional) Edit `charidotella-coniguration.toml` to change the jobs' parameters
+4. (Optional) Edit `charidotella-configuration.toml` to change the jobs' parameters
 
 5. Run the jobs
 
     ```
     charidotella run
     ```
 
@@ -91,15 +92,15 @@
     │   │    └── rendered-file-m.es
     │   ├── adjective-animal-2
     │   ├── ...
     │   └── adjective-animal-n
     └── charidotella-configuration.toml
     ```
 
-6. (Optional) Edit `charidotella-coniguration.toml` and run `charidotella run` again (job that have already been completed will be skipped unless `--force` is used)
+6. (Optional) Edit `charidotella-configuration.toml` and run `charidotella run` again (job that have already been completed will be skipped unless `--force` is used)
 
 See `charidotella --help` for a list of other options.
 
 ## Contribute
 
 After code edits, run the formatters and linters.
```

### Comparing `charidotella-0.7/charidotella/__init__.py` & `charidotella-0.8/charidotella/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,34 +63,32 @@
         description="Process Event Stream files",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     parser.add_argument(
         "--version", "-v", action="store_true", help="show the version and exit"
     )
     subparsers = parser.add_subparsers(dest="command")
-    configure_parser = subparsers.add_parser(
-        "configure", help="Generate a configuration file"
+    init_parser = subparsers.add_parser("init", help="Generate a configuration file")
+    init_parser.add_argument(
+        "glob",
+        help="Glob pattern used to search for Event Stream files",
     )
-    configure_parser.add_argument(
-        "directory",
-        help="Directory to scan (recursively) for Event Stream files",
-    )
-    configure_parser.add_argument(
+    init_parser.add_argument(
         "--configuration",
         "-c",
         default="charidotella-configuration.toml",
         help="Render configuration file path",
     )
-    configure_parser.add_argument(
+    init_parser.add_argument(
         "--force",
         "-f",
         action="store_true",
         help="Replace the configuration if it exists",
     )
-    configure_parser.add_argument(
+    init_parser.add_argument(
         "--preserve-names",
         "-p",
         action="store_true",
         help="Do not generate new names for the recordings",
     )
     run_parser = subparsers.add_parser("run", help="Process a configuration file")
     run_parser.add_argument(
@@ -146,15 +144,15 @@
                 if not isinstance(o[section], dict):
                     arrayoftables = False
                     if isinstance(o[section], list):
                         for a in o[section]:
                             if isinstance(a, dict):
                                 arrayoftables = True
                     if arrayoftables:
-                        for index, a in enumerate(o[section]):
+                        for a in o[section]:
                             arraytabstr = ""
                             arraystr += f"\n[[{sup}{qsection}]]\n"
                             s, d = self.dump_sections(a, sup + qsection)
                             if s:
                                 if s[0] == "[":
                                     arraytabstr += s
                                 else:
@@ -311,29 +309,30 @@
                             if generated_entry_name in configuration[key]:
                                 utilities.error(
                                     f"the {key} generator \"{generator['template']['name']}\" created an entry whose name (\"{generated_entry_name}\") already exists"
                                 )
                             configuration[key][generated_entry_name] = generated_entry
                 del configuration[generator_key]
 
-    if args.command == "configure":
+    if args.command == "init":
         configuration_path = pathlib.Path(args.configuration).resolve()
         if not args.force and configuration_path.is_file():
             utilities.error(
                 f'"{configuration_path}" already exists (use --force to override it)'
             )
-        directory = pathlib.Path(args.directory).resolve()
-        if not directory.is_dir():
-            utilities.error(f'"{directory}" does not exist or is not a directory')
-        paths = list(directory.rglob("*.es"))
+        paths = [
+            path.resolve()
+            for path in pathlib.Path(".").rglob(args.glob)
+            if path.is_file() and path.suffix == ".es"
+        ]
         paths.sort(key=lambda path: (path.stem, path.parent))
         if len(paths) == 0:
-            utilities.error(f'no .es files found in "{directory}"')
+            utilities.error(f'no .es files match "{args.glob}"')
         if args.preserve_names:
-            names = [path.stem for path in paths]
+            names = sorted([path.stem for path in paths])
             if len(names) != len(set(names)):
                 name_to_path: dict[str, pathlib.Path] = {}
                 for path in paths:
                     if path.stem in name_to_path:
                         utilities.error(
                             f'two files have the same name ("{name_to_path[path.stem]}" and "{path}"), rename one or do *not* use the flag --preserve-name'
                         )
@@ -343,15 +342,20 @@
         attachments: dict[str, list[dict[str, str]]] = {}
         for name, path in zip(names, paths):
             for sibling in path.parent.iterdir():
                 if sibling != path and sibling.stem == path.stem:
                     if not name in attachments:
                         attachments[name] = []
                     attachments[name].append(
-                        {"source": str(sibling), "target": f"{name}{sibling.suffix}"}
+                        {
+                            "source": str(
+                                sibling.relative_to(configuration_path.parent)
+                            ),
+                            "target": f"{name}{sibling.suffix}",
+                        }
                     )
         jobs = []
         for index, (name, path) in enumerate(zip(names, paths)):
             utilities.info(
                 animals.composite_name_to_icon(name),
                 f'{index + 1}/{len(paths)} reading range for {utilities.format_bold(name)} ("{path}")',
             )
@@ -429,15 +433,15 @@
                                 "ratio": "@raw(ratio)",
                             },
                         },
                         {
                             "parameters": {
                                 "suffix": [
                                     "flip-left-right",
-                                    "flip-top_bottom",
+                                    "flip-top-bottom",
                                     "rotate-90",
                                     "rotate-180",
                                     "rotate-270",
                                     "transpose",
                                     "transverse",
                                 ],
                                 "method": [
@@ -447,15 +451,15 @@
                                     "rotate_180",
                                     "rotate_270",
                                     "transpose",
                                     "transverse",
                                 ],
                             },
                             "template": {
-                                "name": "transpose-@suffix",
+                                "name": "@suffix",
                                 "type": "transpose",
                                 "icon": "📐",
                                 "suffix": "@suffix",
                                 "method": "@method",
                             },
                         },
                     ]
@@ -620,15 +624,20 @@
                         encoder=Encoder(),
                     ).split("\n")
                     if len(line) > 0
                 )
             )
             configuration_file.write("\n\n\n# generated name to source file\n")
             toml.dump(
-                {"sources": {name: str(path) for name, path in zip(names, paths)}},
+                {
+                    "sources": {
+                        name: str(path.relative_to(configuration_path.parent))
+                        for name, path in zip(names, paths)
+                    }
+                },
                 configuration_file,
                 encoder=Encoder(),
             )
             configuration_file.write(
                 "\n\n# attachments are copied in target directories, algonside generated files \n"
             )
             toml.dump(
@@ -768,23 +777,24 @@
                     if (
                         not args.force
                         and attachment["target"] in parameters["attachments"]
                         and (directory / name / attachment["target"]).is_file()
                     ):
                         utilities.info(
                             "⏭ ",
-                            f"skip copy {attachment['source']} → {attachment['target']}",
+                            f"skip copy {pathlib.Path(configuration_path.parent) / attachment['source']} → {attachment['target']}",
                         )
                     else:
                         utilities.info(
                             "🗃 ",
-                            f"copy {attachment['source']} → {attachment['target']}",
+                            f"copy {pathlib.Path(configuration_path.parent) / attachment['source']} → {attachment['target']}",
                         )
                         shutil.copy2(
-                            pathlib.Path(attachment["source"]),
+                            pathlib.Path(configuration_path.parent)
+                            / attachment["source"],
                             utilities.with_suffix(
                                 directory / name / attachment["target"], ".part"
                             ),
                         )
                         utilities.with_suffix(
                             directory / name / attachment["target"], ".part"
                         ).rename(directory / name / attachment["target"])
@@ -802,15 +812,16 @@
                     )
                     and output_path.is_file()
                 ):
                     utilities.info("⏭ ", f"skip filter {filter_name}")
                 else:
                     utilities.info(filter["icon"], f"apply filter {filter_name}")
                     FILTERS[filter["type"]](
-                        pathlib.Path(configuration["sources"][job["name"]]),
+                        pathlib.Path(configuration_path.parent)
+                        / configuration["sources"][job["name"]],
                         utilities.with_suffix(output_path, ".part"),
                         begin,
                         end,
                         filter["parameters"],
                     )
                     utilities.with_suffix(output_path, ".part").rename(output_path)
                     parameters["filters"][filter_name] = filter["parameters"]
@@ -832,15 +843,18 @@
                 ):
                     utilities.info("⏭ ", f"skip filters {' + '.join(job['filters'])}")
                 else:
                     with tempfile.TemporaryDirectory(
                         suffix=job["name"]
                     ) as temporary_directory_name:
                         temporary_directory = pathlib.Path(temporary_directory_name)
-                        input = pathlib.Path(configuration["sources"][job["name"]])
+                        input = (
+                            pathlib.Path(configuration_path.parent)
+                            / configuration["sources"][job["name"]]
+                        )
                         for index, filter_name in enumerate(job["filters"]):
                             if index == len(job["filters"]) - 1:
                                 output = utilities.with_suffix(output_path, ".part")
                             else:
                                 output = temporary_directory / f"{uuid.uuid4()}.es"
                             filter = configuration["filters"][filter_name]
                             utilities.info(
```

### Comparing `charidotella-0.7/charidotella/animals.py` & `charidotella-0.8/charidotella/animals.py`

 * *Files 5% similar despite different names*

```diff
@@ -113,13 +113,13 @@
     config["subj"]["lists"] = ["animal"]
     generator = coolname.RandomGenerator(config)
     coolname_length = 4
     for length in (2, 3):
         if count < generator.get_combinations_count(length) / 2:
             coolname_length = length
             break
-    names = []
-    while len(set(names)) < count:
-        while len(names) < count:
-            names.append(generator.generate_slug(coolname_length))
+    names_set: set[str] = set()
+    while len(names_set) < count:
+        names_set.add(generator.generate_slug(coolname_length))
+    names = list(names_set)
     names.sort()
     return names
```

### Comparing `charidotella-0.7/charidotella/assets/configuration-schema.json` & `charidotella-0.8/charidotella/assets/configuration-schema.json`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/charidotella/assets/es_to_frames` & `charidotella-0.8/charidotella/assets/es_to_frames`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/charidotella/assets/event_rate` & `charidotella-0.8/charidotella/assets/event_rate`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/charidotella/assets/size` & `charidotella-0.8/charidotella/assets/size`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/charidotella/charidotella_extension_placeholder.c` & `charidotella-0.8/charidotella/charidotella_extension_placeholder.c`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/charidotella/filters/arbiter_saturation.py` & `charidotella-0.8/charidotella/filters/arbiter_saturation.py`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/charidotella/filters/default.py` & `charidotella-0.8/charidotella/filters/default.py`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/charidotella/filters/hot_pixels.py` & `charidotella-0.8/charidotella/filters/hot_pixels.py`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/charidotella/filters/transpose.py` & `charidotella-0.8/charidotella/filters/transpose.py`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/charidotella/tasks/colourtime.py` & `charidotella-0.8/charidotella/tasks/colourtime.py`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/charidotella/tasks/event_rate.py` & `charidotella-0.8/charidotella/tasks/event_rate.py`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/charidotella/tasks/video.py` & `charidotella-0.8/charidotella/tasks/video.py`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/charidotella/tasks/wiggle.py` & `charidotella-0.8/charidotella/tasks/wiggle.py`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/charidotella/utilities.py` & `charidotella-0.8/charidotella/utilities.py`

 * *Files 14% similar despite different names*

```diff
@@ -44,17 +44,17 @@
     timestamp -= hours * 60 * 60 * 1000000
     minutes = timestamp // (60 * 1000000)
     timestamp -= minutes * 60 * 1000000
     seconds = timestamp // 1000000
     timestamp -= seconds * 1000000
     timestamp_string = "" if timestamp == 0 else f".{timestamp:06d}".rstrip("0")
     if hours > 0:
-        return f"{hours}:{minutes:02d}:{seconds:02d}{timestamp_string}"
+        return f"{hours}-{minutes:02d}-{seconds:02d}{timestamp_string}"
     if minutes > 0:
-        return f"{minutes}:{seconds:02d}{timestamp_string}"
+        return f"{minutes}-{seconds:02d}{timestamp_string}"
     return f"{seconds}{timestamp_string}"
 
 
 def timecode(value: str) -> int:
     if value.isdigit():
         return int(value)
     match = TIMECODE_PATTERN.match(value)
```

### Comparing `charidotella-0.7/charidotella.egg-info/PKG-INFO` & `charidotella-0.8/charidotella.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: charidotella
-Version: 0.7
+Version: 0.8
 Summary: Charidotella is a toolbox to organise and visualise Event Stream (.es) recordings
 Home-page: https://github.com/neuromorphicsystems/charidotella
 Author: Alexandre Marcireau
 Author-email: alexandre.marcireau@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 Charidotella (https://en.wikipedia.org/wiki/Charidotella_sexpunctata) is a toolbox to organise and visualise Event Stream (.es) recordings.
 
+It supports Python 3.9, 3.10, and 3.11.
+
 - [Dependencies](#dependencies)
 - [Get started](#get-started)
 - [Contribute](#contribute)
 
-
 ## Dependencies
 
 -   **Debian / Ubuntu**
 
     ```sh
     sudo apt install ffmpeg
     ```
@@ -59,30 +60,30 @@
         └── file_n.es
     ```
 
 3. Generate a configuration file
 
     ```sh
     cd my-wonderful-project
-    charidotella configure ./recordings
+    charidotella init 'recordings/*.es'
     ```
 
     The directory now has the following structure
 
     ```txt
     my-wonderful-project
     ├── recordings
     │   ├── file_1.es
     │   ├── file_2.es
     │   ├── ...
     │   └── file_n.es
     └── charidotella-configuration.toml
     ```
 
-4. (Optional) Edit `charidotella-coniguration.toml` to change the jobs' parameters
+4. (Optional) Edit `charidotella-configuration.toml` to change the jobs' parameters
 
 5. Run the jobs
 
     ```
     charidotella run
     ```
 
@@ -103,15 +104,15 @@
     │   │    └── rendered-file-m.es
     │   ├── adjective-animal-2
     │   ├── ...
     │   └── adjective-animal-n
     └── charidotella-configuration.toml
     ```
 
-6. (Optional) Edit `charidotella-coniguration.toml` and run `charidotella run` again (job that have already been completed will be skipped unless `--force` is used)
+6. (Optional) Edit `charidotella-configuration.toml` and run `charidotella run` again (job that have already been completed will be skipped unless `--force` is used)
 
 See `charidotella --help` for a list of other options.
 
 ## Contribute
 
 After code edits, run the formatters and linters.
```

### Comparing `charidotella-0.7/charidotella.egg-info/SOURCES.txt` & `charidotella-0.8/charidotella.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -44,12 +44,13 @@
 command_line_tools/source/html.hpp
 command_line_tools/source/rainbow.cpp
 command_line_tools/source/rainmaker.cpp
 command_line_tools/source/size.cpp
 command_line_tools/source/statistics.cpp
 command_line_tools/source/synth.cpp
 command_line_tools/source/timecode.hpp
+command_line_tools/third_party/monaco.ttf.base64.hpp
 command_line_tools/third_party/stb_truetype.hpp
 command_line_tools/third_party/pontella/source/pontella.hpp
 command_line_tools/third_party/sepia/source/sepia.hpp
 command_line_tools/third_party/tarsier/source/replicate.hpp
 command_line_tools/third_party/tarsier/source/stitch.hpp
```

### Comparing `charidotella-0.7/command_line_tools/premake4.lua` & `charidotella-0.8/command_line_tools/premake4.lua`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/command_line_tools/source/crop.cpp` & `charidotella-0.8/command_line_tools/source/crop.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/command_line_tools/source/cut.cpp` & `charidotella-0.8/command_line_tools/source/cut.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/command_line_tools/source/dat.hpp` & `charidotella-0.8/command_line_tools/source/dat.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/command_line_tools/source/dat_to_es.cpp` & `charidotella-0.8/command_line_tools/source/dat_to_es.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/command_line_tools/source/es_to_csv.cpp` & `charidotella-0.8/command_line_tools/source/es_to_csv.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/command_line_tools/source/es_to_frames.cpp` & `charidotella-0.8/command_line_tools/source/es_to_frames.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/command_line_tools/source/es_to_ply.cpp` & `charidotella-0.8/command_line_tools/source/es_to_ply.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/command_line_tools/source/event_rate.cpp` & `charidotella-0.8/command_line_tools/source/event_rate.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/command_line_tools/source/evt3.hpp` & `charidotella-0.8/command_line_tools/source/evt3.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/command_line_tools/source/evt3_to_es.cpp` & `charidotella-0.8/command_line_tools/source/evt3_to_es.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/command_line_tools/source/font.hpp` & `charidotella-0.8/command_line_tools/source/font.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/command_line_tools/source/html.hpp` & `charidotella-0.8/command_line_tools/source/html.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/command_line_tools/source/rainbow.cpp` & `charidotella-0.8/command_line_tools/source/rainbow.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/command_line_tools/source/rainmaker.cpp` & `charidotella-0.8/command_line_tools/source/rainmaker.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/command_line_tools/source/size.cpp` & `charidotella-0.8/command_line_tools/source/size.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/command_line_tools/source/statistics.cpp` & `charidotella-0.8/command_line_tools/source/statistics.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/command_line_tools/source/synth.cpp` & `charidotella-0.8/command_line_tools/source/synth.cpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/command_line_tools/source/timecode.hpp` & `charidotella-0.8/command_line_tools/source/timecode.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/command_line_tools/third_party/pontella/source/pontella.hpp` & `charidotella-0.8/command_line_tools/third_party/pontella/source/pontella.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/command_line_tools/third_party/sepia/source/sepia.hpp` & `charidotella-0.8/command_line_tools/third_party/sepia/source/sepia.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/command_line_tools/third_party/stb_truetype.hpp` & `charidotella-0.8/command_line_tools/third_party/stb_truetype.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/command_line_tools/third_party/tarsier/source/replicate.hpp` & `charidotella-0.8/command_line_tools/third_party/tarsier/source/replicate.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/command_line_tools/third_party/tarsier/source/stitch.hpp` & `charidotella-0.8/command_line_tools/third_party/tarsier/source/stitch.hpp`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/configuration-schema.json` & `charidotella-0.8/configuration-schema.json`

 * *Files identical despite different names*

### Comparing `charidotella-0.7/setup.py` & `charidotella-0.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         "include command_line_tools/source/*.cpp",
         "include command_line_tools/premake4.lua",
         "include command_line_tools/third_party/pontella/source/pontella.hpp",
         "include command_line_tools/third_party/sepia/source/sepia.hpp",
         "include command_line_tools/third_party/tarsier/source/replicate.hpp",
         "include command_line_tools/third_party/tarsier/source/stitch.hpp",
         "include command_line_tools/third_party/stb_truetype.hpp",
+        "include command_line_tools/third_party/monaco.ttf.base64.hpp",
     ]
     if "sdist" in sys.argv:
         manifest_lines.append(f"include configuration-schema.json")
     else:
         shutil.rmtree(dirname / "charidotella" / "assets", ignore_errors=True)
         (dirname / "charidotella" / "assets").mkdir()
         if sys.platform == "win32":
@@ -80,18 +81,19 @@
             dirname / "charidotella" / "assets" / "configuration-schema.json",
         )
         manifest_lines.append(f"include charidotella/assets/configuration-schema.json")
     with open("MANIFEST.in", "w") as manifest:
         content = "\n".join(manifest_lines)
         manifest.write(f"{content}\n")
 
+exec(open(dirname / "charidotella" / "version.py").read())
 
 setuptools.setup(
     name="charidotella",
-    version="0.7",
+    version=__version__, # type: ignore
     url="https://github.com/neuromorphicsystems/charidotella",
     author="Alexandre Marcireau",
     author_email="alexandre.marcireau@gmail.com",
     description="Charidotella is a toolbox to organise and visualise Event Stream (.es) recordings",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
```

