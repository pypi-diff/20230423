# Comparing `tmp/batogram-1.0.5.tar.gz` & `tmp/batogram-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batogram-1.0.5.tar", last modified: Sat Apr  8 15:21:15 2023, max compression
+gzip compressed data, was "batogram-1.0.6.tar", last modified: Sun Apr 23 19:36:38 2023, max compression
```

## Comparing `batogram-1.0.5.tar` & `batogram-1.0.6.tar`

### file list

```diff
@@ -1,62 +1,83 @@
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-04-08 15:21:15.533095 batogram-1.0.5/
--rw-r--r--   0 jmears    (1000) jmears    (1000)     1053 2023-04-02 15:18:25.000000 batogram-1.0.5/LICENSE
--rw-r--r--   0 jmears    (1000) jmears    (1000)       98 2023-04-06 17:26:29.000000 batogram-1.0.5/MANIFEST.in
--rw-r--r--   0 jmears    (1000) jmears    (1000)     6018 2023-04-08 15:21:15.533095 batogram-1.0.5/PKG-INFO
--rw-r--r--   0 jmears    (1000) jmears    (1000)     4070 2023-04-07 16:33:09.000000 batogram-1.0.5/README.md
--rw-r--r--   0 jmears    (1000) jmears    (1000)     1435 2023-04-08 15:19:50.000000 batogram-1.0.5/pyproject.toml
--rw-r--r--   0 jmears    (1000) jmears    (1000)       38 2023-04-08 15:21:15.533095 batogram-1.0.5/setup.cfg
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-04-08 15:21:15.525095 batogram-1.0.5/src/
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-04-08 15:21:15.531095 batogram-1.0.5/src/batogram/
--rw-r--r--   0 jmears    (1000) jmears    (1000)      232 2022-12-31 16:28:12.000000 batogram-1.0.5/src/batogram/3669170_home_ic_icon.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      191 2023-04-08 15:20:15.000000 batogram-1.0.5/src/batogram/__init__.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)      535 2023-04-08 15:03:35.000000 batogram-1.0.5/src/batogram/__main__.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2467 2023-04-07 16:59:42.000000 batogram-1.0.5/src/batogram/about.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     4634 2023-04-05 20:25:50.000000 batogram-1.0.5/src/batogram/amplitudegraphframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)      407 2023-01-08 21:24:32.000000 batogram-1.0.5/src/batogram/arrow-left-circle-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      230 2022-12-31 16:57:23.000000 batogram-1.0.5/src/batogram/arrow-left-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      425 2023-01-15 18:28:59.000000 batogram-1.0.5/src/batogram/arrow-right-circle-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      224 2022-12-31 16:57:23.000000 batogram-1.0.5/src/batogram/arrow-right-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)     7482 2023-04-05 20:07:25.000000 batogram-1.0.5/src/batogram/audiofileservice.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     1373 2023-04-01 16:47:47.000000 batogram-1.0.5/src/batogram/batogram.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)     3159 2023-04-05 20:07:26.000000 batogram-1.0.5/src/batogram/breadcrumbservice.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     7235 2023-04-05 20:07:25.000000 batogram-1.0.5/src/batogram/buttonframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     5245 2023-04-02 15:49:35.000000 batogram-1.0.5/src/batogram/chunky_spectrogram.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2729 2023-04-02 15:51:19.000000 batogram-1.0.5/src/batogram/colourmap.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     1605 2023-04-02 15:20:15.000000 batogram-1.0.5/src/batogram/common.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     1724 2023-04-08 14:16:31.000000 batogram-1.0.5/src/batogram/constants.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)      263 2023-01-08 21:11:46.000000 batogram-1.0.5/src/batogram/download-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      362 2022-12-31 17:04:27.000000 batogram-1.0.5/src/batogram/drag-move-2-line.png
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-04-08 15:21:15.533095 batogram-1.0.5/src/batogram/external/
--rw-r--r--   0 jmears    (1000) jmears    (1000)        0 2023-04-03 13:24:39.000000 batogram-1.0.5/src/batogram/external/__init__.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    19291 2023-02-25 21:12:13.000000 batogram-1.0.5/src/batogram/external/guano.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     4666 2023-04-02 15:28:51.000000 batogram-1.0.5/src/batogram/external/tooltip.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2063 2023-04-05 20:07:26.000000 batogram-1.0.5/src/batogram/fileinfoframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2638 2023-04-05 20:25:41.000000 batogram-1.0.5/src/batogram/frames.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     5374 2023-04-05 20:25:33.000000 batogram-1.0.5/src/batogram/graphsettings.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2096 2023-04-02 15:58:14.000000 batogram-1.0.5/src/batogram/historianservice.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)      337 2022-12-31 16:54:39.000000 batogram-1.0.5/src/batogram/home-4-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)     7310 2022-12-12 15:11:55.000000 batogram-1.0.5/src/batogram/kindlmann-table-byte-0256.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)    29566 2023-01-07 15:05:04.000000 batogram-1.0.5/src/batogram/kindlmann-table-byte-1024.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)    25798 2023-04-07 19:57:49.000000 batogram-1.0.5/src/batogram/layouts.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    28625 2023-04-08 14:17:45.000000 batogram-1.0.5/src/batogram/morebncframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    12392 2023-04-05 20:26:08.000000 batogram-1.0.5/src/batogram/moreframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     5140 2023-04-05 20:32:37.000000 batogram-1.0.5/src/batogram/morerenderingframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     5680 2023-04-05 20:07:25.000000 batogram-1.0.5/src/batogram/morescaleframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     4405 2023-04-05 20:25:58.000000 batogram-1.0.5/src/batogram/profilegraphframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     3518 2023-04-05 20:07:26.000000 batogram-1.0.5/src/batogram/readoutframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    55914 2023-04-08 14:13:13.000000 batogram-1.0.5/src/batogram/rendering.py
--rwxr-xr-x   0 jmears    (1000) jmears    (1000)    30405 2023-04-08 15:09:34.000000 batogram-1.0.5/src/batogram/rootwindow.py
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-04-08 15:21:15.533095 batogram-1.0.5/src/batogram/samples/
--rw-r--r--   0 jmears    (1000) jmears    (1000)        0 2023-04-06 17:24:57.000000 batogram-1.0.5/src/batogram/samples/__init__.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    18364 2023-04-08 14:34:34.000000 batogram-1.0.5/src/batogram/spectrogramgraphframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    12370 2023-04-08 14:27:03.000000 batogram-1.0.5/src/batogram/spectrogrammouseservice.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    17001 2023-04-02 15:21:16.000000 batogram-1.0.5/src/batogram/validatingwidgets.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    13433 2023-04-03 14:02:00.000000 batogram-1.0.5/src/batogram/wavfileparser.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)      452 2022-12-31 17:04:35.000000 batogram-1.0.5/src/batogram/zoom-in-line.png
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-04-08 15:21:15.532095 batogram-1.0.5/src/batogram.egg-info/
--rw-r--r--   0 jmears    (1000) jmears    (1000)     6018 2023-04-08 15:21:15.000000 batogram-1.0.5/src/batogram.egg-info/PKG-INFO
--rw-r--r--   0 jmears    (1000) jmears    (1000)     1647 2023-04-08 15:21:15.000000 batogram-1.0.5/src/batogram.egg-info/SOURCES.txt
--rw-r--r--   0 jmears    (1000) jmears    (1000)        1 2023-04-08 15:21:15.000000 batogram-1.0.5/src/batogram.egg-info/dependency_links.txt
--rw-r--r--   0 jmears    (1000) jmears    (1000)       51 2023-04-08 15:21:15.000000 batogram-1.0.5/src/batogram.egg-info/entry_points.txt
--rw-r--r--   0 jmears    (1000) jmears    (1000)       36 2023-04-08 15:21:15.000000 batogram-1.0.5/src/batogram.egg-info/requires.txt
--rw-r--r--   0 jmears    (1000) jmears    (1000)        9 2023-04-08 15:21:15.000000 batogram-1.0.5/src/batogram.egg-info/top_level.txt
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-04-23 19:36:38.649627 batogram-1.0.6/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     1053 2023-04-22 20:32:02.000000 batogram-1.0.6/LICENSE
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      118 2023-04-21 19:32:05.000000 batogram-1.0.6/MANIFEST.in
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     6317 2023-04-23 19:36:38.648627 batogram-1.0.6/PKG-INFO
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     4369 2023-04-23 19:35:13.000000 batogram-1.0.6/README.md
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-04-23 19:36:38.572626 batogram-1.0.6/batogram/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      310 2023-04-23 19:25:54.000000 batogram-1.0.6/batogram/__init__.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      535 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/__main__.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2189 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/about.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     4634 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/amplitudegraphframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2599 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/appsettings.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     5255 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/appsettingsmodal.py
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-04-23 19:36:38.580626 batogram-1.0.6/batogram/assets/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      232 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/assets/3669170_home_ic_icon.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      407 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/assets/arrow-left-circle-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      230 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/assets/arrow-left-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      425 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/assets/arrow-right-circle-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      224 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/assets/arrow-right-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     1373 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/assets/batogram.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      263 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/assets/download-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      362 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/assets/drag-move-2-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      222 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/assets/expand-left-right-fill.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      214 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/assets/expand-up-down-fill.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      337 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/assets/home-4-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      452 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/assets/zoom-in-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     7482 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/audiofileservice.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     3159 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/breadcrumbservice.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     7257 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/buttonframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     5245 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/chunky_spectrogram.py
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-04-23 19:36:38.631627 batogram-1.0.6/batogram/colour_maps/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2727 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/colour_maps/CET-L01.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2280 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/colour_maps/CET-L03.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2343 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/colour_maps/CET-L05.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2618 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/colour_maps/CET-L06.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2679 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/colour_maps/CET-L07.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2726 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/colour_maps/CET-L08.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2663 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/colour_maps/CET-L09.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2612 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/colour_maps/CET-L16.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2933 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/colour_maps/CET-L17.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2857 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/colour_maps/CET-L18.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2961 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/colour_maps/CET-L19.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2705 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/colour_maps/CET-L20.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    30096 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/colour_maps/black-body-table-byte-1024.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    29916 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/colour_maps/extended-kindlmann-table-byte-1024.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    30107 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/colour_maps/inferno-table-byte-1024.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    29566 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/colour_maps/kindlmann-table-byte-1024.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     3593 2023-04-22 20:37:59.000000 batogram-1.0.6/batogram/colourmap.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     1605 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/common.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     1762 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/constants.py
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-04-23 19:36:38.636627 batogram-1.0.6/batogram/external/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)        0 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/external/__init__.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    19291 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/external/guano.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     4666 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/external/tooltip.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2063 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/fileinfoframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2638 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/frames.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     5298 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/graphsettings.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2096 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/historianservice.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    27810 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/layouts.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     1244 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/modalwindow.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    28314 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/morebncframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    12392 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/moreframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     5140 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/morerenderingframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     6055 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/morescaleframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     4486 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/profilegraphframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     3518 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/readoutframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    56511 2023-04-22 19:51:11.000000 batogram-1.0.6/batogram/rendering.py
+-rwxr-xr-x   0 jmears    (1000) jmears    (1000)    34753 2023-04-22 19:51:11.000000 batogram-1.0.6/batogram/rootwindow.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      493 2023-04-22 20:48:37.000000 batogram-1.0.6/batogram/runner.py
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-04-23 19:36:38.647627 batogram-1.0.6/batogram/samples/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)        0 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/samples/__init__.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    19066 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/spectrogramgraphframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    15524 2023-04-23 18:49:49.000000 batogram-1.0.6/batogram/spectrogrammouseservice.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    17001 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/validatingwidgets.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    13433 2023-04-22 20:32:02.000000 batogram-1.0.6/batogram/wavfileparser.py
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-04-23 19:36:38.578626 batogram-1.0.6/batogram.egg-info/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     6317 2023-04-23 19:36:38.000000 batogram-1.0.6/batogram.egg-info/PKG-INFO
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2226 2023-04-23 19:36:38.000000 batogram-1.0.6/batogram.egg-info/SOURCES.txt
+-rw-r--r--   0 jmears    (1000) jmears    (1000)        1 2023-04-23 19:36:38.000000 batogram-1.0.6/batogram.egg-info/dependency_links.txt
+-rw-r--r--   0 jmears    (1000) jmears    (1000)       49 2023-04-23 19:36:38.000000 batogram-1.0.6/batogram.egg-info/entry_points.txt
+-rw-r--r--   0 jmears    (1000) jmears    (1000)       58 2023-04-23 19:36:38.000000 batogram-1.0.6/batogram.egg-info/requires.txt
+-rw-r--r--   0 jmears    (1000) jmears    (1000)        9 2023-04-23 19:36:38.000000 batogram-1.0.6/batogram.egg-info/top_level.txt
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     1467 2023-04-23 19:26:27.000000 batogram-1.0.6/pyproject.toml
+-rw-r--r--   0 jmears    (1000) jmears    (1000)       38 2023-04-23 19:36:38.649627 batogram-1.0.6/setup.cfg
```

### Comparing `batogram-1.0.5/LICENSE` & `batogram-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `batogram-1.0.5/PKG-INFO` & `batogram-1.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batogram
-Version: 1.0.5
+Version: 1.0.6
 Summary: Batogram is a GUI program for rendering spectrograms from full spectrum recordings of bat calls.
 Author-email: John Mears <john+batogram@themears.co.uk>
 License: Copyright (c) 2023 John Mears
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -33,29 +33,47 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 batogram
 ========
 
-Batogram is an open source application for viewing bat calls spectrograms.
+Batogram is an open source application for viewing bat call spectrograms.
 
 Some capabilities and features: 
 * Rendering of spectrograms from .wav files.
 * Auto selection of many parameters for simple operation.
 * Efficient rendering with graceful handling of larger data files.
-* Pan and scale using the mouse or by manual selection.
+* Pan and scale using the mouse, keys or by manual selection.
 * Handling of multichannel data files, including stereo.
 * Basic side by side comparison of two spectrograms.
 * Display of GUANO metadata, including the ability to click to open the location in Google Maps.
-* Runs on Windows, macOS and Linux operating systems.
+* Runs on Windows, Linux and macOS (experimental) operating systems.
 
 Installation
 ------------
 
+### Windows
+
+There are currently two approaches to installing Batogram on Windows. The first and simplest
+method is as follows:
+
+* Download a Batogram executable for Windows from Github. Available releases are listed 
+[here](https://github.com/jmears63/batogram/releases).
+* Probably Windows Defender will warn you of the danger of downloading such files from unknown
+sources. Assess the risk and decide if you going ahead. Assuming you are, proceed to the
+next step.
+* Copy the downloaded executable to your Windows desktop, so that you can find it when you want it.
+* Double click it on the desktop to run it. The first time you run it, it will take a little longer to start 
+up than usual. You will notice a command window launched alongside Batogram - ignore it. This is to
+aid debugging, and will be removed in a future release.
+
+The second installation method is to install Python on your Windows computer, and then follow the 
+same steps as the Linux installation. If you take this route, I assume you know what you are doing.
+
 ### Linux
 
 On Linux, Batogram is currently installed from the command line using pip, as below.
 You need to have Python 3.10 as a minimum.  
 
     # Create a virtual environment at a convenient location in your home directory:
     mkdir ~/batogram
@@ -63,46 +81,24 @@
     python3 -m venv venv
     source venv/bin/activate
 
     # It's good practice to have pip up to date:
     pip install pip --upgrade
 
     # Install batogram and its dependencies. This may take a few moments.
-    # Obviously, substitute the lastest and greatest version number:
-    pip install batogram-x.y.z.tar.gz
+    pip install batogram
     
     # Batogram is now in PATH. You can run it with this simple command:
     batogram
 
-### Windows
-For now, Batogram is installed onto windows using the following slightly convoluted
-steps. At some point in the future, I will provide a simpler install.
-
-This sequence assumes Windows 11.
-
-* Launch the Microsoft Store. You can do this from the Start menu - search for Microsoft Store,
-and launch it.
-* In the store, search for Python using the upper right menu. Select a version which is
-at least 3.10 - probably, the most recent version. I used version 3.11.
-* Go ahead and install it.
-* Open a windows command prompt - for example, by searching for cmd from the start menu. 
-
-In the command prompt, enter this command to install Batogram and its dependencies, which
-may take a few moments:
-
-    pip install batogram
-
-The install command will finish by displaying a path to batogram.exe. You may wish to copy
-that file to your desktop for convenient launching. Otherwise, you can launch
-Batogram from the command prompt:
-
-    python -m batogram
+### macOS (experimental)
 
-Subsequently you can launch Batogram using that command in the command prompt, or by double
-clicking on batogram.exe on your desktop, if you copied it there in the previous step.
+It should be possible to follow the same steps as the Linux installation to install and run
+batogram. However, I am not an expert on Apple products, and don't have any macOS systems to
+test this on.
 
 Usage
 -----
 
 Refer to files in the docs directory for more information. In particular, see
 [batogram.md](docs/batogram.md) for usage notes.
 
@@ -123,19 +119,21 @@
 For the moment, while the structure of the code is fairly rapid flux, so I am not accepting
 pull requests other than for small fixes. This may change in the future.
 
 Credits
 -------
 
 In no particular order:
-* [Pictogrammers Team](https://www.iconarchive.com/show/material-icons-by-pictogrammers/bat-icon.html)
-* [Tucker Beck](https://code.activestate.com/recipes/576688-tooltip-for-tkinter/)
-* [Remix Icon](https://remixicon.com/)
-* [Kenneth Moreland](https://www.kennethmoreland.com/color-advice/)
-* [David A. Riggs](https://github.com/riggsd/guano-py/blob/master/guano.py)
+* [Pictogrammers Team](https://www.iconarchive.com/show/material-icons-by-pictogrammers/bat-icon.html) for the application icon.
+* [Tucker Beck](https://code.activestate.com/recipes/576688-tooltip-for-tkinter/) for tooltip code.
+* [Remix Icon](https://remixicon.com/) for icons.
+* [Kenneth Moreland](https://www.kennethmoreland.com/color-advice/) for colour maps.
+* [David A. Riggs](https://github.com/riggsd/guano-py/blob/master/guano.py) for GUANO code.
+* [Arnold Andreasson](https://github.com/arnoldandreasson) for testing and insights.
+* [Peter Kovesi](https://colorcet.com/index.html) for colour maps.
 
 About the Author
 ----------------
 
 I am John Mears. I obtained a degree in physics in the University of Oxford
 in the distant past. I have spent much of the last 40 years writing software
 relating to scientific and email seccurity applications. In my spare time I cycle,
```

### Comparing `batogram-1.0.5/README.md` & `batogram-1.0.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,43 @@
 batogram
 ========
 
-Batogram is an open source application for viewing bat calls spectrograms.
+Batogram is an open source application for viewing bat call spectrograms.
 
 Some capabilities and features: 
 * Rendering of spectrograms from .wav files.
 * Auto selection of many parameters for simple operation.
 * Efficient rendering with graceful handling of larger data files.
-* Pan and scale using the mouse or by manual selection.
+* Pan and scale using the mouse, keys or by manual selection.
 * Handling of multichannel data files, including stereo.
 * Basic side by side comparison of two spectrograms.
 * Display of GUANO metadata, including the ability to click to open the location in Google Maps.
-* Runs on Windows, macOS and Linux operating systems.
+* Runs on Windows, Linux and macOS (experimental) operating systems.
 
 Installation
 ------------
 
+### Windows
+
+There are currently two approaches to installing Batogram on Windows. The first and simplest
+method is as follows:
+
+* Download a Batogram executable for Windows from Github. Available releases are listed 
+[here](https://github.com/jmears63/batogram/releases).
+* Probably Windows Defender will warn you of the danger of downloading such files from unknown
+sources. Assess the risk and decide if you going ahead. Assuming you are, proceed to the
+next step.
+* Copy the downloaded executable to your Windows desktop, so that you can find it when you want it.
+* Double click it on the desktop to run it. The first time you run it, it will take a little longer to start 
+up than usual. You will notice a command window launched alongside Batogram - ignore it. This is to
+aid debugging, and will be removed in a future release.
+
+The second installation method is to install Python on your Windows computer, and then follow the 
+same steps as the Linux installation. If you take this route, I assume you know what you are doing.
+
 ### Linux
 
 On Linux, Batogram is currently installed from the command line using pip, as below.
 You need to have Python 3.10 as a minimum.  
 
     # Create a virtual environment at a convenient location in your home directory:
     mkdir ~/batogram
@@ -27,46 +45,24 @@
     python3 -m venv venv
     source venv/bin/activate
 
     # It's good practice to have pip up to date:
     pip install pip --upgrade
 
     # Install batogram and its dependencies. This may take a few moments.
-    # Obviously, substitute the lastest and greatest version number:
-    pip install batogram-x.y.z.tar.gz
+    pip install batogram
     
     # Batogram is now in PATH. You can run it with this simple command:
     batogram
 
-### Windows
-For now, Batogram is installed onto windows using the following slightly convoluted
-steps. At some point in the future, I will provide a simpler install.
-
-This sequence assumes Windows 11.
-
-* Launch the Microsoft Store. You can do this from the Start menu - search for Microsoft Store,
-and launch it.
-* In the store, search for Python using the upper right menu. Select a version which is
-at least 3.10 - probably, the most recent version. I used version 3.11.
-* Go ahead and install it.
-* Open a windows command prompt - for example, by searching for cmd from the start menu. 
-
-In the command prompt, enter this command to install Batogram and its dependencies, which
-may take a few moments:
-
-    pip install batogram
-
-The install command will finish by displaying a path to batogram.exe. You may wish to copy
-that file to your desktop for convenient launching. Otherwise, you can launch
-Batogram from the command prompt:
-
-    python -m batogram
+### macOS (experimental)
 
-Subsequently you can launch Batogram using that command in the command prompt, or by double
-clicking on batogram.exe on your desktop, if you copied it there in the previous step.
+It should be possible to follow the same steps as the Linux installation to install and run
+batogram. However, I am not an expert on Apple products, and don't have any macOS systems to
+test this on.
 
 Usage
 -----
 
 Refer to files in the docs directory for more information. In particular, see
 [batogram.md](docs/batogram.md) for usage notes.
 
@@ -87,19 +83,21 @@
 For the moment, while the structure of the code is fairly rapid flux, so I am not accepting
 pull requests other than for small fixes. This may change in the future.
 
 Credits
 -------
 
 In no particular order:
-* [Pictogrammers Team](https://www.iconarchive.com/show/material-icons-by-pictogrammers/bat-icon.html)
-* [Tucker Beck](https://code.activestate.com/recipes/576688-tooltip-for-tkinter/)
-* [Remix Icon](https://remixicon.com/)
-* [Kenneth Moreland](https://www.kennethmoreland.com/color-advice/)
-* [David A. Riggs](https://github.com/riggsd/guano-py/blob/master/guano.py)
+* [Pictogrammers Team](https://www.iconarchive.com/show/material-icons-by-pictogrammers/bat-icon.html) for the application icon.
+* [Tucker Beck](https://code.activestate.com/recipes/576688-tooltip-for-tkinter/) for tooltip code.
+* [Remix Icon](https://remixicon.com/) for icons.
+* [Kenneth Moreland](https://www.kennethmoreland.com/color-advice/) for colour maps.
+* [David A. Riggs](https://github.com/riggsd/guano-py/blob/master/guano.py) for GUANO code.
+* [Arnold Andreasson](https://github.com/arnoldandreasson) for testing and insights.
+* [Peter Kovesi](https://colorcet.com/index.html) for colour maps.
 
 About the Author
 ----------------
 
 I am John Mears. I obtained a degree in physics in the University of Oxford
 in the distant past. I have spent much of the last 40 years writing software
 relating to scientific and email seccurity applications. In my spare time I cycle,
```

### Comparing `batogram-1.0.5/pyproject.toml` & `batogram-1.0.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "batogram"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
     {name = "John Mears", email = "john+batogram@themears.co.uk"},
 ]
 description = "Batogram is a GUI program for rendering spectrograms from full spectrum recordings of bat calls."
 readme = "README.md"
 requires-python = ">=3.10"      # To support | with type hints.
 keywords = ["bat", "spectrogram", "chiropterology", "fourier", "ultrasonic", "ultrasound", "echo", "GUANO"]
@@ -20,32 +20,33 @@
     'Intended Audience :: Science/Research',
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     'Topic :: Multimedia :: Sound/Audio :: Analysis',
 ]
 dependencies = [
-    "pathlib",
     "numpy",
     "scipy",
     "Pillow",
-    "argparse"
+    "argparse",
+    "dataclasses-json",
+    "platformdirs"
 ]
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
-where = ["src"]
+where = ["."]
+include = ["batogram*"]
 
 [tool.setuptools.package-data]
 # For some reason these file types also need to be listed in MANIFEST.in
-# "*" = ["*.png", "*.csv", "*.wav"]
-"*" = ["*.png", "*.csv"]
+"*" = ["assets/*.png", "colour_maps/*.csv"]
 
 [project.scripts]
 # Automatically create a command to run the program. There is an alternative to run a GUI script,
 # with no terminal window.
-batogram = "batogram.__main__:run"
+batogram = "batogram.runner:run"
 
 [project.urls]
 "Homepage" = "https://github.com/jmears63/batogram"
```

### Comparing `batogram-1.0.5/src/batogram/__main__.py` & `batogram-1.0.6/batogram/__main__.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.5/src/batogram/about.py` & `batogram-1.0.6/batogram/frames.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,45 +13,56 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+
 import tkinter as tk
+import tkinter.messagebox
 
-from PIL import ImageTk, Image
-from . import get_asset_path, __version__
+from .constants import PROGRAM_NAME
 
 
-class AboutWindow(tk.Toplevel):
-    def __init__(self, parent):
-        super().__init__(parent)
-        self.title("About Batogram")
-        self.transient()  # Doesn't seem to do anything.
-        self.attributes('-topmost', 'true')  # Keep in front of its parent.
-
-        ref = parent
-        width, height = 300, 300
-        self.geometry("{}x{}+{}+{}".format(
-            width, height,
-            ref.winfo_rootx() + (ref.winfo_width() - width) // 2,
-            ref.winfo_rooty() + (ref.winfo_height() - height) // 2))
-
-        pad = 5
-
-        # We must assign the image to a member variable to prevent the GC getting rid of it
-        # too soon:
-        self._img = ImageTk.PhotoImage(Image.open(get_asset_path("batogram.png")))
-        label = tk.Label(self, image=self._img)
-        label.grid(row=0, column=0, padx=pad, pady=pad)
-
-        label = tk.Label(self, text="Version: {}".format(__version__))
-        label.grid(row=1, column=0, padx=pad, pady=pad)
+class DrawableFrame(tk.Frame):
+    """All frames within a pane are of this type, to allow them to be drawn in the same way."""
+
+    # Flags to pass to the notification methods to limit which graphs will be refreshed:
+    DRAW_SPECTROGRAM = 1
+    DRAW_PROFILE = 2
+    DRAW_AMPLITUDE = 4
+    DRAW_ALL = DRAW_SPECTROGRAM | DRAW_PROFILE | DRAW_AMPLITUDE
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
-        label = tk.Label(self, text="Author: John Mears")
-        label.grid(row=2, column=0, padx=pad, pady=pad)
+    def draw(self, draw_scope: int = DRAW_ALL):
+        pass  # Subclasses may do drawing here, if they want.
 
-        btn = tk.Button(self, text="Close", command=self.destroy)
-        btn.grid(row=3, column=0, padx=pad, pady=pad)
+    def reset_draw(self, draw_scope: int = DRAW_ALL):
+        pass  # Subclasses may use this hint to abandon any pending drawing.
 
-        self.columnconfigure(0, weight=1)   # Expand to use the width.
+
+class GraphFrame(DrawableFrame):
+    """All frames containing graph data are of this type."""
+
+    def __init__(self, parent, root, pipeline, data_context, settings: "GraphSettings"):
+        super().__init__(parent)
+        self._completer = None
+        self._my_root = root
+        self._pipeline = pipeline
+        self._dc = data_context
+        self._settings: "GraphSettings" = settings
+        self._layout = None
+
+    def _on_canvas_change(self, _):
+        self.draw()
+
+    @staticmethod
+    def _pipeline_error_handler(e):
+        tk.messagebox.showerror(PROGRAM_NAME, "Error encountered in processing pipeline: {}".format(e))
+        raise e
+
+    def reset_draw(self, draw_scope: int = DrawableFrame.DRAW_ALL):
+        super().reset_draw()
+        self._completer = None
```

### Comparing `batogram-1.0.5/src/batogram/amplitudegraphframe.py` & `batogram-1.0.6/batogram/amplitudegraphframe.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.5/src/batogram/audiofileservice.py` & `batogram-1.0.6/batogram/audiofileservice.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.5/src/batogram/batogram.png` & `batogram-1.0.6/batogram/assets/batogram.png`

 * *Files identical despite different names*

### Comparing `batogram-1.0.5/src/batogram/breadcrumbservice.py` & `batogram-1.0.6/batogram/breadcrumbservice.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.5/src/batogram/buttonframe.py` & `batogram-1.0.6/batogram/buttonframe.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,22 +87,22 @@
         ToolTip(self._next_button, msg="Reinstate the subsequent zoom")
         col += 1
 
         self._zoom_image = self._load_image("zoom-in-line.png")
         self._zoom_button = MyButton(self, self._zoom_image,
                                      command=lambda: self._handle_cursor_mode(CursorMode.CURSOR_ZOOM))
         self._zoom_button.grid(row=0, column=col, padx=(10, 0), ipadx=0, sticky="NSEW")
-        ToolTip(self._zoom_button, msg="Select zoom cursor mode\nHold shift to lock the frequency span")
+        ToolTip(self._zoom_button, msg="Select zoom cursor: left mouse drag to zoom.\nHold shift to lock mode.")
         col += 1
 
         self._pan_image = self._load_image("drag-move-2-line.png")
         self._pan_button = MyButton(self, self._pan_image,
                                     command=lambda: self._handle_cursor_mode(CursorMode.CURSOR_PAN))
         self._pan_button.grid(row=0, column=col, padx=0, ipadx=0, sticky="NSEW")
-        ToolTip(self._pan_button, msg="Select pan cursor mode\nHold shift to lock the frequency span")
+        ToolTip(self._pan_button, msg="Select pan cursor: left mouse drag to pan/scroll.\nHold shift to lock mode.")
         col += 1
 
         spacer = tk.Label(self)
         spacer.grid(row=0, column=col)
         spacer2_index = col
         col += 1
```

### Comparing `batogram-1.0.5/src/batogram/chunky_spectrogram.py` & `batogram-1.0.6/batogram/chunky_spectrogram.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.5/src/batogram/colourmap.py` & `batogram-1.0.6/batogram/colourmap.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,38 +15,54 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import numpy as np
-import pathlib as pl
+
+from . import get_colour_map_path
+from .appsettings import COLOUR_MAPS, DEFAULT_COLOUR_MAP
 
 
 class ColourMap:
     """The colour map is used to render spectrograms in the UI."""
 
-    def __init__(self):
+    def __init__(self, map_file: str):
+        """
+        Don't use this to create instances, instead access
+        the single shared instance using get_instance().
+        """
+
         self._cmap = None
         self._num_steps: int | None = None
+        self._polyfilla_colour: str | None = None
+
+        self.reload_map(map_file)
 
-    def load_map(self, colour_mapping_path: pl.Path):
-        """Read a colour map from a CSV with four columns like this:
-            0.0,0,0,0
-            0.0009775171065493646,1,0,1
-            ...
-            0.9990224828934506,255,255,255
-            1.0,255,255,255
+    def reload_map(self, map_file: str):
+        """
+            Read a colour map from a CSV with thee or four columns. The last three columns
+            are RGB byte values.
+            NB remove the initial row of column headers from files, if present.
         """
 
-        raw_cmap = np.genfromtxt(colour_mapping_path, delimiter=',', dtype=np.uint8)  # Rows are: value, R, G, B
-        # The first column is not required, the remaining 3 are RGB:
-        self._cmap = np.delete(raw_cmap, 0, axis=1)
+        colour_mapping_path = get_colour_map_path(map_file)
+        raw_cmap: np.ndarray = np.genfromtxt(colour_mapping_path, delimiter=',', dtype=np.uint8)
+
+        # Some formats have the value in the first column, which is not required:
+        if raw_cmap.shape[1] == 4:
+            raw_cmap = np.delete(raw_cmap, 0, axis=1)
+        self._cmap = raw_cmap
         self._num_steps = len(self._cmap)
 
+        # Calculate the "lowest" colour as a string:
+        entry = self._cmap[0]
+        self._polyfilla_colour = "#{:02X}{:02X}{:02X}".format(*entry)
+
     def map(self, inputdata: np.ndarray) -> np.ndarray:
         """Replace each value in the input with an (RGB) tuple.
         The input data values must be in the range 0-1."""
 
         # Create a new array for the output data, the same shape as the input data:
         outputdata = np.zeros((*inputdata.shape, 3), dtype=np.uint8)  # Allow for RGB layers.
         # Do the mapping: each value in inputdata is replaced with an RGB from
@@ -55,7 +71,15 @@
         # ‘clip’ mode means that all indices that are too large are replaced by the index that addresses the last
         # element along that axis. Note that this disables indexing with negative numbers.
 
         inputdata = (inputdata * self._num_steps).astype(int)
         np.take(self._cmap, inputdata, axis=0, mode='clip', out=outputdata)
 
         return outputdata
+
+    def get_polyfilla_colour(self) -> str:
+        """Get the 'lowest' colour of the spectrum to be used for filling awkward gaps."""
+        return self._polyfilla_colour
+
+
+# The single global instance of the colour map:
+instance: ColourMap = ColourMap(COLOUR_MAPS[DEFAULT_COLOUR_MAP])
```

### Comparing `batogram-1.0.5/src/batogram/common.py` & `batogram-1.0.6/batogram/common.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.5/src/batogram/constants.py` & `batogram-1.0.6/batogram/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,12 +22,13 @@
 DATA_CHANGE_MAIN_EVENT = "<<OnDataChangeMain>>"  # Underlying data has change: for example, a file opened or closed.
 DATA_CHANGE_REF_EVENT = "<<OnDataChangeRef>>"  # Underlying data has change: for example, a file opened or closed.
 MAIN_SPECTROGAM_COMPLETER_EVENT = "<<MainSpectrogramCompleter>>"
 MAIN_AMPLITUDE_COMPLETER_EVENT = "<<MainAmplitudeCompleter>>"
 MAIN_PROFILE_COMPLETER_EVENT = "<<MainProfileCompleter>>"
 FONT_SIZE = 12
 ZOOM_ORDER = 2  # This will move into settings. 0-2 is a useful range.
-ASSETS_PATH = "."
+COLOUR_MAPS_PATH = "colour_maps"
+ASSETS_PATH = "assets"
 
 # Limit how far they can zoom in:
 MIN_F_RANGE: float = 500
 MIN_T_RANGE: float = 0.001
```

### Comparing `batogram-1.0.5/src/batogram/external/guano.py` & `batogram-1.0.6/batogram/external/guano.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.5/src/batogram/external/tooltip.py` & `batogram-1.0.6/batogram/external/tooltip.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.5/src/batogram/fileinfoframe.py` & `batogram-1.0.6/batogram/fileinfoframe.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.5/src/batogram/graphsettings.py` & `batogram-1.0.6/batogram/graphsettings.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from dataclasses import dataclass
 from typing import Optional, NoReturn, Callable
+
+from .appsettings import DEFAULT_COLOUR_MAP, COLOUR_MAPS
 from .common import AxisRange
 from .frames import DrawableFrame
 
 borderwidth = 10
 
 SUPPORTED_FFT_SAMPLES = [64, 128, 256, 512, 1024, 2048, 4096, 8192]
 DEFAULT_FFT_SAMPLES_INDEX = 3
@@ -40,16 +42,16 @@
 
 ADAPTIVE_FFT_OVERLAP_PERCENT = -1
 FFT_OVERLAP_PERCENT_OPTIONS = {
     ADAPTIVE_FFT_OVERLAP_PERCENT: "Auto",
     0: "0", 25: "25", 50: "50", 75: "75", 90: "90", 95: "95"}
 DEFAULT_FFT_OVERLAP_PERCENT = ADAPTIVE_FFT_OVERLAP_PERCENT
 
-INTERPOLATION_OPTIONS = {0: "None", 1: "Linear", 2: "Quadratic"}
-DEFAULT_INTERPOLATION = 1       # Linear is fairly smooth and fairly fast,
+INTERPOLATION_OPTIONS = {0: "None", 1: "Linear", 2: "Quadratic", 3: "Cubic"}
+DEFAULT_INTERPOLATION = 2       # Linear is fairly smooth and fairly fast,
                                 # and avoids edge artifacts that quadratic generates.
 
 # Note: boxcar window blows up in the calculations involving infinity
 WINDOW_TYPE_OPTIONS = {"hann": "Hann", "hamming": "Hamming", "blackman": "Blackman", "tukey": "Tukey 0.5",
                        "bartlett": "Bartlett", "flattop": "Flat top"}
 DEFAULT_WINDOW_TYPE = "hann"
 
@@ -59,14 +61,15 @@
 BNC_MODES = {BNC_ADAPTIVE_MODE: "Auto", BNC_MANUAL_MODE: "Manual", BNC_INTERACTIVE_MODE: "Interactive"}
 
 
 @dataclass
 class GraphSettings:
     """Settings relating to a specific graph panel."""
     time_range: Optional[AxisRange]
+    zero_based_time: bool
     frequency_range: Optional[AxisRange]
     show_grid: bool
     show_profile: bool
     fft_samples: int
     fft_overlap: int
     window_type: str
     zoom_interpolation: int
@@ -79,26 +82,24 @@
     bnc_manual_max: float
 
     def __init__(self,
                  on_app_modified_settings: Callable[[int], NoReturn],
                  on_user_applied_settings: Callable[[int], NoReturn],
                  show_profile=True):
         self.time_range = AxisRange(0, 1)
+        self.zero_based_time = True
         self.frequency_range = AxisRange(0, 1)
         self._on_app_modified_settings: Callable[[int], NoReturn] = on_app_modified_settings  # Call this to signal that the UI needs to refresh.
         self._on_user_applied_settings: Callable[[int], NoReturn] = on_user_applied_settings  # Call this to signal that the application needs to refresh.
         self.show_grid = True
         self.show_profile = show_profile
         self.fft_samples = DEFAULT_FFT_SAMPLES
         self.fft_overlap = DEFAULT_FFT_OVERLAP_PERCENT
         self.window_type = DEFAULT_WINDOW_TYPE
         self.zoom_interpolation = DEFAULT_INTERPOLATION
-        # The colour mapping we are going to use. See https://www.kennethmoreland.com/color-advice.
-        self.colour_mapping_path = "kindlmann-table-byte-1024.csv"
-        self.colour_mapping_steps = 1024
         self.do_histogram_normalization = False
         self.bnc_adjust_type = BNC_ADAPTIVE_MODE
         self.bnc_background_threshold_percent = 80.0
         self.bnc_manual_min, self.bnc_manual_max = 0.0, 1.0
 
     def on_app_modified_settings(self, draw_scope: int = DrawableFrame.DRAW_ALL) -> NoReturn:
         """Signal to the settings UI that the underlying settings values have changed."""
```

### Comparing `batogram-1.0.5/src/batogram/historianservice.py` & `batogram-1.0.6/batogram/historianservice.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.5/src/batogram/kindlmann-table-byte-1024.csv` & `batogram-1.0.6/batogram/colour_maps/kindlmann-table-byte-1024.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.5/src/batogram/layouts.py` & `batogram-1.0.6/batogram/layouts.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,19 +15,24 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import math
+import sys
 import tkinter as tk
+from dataclasses import dataclass
+
 import numpy as np
 
-from typing import Optional, Tuple
+from typing import Optional, Tuple, List
 from PIL import ImageTk, Image, ImageOps
+
+from . import colourmap
 from .common import AxisRange
 
 AXIS_BG_COLOUR = "#404040"
 AXIS_FG_COLOUR = "white"
 GRID_COLOUR = "#404040"
 
 
@@ -136,26 +141,25 @@
         (1) The axes etc., which are fast to draw, are drawn immediately by this method
         (2) The image and things overlaying it (such as the grid) are drawn later when the image
             has been calculated. A capture is returned that the caller can use later to do this.
         """
 
         self._data_ranges = x_range, y_range
 
-    def rect_to_values(self, pixel_rect, frequency_clamped: bool) -> Tuple[float, float, float, float] | None:
+    def rect_to_values(self, pixel_rect) \
+            -> Tuple[float, float, float, float] | None:
         """Scale the pixel rectangle supplied to real axis values."""
 
         l, t, r, b = pixel_rect
         if self._x_axis and self._y_axis:
+            # if clamp:
             vl = self._x_axis.canvas_to_axis(l)
             vr = self._x_axis.canvas_to_axis(r)
-            if frequency_clamped:
-                vb, vt = self._y_axis.get_axis_range().get_tuple()
-            else:
-                vt = self._y_axis.canvas_to_axis(t)
-                vb = self._y_axis.canvas_to_axis(b)
+            vt = self._y_axis.canvas_to_axis(t)
+            vb = self._y_axis.canvas_to_axis(b)
             return vl, vt, vr, vb
         else:
             return None
 
     def canvas_to_axis(self, p_canvas):
         """Scale the pixel position relative to the canvas origin to real axis values."""
 
@@ -167,14 +171,23 @@
             return t_axis, f_axis
         else:
             return None
 
     @staticmethod
     def _draw_graph_image(canvas, data_area, image):
         (il, it, ir, ib) = data_area
+
+        # There may be a right margin to fill, if we are zoomed right out:
+        image_height, image_width, _ = image.shape
+        data_area_width: int = ir - il
+        if image_width < data_area_width:
+            delta = data_area_width - image_width
+            fill_colour: str = colourmap.instance.get_polyfilla_colour()
+            canvas.create_rectangle(ir - delta, it, ir, it + image_height - 1, fill=fill_colour, outline=fill_colour)
+
         inverted_image = Image.fromarray(np.uint8(image)).convert('RGB')
         pil_image = ImageOps.flip(inverted_image)
         image = ImageTk.PhotoImage(pil_image)
         canvas.my_image = image  # Hack to protect the image against garbage collection
         # (see https://web.archive.org/web/20201111190625id_/http://effbot.org/pyfaq/why-do-my-tkinter-images-not-appear.htm)
         canvas.create_image(il, it, image=image, anchor='nw')
 
@@ -213,31 +226,40 @@
         l, t, r, b = data_area
         for v, p in y_ticks:
             if p > 0:  # Don't overwrite the axes.
                 y_pixels = b - p + 1  # The first y-axis tick is actually over the xaxis
                 canvas.create_line(l, y_pixels, r, y_pixels, fill=GRID_COLOUR, width=1, dash=(1, 1))
 
 
+@dataclass
+class AxisUnit:
+    limit: float = sys.float_info.max  # Upper limit for this unit, or sys.float_info.max if it is the default.
+    units: str = ""  # The unit.
+    scaler: float = 1.0  # Multiples the tick vakues.
+
+
 class AxisLayout(Layout):
     """This class knows how to lay out and draw a graph axis."""
 
     ORIENT_VERTICAL = 1
     ORIENT_HORIZONTAL = 2
 
-    def __init__(self, orientation: object, font_height: object, title: object, canvas_width: object,
-                 canvas_height: object, hide_text: object = False):
+    def __init__(self, orientation: int, font_height: int, title: str, canvas_width: int,
+                 canvas_height: int, units: List[AxisUnit], hide_text: bool = False):
         super().__init__(font_height, canvas_width, canvas_height)
         self._orientation = orientation
         self._title = title
         self._hide_text = hide_text
         self._font_name = "helvetica"
         self._layout()
         self._min_pixel = None
         self._max_pixel = None
         self._axis_range: Optional[AxisRange] = None
+        self._units: List[AxisUnit] = sorted(units, key=lambda u: u.limit)  # Ascending.
+        self._units_to_use: AxisUnit | None = None
 
     def _layout(self):
         # These coordinates increase from 0 on the outside to maximum
         # next to the data area.
 
         unit = self._font_height  # Everything is relative to font size.
         half_unit = int(unit / 2 + 0.5)  # Avoid floating point.
@@ -256,35 +278,43 @@
         self._tick_start = self._tick_end + half_unit
         self._axis_offset = self._tick_start + 1
         self._size = self._axis_offset
 
     def get_size(self):
         return self._size
 
-    def draw(self, canvas, x, y, extent, axis_range: AxisRange, multiplier=1, target_spacing_pixels=100):
-        # One day we could make this more abstract by having a Tk flavoured derived
-        # class or by passing in a drawing context of our own devising. Will that day ever come?
-
+    def draw(self, canvas, x, y, extent, axis_range: AxisRange, zero_based_axis: bool, target_spacing_pixels=100):
         # Note: create_rectangle doesn't include the bottom/right edges, so we have to +1.
 
         self._axis_range = axis_range
 
-        (ticks, decimal_places) = self.calculate_ticks(self._axis_range, multiplier, extent,
+        if zero_based_axis:
+            # Offset the time ticks so that they always start at zero:
+            offset_axis_range = AxisRange(0, self._axis_range.max - self._axis_range.min)
+        else:
+            offset_axis_range = self._axis_range
+
+        # Decide what units to use based on the axis range:
+        u = self._get_units(offset_axis_range)
+
+        (ticks, decimal_places) = self.calculate_ticks(offset_axis_range, u.scaler, extent,
                                                        target_spacing_pixels=target_spacing_pixels)
 
         # Negative font height is in pixels:
         axis_font = (self._font_name, -self._font_height)
 
+        text: str = "{} ({})".format(self._title, u.units)
+
         if self._orientation == self.ORIENT_VERTICAL:
             Layout._create_rectangle(canvas, x, y, self._size - 1, y + extent, AXIS_BG_COLOUR)
             # Line seems to need a +1 to reach the final pixel:
             canvas.create_line([(x + self._axis_offset - 1, y), (x + self._axis_offset - 1, y + extent + 1)],
                                fill=AXIS_FG_COLOUR, width=1)
             if not self._hide_text:
-                canvas.create_text(x + self._title_start, x + extent / 2, text=self._title, fill=AXIS_FG_COLOUR,
+                canvas.create_text(x + self._title_start, x + extent / 2, text=text, fill=AXIS_FG_COLOUR,
                                    angle=90, font=axis_font, anchor=tk.N)
             for v, p in ticks:
                 canvas.create_line(x + self._tick_end, y + extent - p, x + self._tick_start, y + extent - p,
                                    fill=AXIS_FG_COLOUR, width=1)
                 if not self._hide_text:
                     canvas.create_text(x + self._scale_start, y + extent - p,
                                        text="{0:.{dps}f}".format(float(v), dps=decimal_places), angle=90,
@@ -293,15 +323,15 @@
             self._max_pixel = y
 
         if self._orientation == self.ORIENT_HORIZONTAL:
             Layout._create_rectangle(canvas, x, y, x + extent, y + self._size - 1, AXIS_BG_COLOUR)
             # Line seems to need a +1 to reach the final pixel:
             canvas.create_line([(x, y), (x + extent + 1, y)], fill=AXIS_FG_COLOUR, width=1)
             if not self._hide_text:
-                canvas.create_text(x + extent / 2, y + self._size - self._title_end, text=self._title,
+                canvas.create_text(x + extent / 2, y + self._size - self._title_end, text=text,
                                    fill=AXIS_FG_COLOUR,
                                    font=axis_font, anchor=tk.N)
             for t, p in ticks:
                 canvas.create_line(x + p, y + self._size - self._tick_end, x + p, y + self._size - self._tick_start,
                                    fill=AXIS_FG_COLOUR, width=1)
                 if not self._hide_text:
                     canvas.create_text(x + p, y + self._size - self._scale_end,
@@ -310,45 +340,62 @@
             self._min_pixel = x  # Pixel that corresponds to the minimum axis value
             self._max_pixel = x + extent
 
         return ticks
 
     def canvas_to_axis(self, p):
         v = (p - self._min_pixel) / (self._max_pixel - self._min_pixel) * (
-                    self._axis_range.max - self._axis_range.min) + self._axis_range.min
+                self._axis_range.max - self._axis_range.min) + self._axis_range.min
         return v
 
     def get_axis_range(self) -> AxisRange:
         return self._axis_range
 
+    def _get_units(self, axis_range) -> AxisUnit:
+        """Decide what units to use based on the axis range."""
+
+        if len(self._units) == 1:
+            return self._units[0]
+        else:
+            abs_max: float = max(abs(axis_range.min), abs(axis_range.max))
+            # The possible units are already sorted in ascending order.
+            for u in self._units:
+                if abs_max < u.limit:
+                    return u
+            return u
+
 
 class SpectrogramLayout(GraphLayout):
     """This Layout knows how to lay out and raw a spectrogram."""
 
+    _x_axis_unit = [AxisUnit(scaler=1.0, units="s"),  # Default
+                    AxisUnit(limit=0.5, scaler=1E-3, units="ms")
+                    ]
+    _y_axis_unit = [AxisUnit(scaler=1000.0, units="kHz")]
+
     def __init__(self, font_height, canvas_width, canvas_height):
         super().__init__(font_height, canvas_width, canvas_height)
-        self._x_axis = AxisLayout(AxisLayout.ORIENT_HORIZONTAL, font_height, "time (s)", canvas_width,
-                                  canvas_height)
-        self._y_axis = AxisLayout(AxisLayout.ORIENT_VERTICAL, font_height, "frequency (kHz)", canvas_width,
-                                  canvas_height,
-                                  hide_text=False)
+        self._x_axis = AxisLayout(AxisLayout.ORIENT_HORIZONTAL, font_height, "time", canvas_width,
+                                  canvas_height, self._x_axis_unit)
+        self._y_axis = AxisLayout(AxisLayout.ORIENT_VERTICAL, font_height, "frequency", canvas_width,
+                                  canvas_height, self._y_axis_unit, hide_text=False)
         self._layout()
 
     def _layout(self):
         self._x_axis_height = self._x_axis.get_size()
         self._y_axis_width = self._y_axis.get_size()
 
         # Calculate some *inclusive* zero based rectangle coords:
         self._data_area = (
             self._y_axis_width, self._margin, self._canvas_width - self._margin - 1,
             self._canvas_height - self._x_axis_height - 1)
         self._dead_space = (
             0, self._canvas_height - self._x_axis_height, self._y_axis_width - 1, self._canvas_height - 1)
 
-    def draw(self, canvas, x_range: AxisRange, y_range: AxisRange, show_grid):
+    def draw(self, canvas, x_range: AxisRange, y_range: AxisRange, show_grid, zero_based_x_axis: bool):
         super().draw(canvas, x_range, y_range, show_grid)
 
         """Draw a graph including axes, image and grid. We do this in two phases:
         (1) The axes etc, which are fast to draw, are drawn immediately by this method
         (2) The image and things overlaying it (such as the grid) are drawn later when the image
             has been calculated. A capture is returned that the caller can use later to do this.
         """
@@ -363,20 +410,20 @@
         Layout._create_rectangle(canvas, t, l, r, b, AXIS_BG_COLOUR)
 
         Layout._create_rectangle(canvas, *self._get_right_margin(), AXIS_BG_COLOUR)
         Layout._create_rectangle(canvas, *self._get_top_margin(), AXIS_BG_COLOUR)
 
         # Draw the axes:
         (yaxis_x, yaxis_y, yaxis_extent) = (0, self._margin, self._canvas_height - self._x_axis_height - self._margin)
-        y_ticks = self._y_axis.draw(canvas, yaxis_x, yaxis_y, yaxis_extent, y_range, multiplier=1000)
+        y_ticks = self._y_axis.draw(canvas, yaxis_x, yaxis_y, yaxis_extent, y_range, zero_based_axis=False)
 
         (xaxis_x, xaxis_y, xaxis_extent) = (
             self._y_axis_width - 1, self._canvas_height - self._x_axis.get_size(),
             self._canvas_width - self._y_axis_width - self._margin)
-        x_ticks = self._x_axis.draw(canvas, xaxis_x, xaxis_y, xaxis_extent, x_range)
+        x_ticks = self._x_axis.draw(canvas, xaxis_x, xaxis_y, xaxis_extent, x_range, zero_based_axis=zero_based_x_axis)
 
         # Create a capture that can be used to finish drawing the graph later on, when the image
         # is available:
         def draw_completer(is_memory_limit_hit: bool = False, image=None):
             # width, height = canvas.winfo_width(), canvas.winfo_height()
 
             if is_memory_limit_hit:
@@ -408,23 +455,24 @@
         else:
             return None
 
 
 class AmplitudeLayout(GraphLayout):
     """This Layout knows how to lay out and raw an amplitude graph."""
 
+    _x_axis_unit = [AxisUnit()]
+    _y_axis_unit = [AxisUnit()]
+
     def __init__(self, font_height, canvas_width, canvas_height, is_reference=False):
         super().__init__(font_height, canvas_width, canvas_height)
         self._is_reference = is_reference
-        self._x_axis = AxisLayout(AxisLayout.ORIENT_HORIZONTAL, font_height, "time (s)", canvas_width,
-                                  canvas_height)
+        self._x_axis = AxisLayout(AxisLayout.ORIENT_HORIZONTAL, font_height, "time", canvas_width,
+                                  canvas_height, units=self._x_axis_unit)
         self._y_axis = AxisLayout(AxisLayout.ORIENT_VERTICAL, font_height, "amplitude", canvas_width,
-                                  canvas_height,
-                                  # hide_text=is_reference,
-                                  hide_text=False)
+                                  canvas_height, units=self._y_axis_unit, hide_text=False)
         self._layout()
 
     def _layout(self):
         self._x_axis_height = self._x_axis.get_size()
         self._y_axis_width = self._y_axis.get_size()
 
         # Calculate some *inclusive* zero based rectangle coords:
@@ -475,34 +523,37 @@
 
         return draw_followup, self._data_area
 
 
 class ProfileLayout(GraphLayout):
     """This Layout knows how to lay out and raw a profile graph."""
 
+    _x_axis_unit = [AxisUnit()]
+    _y_axis_unit = [AxisUnit()]
+
     def __init__(self, font_height, canvas_width, canvas_height):
         super().__init__(font_height, canvas_width, canvas_height)
         self._x_axis = AxisLayout(AxisLayout.ORIENT_HORIZONTAL, font_height, "dB", canvas_width,
-                                  canvas_height)
+                                  canvas_height, units=self._x_axis_unit)
         self._y_axis = AxisLayout(AxisLayout.ORIENT_VERTICAL, font_height, "frequency (kHz)", canvas_width,
-                                  canvas_height, hide_text=True)
+                                  canvas_height, units=self._y_axis_unit, hide_text=True)
         self._layout()
 
     def _layout(self):
         self._x_axis_height = self._x_axis.get_size()
         self._y_axis_width = self._y_axis.get_size()
 
         # Calculate some *inclusive* zero based rectangle coords:
         self._data_area = (
             self._y_axis_width, self._margin, self._canvas_width - self._margin - 1,
             self._canvas_height - self._x_axis_height - 1)
         self._dead_space = (
             0, self._canvas_height - self._x_axis_height, self._y_axis_width - 1, self._canvas_height - 1)
 
-    def draw(self, canvas, x_range: AxisRange, y_range: AxisRange, show_grid: bool):
+    def draw(self, canvas, x_range: AxisRange, y_range: AxisRange, show_grid: bool, zero_based_x_axis: bool):
         super().draw(canvas, x_range, y_range, show_grid)
 
         """Draw a graph including axes, image and grid. We do this in two phases:
         (1) The axes etc, which are fast to draw, are drawn immediately by this method
         (2) The image and things overlaying it (such as the grid) are drawn later when the image
             has been calculated. A capture is returned that the caller can use later to do this.
         """
@@ -518,35 +569,36 @@
         # Fill the margins:
         Layout._create_rectangle(canvas, *self._get_top_margin(), AXIS_BG_COLOUR)
         Layout._create_rectangle(canvas, *self._get_right_margin(), AXIS_BG_COLOUR)
         Layout._create_rectangle(canvas, *self._dead_space, AXIS_BG_COLOUR)
 
         # Draw the axes:
         (yaxis_x, yaxis_y, yaxis_extent) = (0, self._margin, self._canvas_height - self._x_axis_height - self._margin)
-        y_ticks = self._y_axis.draw(canvas, yaxis_x, yaxis_y, yaxis_extent, y_range, multiplier=1000)
+        y_ticks = self._y_axis.draw(canvas, yaxis_x, yaxis_y, yaxis_extent, y_range, zero_based_axis=False)
 
         (xaxis_x, xaxis_y, xaxis_extent) = (
             self._y_axis_width - 1, self._canvas_height - self._x_axis.get_size(),
             self._canvas_width - self._y_axis_width - self._margin)
-        x_ticks = self._x_axis.draw(canvas, xaxis_x, xaxis_y, xaxis_extent, x_range)
+        x_ticks = self._x_axis.draw(canvas, xaxis_x, xaxis_y, xaxis_extent, x_range, zero_based_axis=zero_based_x_axis)
 
         # Create a capture that can be used to finish drawing the graph later on, when the image
         # is available:
-        def draw_followup(is_memory_limit_hit: bool = False, points=None, axis_range: AxisRange = AxisRange(rmin=0, rmax=1)):
+        def draw_followup(is_memory_limit_hit: bool = False, points=None,
+                          axis_range: AxisRange = AxisRange(rmin=0, rmax=1)):
             # Reblank the data area in case the two phases of drawing got out of order, to
             # avoid multiple data appearing on the same axis:
             l, t, r, b = self._data_area
             Layout._create_rectangle(canvas, l, t, r, b, 'black')
 
             # Redraw the x xaxis and adjacent margins, now that we know its range:
             Layout._create_rectangle(canvas, *self._get_right_margin(), AXIS_BG_COLOUR)
             Layout._create_rectangle(canvas, *self._dead_space, AXIS_BG_COLOUR)
             if not is_memory_limit_hit:
                 new_x_ticks = self._x_axis.draw(canvas, xaxis_x, xaxis_y, xaxis_extent, axis_range,
-                                                target_spacing_pixels=40)
+                                                target_spacing_pixels=40, zero_based_axis=zero_based_x_axis)
 
                 # Draw the actual data:
                 if points is not None:
                     self._draw_graph_points(canvas, self._data_area, points, '#00FFFF')
 
                 if show_grid:
                     self._draw_y_grid(canvas, y_ticks, self._data_area)
```

### Comparing `batogram-1.0.5/src/batogram/morebncframe.py` & `batogram-1.0.6/batogram/morebncframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,19 +17,17 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 import math
 import tkinter as tk
 import numpy as np
 
-from . import get_asset_path
-
+from . import colourmap
 from abc import abstractmethod, ABC
 from typing import Any, List, Tuple
-from .colourmap import ColourMap
 from .common import clip_to_range
 from .frames import DrawableFrame
 from .validatingwidgets import ValidatingMapOptionMenu, ValidatingFrameHelper, ValidatingRadiobutton, \
     DoubleValidatingEntry
 from .graphsettings import GraphSettings, BNC_MODES, borderwidth, BNC_ADAPTIVE_MODE, BNC_MANUAL_MODE, \
     BNC_INTERACTIVE_MODE
 
@@ -161,31 +159,26 @@
 
 class ScaleCanvas(tk.Canvas):
     """A canvas the displays the colour scale for a spectrogram."""
 
     def __init__(self, parent):
         super().__init__(parent, bg="black", height=15, width=CANVAS_WIDTH)
 
-        # For now, our own colour map. Eventually we need to use the same map
-        # as in the rendering pipeline, so that it can chosen in the UI.
-        self._colour_map = ColourMap()
-        self._colour_map.load_map(get_asset_path("kindlmann-table-byte-1024.csv"))
-
     def set_scale_pixels(self, prange: tuple[int, int] | None):
         """Draw a colour mapped scale."""
         width, height = self.winfo_width(), self.winfo_height()
 
         self.clear()
         if prange is not None:
             xmin, xmax = prange
             if xmin < xmax:
                 # Get values in the range 0-1. Values outside that range will be clippped
                 # to the limits at 0 and 1:
                 values = np.array([float(x - xmin) / float(xmax - xmin) for x in range(width)])
-                colours = self._colour_map.map(values)
+                colours = colourmap.instance.map(values)
                 for x in range(width):
                     colour = "#{:02x}{:02x}{:02x}".format(*colours[x])
                     self.create_line(x, 0, x, height - 1, fill=colour)
 
     def clear(self):
         self.delete("all")
```

### Comparing `batogram-1.0.5/src/batogram/moreframe.py` & `batogram-1.0.6/batogram/moreframe.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.5/src/batogram/morerenderingframe.py` & `batogram-1.0.6/batogram/morerenderingframe.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.5/src/batogram/morescaleframe.py` & `batogram-1.0.6/batogram/morescaleframe.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,29 +76,35 @@
         self._f_max = DoubleValidatingEntry(self, controlling_frame, self, width=width,
                                             decimal_places=self._FREQUENCY_DPS,
                                             scaler=self._FREQUENCY_SCALER, value_validator=f_max_validator)
         self._f_max.grid(row=2, column=2, padx=pad)
 
         self._show_grid_checkbutton = ValidatingCheckbutton(self, controlling_frame, self, "Show grid")
         self._show_grid_checkbutton.grid(row=1, column=4, padx=pad, sticky="W")
+
+        self._zero_based_time_checkbutton = ValidatingCheckbutton(self, controlling_frame, self, "Zero based time")
+        self._zero_based_time_checkbutton.grid(row=1, column=5, padx=pad, sticky="W")
+
         self._show_profile_checkbutton = ValidatingCheckbutton(self, controlling_frame, self, text="Show profile")
         self._show_profile_checkbutton.grid(row=2, column=4, padx=pad, sticky="W")
 
         self.copy_settings_to_widgets()
 
     def copy_settings_to_widgets(self):
         # Update the entry values from settings:
         self._t_max.set_value(self._settings.time_range.max)
         self._t_min.set_value(self._settings.time_range.min)
         self._f_max.set_value(self._settings.frequency_range.max)
         self._f_min.set_value(self._settings.frequency_range.min)
         self._show_grid_checkbutton.set_value(self._settings.show_grid)
+        self._zero_based_time_checkbutton.set_value(self._settings.zero_based_time)
         self._show_profile_checkbutton.set_value(self._settings.show_profile)
 
     def copy_widgets_to_settings(self):
         # Update the settings values from the UI:
         self._settings.time_range.max = self._t_max.get_value()
         self._settings.time_range.min = self._t_min.get_value()
         self._settings.frequency_range.max = self._f_max.get_value()
         self._settings.frequency_range.min = self._f_min.get_value()
         self._settings.show_grid = self._show_grid_checkbutton.get_value()
+        self._settings.zero_based_time = self._zero_based_time_checkbutton.get_value()
         self._settings.show_profile = self._show_profile_checkbutton.get_value()
```

### Comparing `batogram-1.0.5/src/batogram/profilegraphframe.py` & `batogram-1.0.6/batogram/profilegraphframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,16 @@
         # Allow the canvas to catch up with any pending resizes so that we get the right
         # size below:
         self.update_idletasks()
 
         width, height = self._canvas.winfo_width(), self._canvas.winfo_height()
         layout = layouts.ProfileLayout(FONT_SIZE, width, height)
         # Draw the graph axes here in the UI thread, as that is fast and provides responsiveness to the user:
-        graph_completer, data_area = layout.draw(self._canvas, profile_range, frequency_range, self._settings.show_grid)
+        graph_completer, data_area = layout.draw(self._canvas, profile_range, frequency_range,
+                                                 self._settings.show_grid, self._settings.zero_based_time)
         if af_data and self._pipeline:
             # Kick off the pipeline which will create a graph in another thread,
             # and complete by generating an event that will finish drawing the grph:
             self._completer = graph_completer
             screen_factors = self._parent.get_screen_factors()
             request = self._get_pipeline_request(af_data, data_area, time_range, frequency_range, screen_factors,
                                                  self._dc.get_afs())
```

### Comparing `batogram-1.0.5/src/batogram/readoutframe.py` & `batogram-1.0.6/batogram/readoutframe.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.5/src/batogram/rendering.py` & `batogram-1.0.6/batogram/rendering.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,23 +18,22 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import math
 import numpy as np
 import scipy
 
-from . import get_asset_path
+from . import colourmap, appsettings
 from copy import deepcopy
 from dataclasses import dataclass
 from threading import Lock, Thread, Condition
 from typing import Type, Tuple, Optional, Any, Callable
 from scipy import ndimage
 from .audiofileservice import AudioFileService, RawDataReader
 from .chunky_spectrogram import chunky_spectrogram
-from .colourmap import ColourMap
 from .common import AxisRange, AreaTuple, clip_to_range
 from .graphsettings import GraphSettings, ADAPTIVE_FFT_SAMPLES, ADAPTIVE_FFT_OVERLAP_PERCENT, \
     FFT_OVERLAP_PERCENT_OPTIONS, BNC_ADAPTIVE_MODE, BNC_MANUAL_MODE, BNC_INTERACTIVE_MODE
 
 
 class RenderingRequest:
     """The base class for rendering pipeline requests of any kind."""
@@ -326,72 +325,74 @@
             self.actual_fft_overlap_percent = settings.fft_overlap
 
         self.actual_fft_overlap_samples = int(self.actual_fft_overlap_percent / 100.0 * self.actual_fft_samples)
         self.step_count: int = int(self.actual_fft_samples - self.actual_fft_overlap_samples)
         half_segment_offset: int = int(self.actual_fft_samples / 2)  # Ignore the rounding error, small.
         step_time: float = (self.actual_fft_samples - self.actual_fft_overlap_samples) / sample_rate
         time_points = file_data.sample_count
-        max_segments: int = int(
-            (time_points - half_segment_offset) / self.step_count) + 1  # Ignore any leftover time points.
+        # max_segment_count: int = int((time_points - half_segment_offset) / self.step_count) + 1  # Ignore any leftover time points.
+        max_segment_count: int = int((time_points - self.actual_fft_overlap_samples) / self.step_count)  # Ignore any leftover time points.
         time_axis_min, time_axis_max = axis_time_range.get_tuple()
         freq_axis_min, freq_axis_max = axis_frequency_range.get_tuple()
 
         # ************** Calculations relating to the time axis **************
 
         def time_to_segment_index(t: float) -> int:
-            """Get the segment number corresponding to the time. t=0 at the centre of
+            """Get the segment number corresponding to the axis time. t=0 at the centre of
             the first segment, and offsets are constant between there and subsequent
             centres. We round down intentionally."""
-            segment_index = int(t / step_time + 0.5)  # This rounds *down* to the nearest step
+            segment_index = int(t / step_time)  # This rounds *down* to the nearest step
             return segment_index
 
         def segment_index_to_time(i: int) -> float:
             """Get the axis time corresponding to a segment index - which is the time at the centre of the segment."""
-            t = i * step_time
+            t = i * step_time # - step_time / 2
             return t
 
         def segment_index_to_time_index(segment_index: int):
-            """Get the index of the first time value that is part of the segment."""
-            # Offset for the spacing of centres AND the negative time range.
+            """Get the index of the FIRST time value that is part of the segment."""
+            # Offset for the spacing of centres - a negative time range index may result.
             time_index = int(segment_index * self.step_count - half_segment_offset)
             return time_index
 
         def time_to_time_index(t: float):
-            """Get the index of the time sample at this axis time."""
-            time_index = int(t * sample_rate)
+            """Get the index of the time sample at the centre of the segment whose centre
+            is this axis time."""
+            time_index = int(t * sample_rate) + half_segment_offset
             return time_index
 
         # Convert the axis ranges supplied to data index ranges, rounding outwards.
         # t=0 is the centre of the first sfft segment, so it depends in the window size.
         # This convention avoids varying time offsets as different window sizes are selected.
 
         self.first_segment_index = time_to_segment_index(time_axis_min)
-        self.last_segment_index: int = self.first_segment_index + math.ceil(
-            (time_axis_max - time_axis_min) / step_time) + 1 + 1  # Half open and round outwards.
+        self.last_segment_index: int = self.first_segment_index + math.ceil(    # Round outwards.
+            (time_axis_max - time_axis_min) / step_time) + 1                    # Half open.
 
         # Allow a left and right margin to hide any edge artifacts from zooming. The
         # result is data indexes that may be outside the range of available data:
         margin: int = 10
         self.first_segment_index -= margin
         self.last_segment_index += margin
 
-        # Limit the segment indexes to the possible range:
+        # Limit the segment indexes to the possible range, last segment index is half open:
         self.first_segment_index = max(0, self.first_segment_index)  # Shouldn't be needed.
-        self.last_segment_index = min(max_segments, self.last_segment_index)
+        self.last_segment_index = min(max_segment_count, self.last_segment_index)
 
         # Convert the segment index range to a time index range. We know the time indexes are sane,
         # because we clipped the segment indexes above. These time index ranges are the range needed
         # to calculate the segments - not the time range of the segments.
-
         self.first_time_index_for_segs = segment_index_to_time_index(self.first_segment_index)
-        self.last_time_index_for_segs = segment_index_to_time_index(self.last_segment_index)
+        # Note: (1) the last_segment_index is half open so - 1. (2) include the full index range for the previous
+        # segment so that it can be calculated.
+        self.last_time_index_for_segs = segment_index_to_time_index(self.last_segment_index - 1) + self.actual_fft_samples
 
         # Reverse calculate to the time range we actually cover, which is the segment centres.
         self.actual_time_axis_min = segment_index_to_time(self.first_segment_index)
-        self.actual_time_axis_max = segment_index_to_time(self.last_segment_index)
+        self.actual_time_axis_max = segment_index_to_time(self.last_segment_index - 1)  # -1 because half open range
 
         # Calculate the time index range corresponding to the actual axis values:
         self.first_time_index_for_amp = time_to_time_index(self.actual_time_axis_min)
         self.last_time_index_for_amp = time_to_time_index(self.actual_time_axis_max)
 
         # ************** Calculations relating to the frequency axis **************
 
@@ -458,14 +459,15 @@
 
         fft_samples_squared = sample_rate * sample_rate * overlap_ratio * aspect_factor
 
         fft_samples = int(scipy.sqrt(fft_samples_squared) + 0.5)
 
         # Round to the nearest factor of 2:
         rounded_fft_samples = 2 ** int(scipy.log2(fft_samples) + 0.5)
+        rounded_fft_samples *= 2  # Subjectively, this looks better.
 
         # These limits need to make the range of samples that can be selected manually:
         rounded_fft_samples = max(64, rounded_fft_samples)
         rounded_fft_samples = min(4096, rounded_fft_samples)
 
         # print("calculated fft samples = {}".format(rounded_fft_samples))
 
@@ -806,21 +808,23 @@
 
         # The segment and frequency range provided matches that in the calc data:
         clipped_inputdata = specdata[calc_data.first_freq_index:calc_data.last_freq_index, :]
 
         # Zoom the spectrogram index ranges into dilated canvas pixels size:
         y_scaler: float = calc_data.freq_dilated_pixels / (calc_data.last_freq_index - calc_data.first_freq_index)
         x_scaler: float = calc_data.time_dilated_pixels / (calc_data.last_segment_index - calc_data.first_segment_index)
+
         dilated_canvas_data = ndimage.zoom(clipped_inputdata,
                                            (y_scaler, x_scaler),
                                            # Scale to apply per axis.
+                                           # order=rs.zoom_interpolation,  # Interpolation spline order
                                            order=rs.zoom_interpolation,  # Interpolation spline order
                                            mode='nearest',
                                            # grid-constant results in bright artifacts at the bottom edge.
-                                           prefilter=True,  # To avoid slight blurring.
+                                           prefilter=False,  # Subjectively looks better as False: fewer artifacts.
                                            grid_mode=True)  # n pixels <=> width is n.
 
         # Clip the canvas dilated size back to the size we need to display:
         freq_offset_pixels = max(calc_data.freq_offset_pixels, 0)  # Paranoia.
         time_offset_pixels = max(calc_data.time_offset_pixels, 0)
         # Note: slicing fails gracefully if the upper value > array size.
         outputdata = dilated_canvas_data[
@@ -901,34 +905,30 @@
 
 class SpectrogramApplyColourMapStep(PipelineStep):
     """Replace each value in the supplied data with an RGB colour"""
 
     def __init__(self, settings: GraphSettings):
         super().__init__(settings)
 
-        self._colour_map = ColourMap()
-        self._colour_map.load_map(get_asset_path("kindlmann-table-byte-1024.csv"))
-
     @dataclass
     class RelevantSettings:
-        colour_mapping_path: str
+        colour_map_name: str  # Included slightly artificially to invalidate cached results.
 
         def __init__(self, settings: GraphSettings):
-            self.colour_mapping_path = settings.colour_mapping_path
+            self.colour_map_name = appsettings.instance.colour_map
 
     def get_relevant_settings(self) -> RelevantSettings:
         """Get the settings subset that is relevant to this step. We will use this as a basis
         for cache invalidation."""
-        # TODO not used for now:
         return SpectrogramApplyColourMapStep.RelevantSettings(self._settings)
 
     def _implementation(self, inputdata, params):
         # previous_serial, = params
         # s = self.get_relevant_settings()
-        outputdata = self._colour_map.map(inputdata)
+        outputdata = colourmap.instance.map(inputdata)
         return outputdata
 
 
 class AmplitudePipelineRequest(RenderingRequest):
     def __init__(self, data_area, file_data: AudioFileService.RenderingData, time_range: AxisRange,
                  frequency_range: AxisRange,
                  amplitude_range: AxisRange, screen_factors: tuple[float, float], rdr: RawDataReader):
@@ -1212,15 +1212,15 @@
         previous_serial, height, width = params
 
         # The input is the spectrogram data. Aggregate each row to get the profile.
         # Use a percentile to focus on the signal, while trimming some noise:
         try:
             profile_data = np.percentile(input_data, 98, axis=1)
         except IndexError as e:
-            profile_data = np.mean(input_data, axis=1)      # If there is no data in the percentile.
+            profile_data = np.mean(input_data, axis=1)  # If there is no data in the percentile.
 
         rows, = profile_data.shape
 
         # Create a series of x,y points for the profile:
         profile_points = np.zeros((rows, 2), dtype=np.int16)
 
         vmax, vmin = profile_data.max(), profile_data.min()
```

### Comparing `batogram-1.0.5/src/batogram/rootwindow.py` & `batogram-1.0.6/batogram/rootwindow.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!./venv/bin/python3
-
 # Copyright (c) 2023 John Mears
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
@@ -24,17 +22,18 @@
 import tkinter as tk
 import tkinter.filedialog
 import tkinter.messagebox
 
 from itertools import chain
 from timeit import default_timer as timer
 from typing import NamedTuple, Optional
-from pathlib import Path
-from . import audiofileservice as af
+from . import audiofileservice as af, appsettings, colourmap
 from .amplitudegraphframe import AmplitudeGraphFrame
+from .appsettings import COLOUR_MAPS
+from .appsettingsmodal import AppSettingsWindow
 from .audiofileservice import AudioFileService
 from .breadcrumbservice import BreadcrumbService, Breadcrumb
 from .buttonframe import ButtonFrame
 from .common import AxisRange
 from .constants import *
 from .fileinfoframe import FileInfoFrame
 from .frames import DrawableFrame
@@ -49,14 +48,15 @@
 from .wavfileparser import WavFileError
 from .about import AboutWindow
 from . import get_asset_path
 
 # One day, we will define the menus using a table including shortcuts and underlined letters:
 MENU_TEXT_FILE = "File"
 MENU_TEXT_ABOUT = "About"
+MENU_TEXT_SETTINGS = "Settings"
 MENU_TEXT_OPEN_MAIN = "Open"
 MENU_TEXT_OPEN_RECENT_MAIN = "Open recent"
 MENU_TEXT_OPEN_REF = "Open reference"
 MENU_TEXT_OPEN_RECENT_REF = "Open recent as reference"
 MENU_TEXT_CLOSE_MAIN = "Close"
 MENU_TEXT_CLOSE_REF = "Close reference"
 # MENU_TEXT_SAVE = "Save"
@@ -156,23 +156,22 @@
         initial_cursor_mode = self._button_frame.get_cursor_mode()
 
         self._amplitude_frame = AmplitudeGraphFrame(self, root, pipelines.amplitude, self._dc, self._settings,
                                                     is_reference=is_reference)
         self._amplitude_frame.grid(row=2, column=col, sticky='nesw', padx=pad)
 
         self._spectrogram_frame = SpectrogramGraphFrame(self, root, pipelines.spectrogram, self._dc, self._settings,
-                                                        initial_cursor_mode, self.on_rescale_handler,
-                                                        is_reference=is_reference)
+                                                        initial_cursor_mode, is_reference=is_reference)
         self._spectrogram_frame.grid(row=3, column=col, sticky='nesw', padx=pad)
 
         # Set up two-way communications between the scroll bar and the graph frame.
         # Set repeatdelay=0 to disable repeating, which behaves oddly.
-        time_scroller = tk.Scrollbar(self, orient='horizontal', jump=True, repeatdelay=0)
-        self._spectrogram_frame.set_scroller_t(time_scroller)
-        time_scroller.grid(row=4, column=col, sticky="ew", padx=pad)
+        self._time_scroller = tk.Scrollbar(self, orient='horizontal', jump=True, repeatdelay=0)
+        self._spectrogram_frame.set_scroller_t(self._time_scroller)
+        self._time_scroller.grid(row=4, column=col, sticky="ew", padx=pad)
 
         self._readout_frame = ReadoutFrame(self)
         self._readout_frame.grid(row=6, column=col, pady=pad, sticky='we')
 
         col = 1
         self._profile_frame = ProfileGraphFrame(self, root, pipelines.profile, self._dc, self._settings)
         self._profile_frame.grid(row=3, column=col, sticky='ns')
@@ -231,14 +230,47 @@
 
         self._dc.time_range, self._dc.frequency_range = time_range, frequency_range
         if add_breadcrumb:
             self._dc.push_breadcrumb()
 
         self.draw(draw_scope)
 
+    def on_scroll_handler(self, delta_t: float, delta_f: float,
+                          range_t: AxisRange, range_f: AxisRange, add_breadcrumb=True):
+        """
+        Scroll time and/or frequency in response to the UI, maintaining the range, and limiting
+        to the range of available data. The deltas must be less than the current axis ranges.
+        """
+
+        # Limit the the deltas to the range of the available data, maintaining the span of each axis,
+        # and assuming (1) the existing range is valid (2) the deltas are less than the current axis ranges.
+        af_data = self._dc.get_afs_data()
+        if af_data:
+            time_min, time_max = af_data.time_range.get_tuple()
+            if delta_t > 0:
+                if range_t.max + delta_t > time_max:
+                    delta_t = time_max - range_t.max
+            else:
+                if range_t.min + delta_t < time_min:
+                    delta_t = -(range_t.min - time_min)
+
+            freq_min, freq_max = af_data.frequency_range.get_tuple()
+            if delta_f > 0:
+                if range_f.max + delta_f > freq_max:
+                    delta_f = freq_max - range_f.max
+            else:
+                if range_f.min + delta_f < freq_min:
+                    delta_f = -(range_f.min - freq_min)
+
+        limited_range_t = AxisRange(range_t.min + delta_t, range_t.max + delta_t)
+        limited_range_f = AxisRange(range_f.min + delta_f, range_f.max + delta_f)
+
+        self.on_rescale_handler(limited_range_t, limited_range_f,
+                                add_breadcrumb=add_breadcrumb, draw_scope=DrawableFrame.DRAW_ALL)
+
     def draw(self, draw_scope: int = DrawableFrame.DRAW_ALL):
         # Update the settings to match the *actual* new axis ranges:
         self._settings.time_range = self._dc.time_range
         self._settings.frequency_range = self._dc.frequency_range
         self._settings.on_app_modified_settings()
 
         # Show or hide the profile graph as required:
@@ -314,14 +346,50 @@
         self.on_rescale_handler(centred_time_range, frequency_range, add_breadcrumb=True)
 
     def get_screen_factors(self) -> tuple[float, float]:
         # Calculate the screen aspect factor based on the spectrogram graph,
         # that will be used in adaptive window length calculations.
         return self._spectrogram_frame.calculate_screen_factors()
 
+    def on_left_key(self, event):
+        self._spectrogram_frame.tview(tk.SCROLL, -1, tk.UNITS)
+
+    def on_shift_left_key(self, event):
+        self._spectrogram_frame.tview(tk.SCROLL, -1, tk.PAGES)
+
+    def on_right_key(self, event):
+        self._spectrogram_frame.tview(tk.SCROLL, 1, tk.UNITS)
+
+    def on_shift_right_key(self, event):
+        self._spectrogram_frame.tview(tk.SCROLL, 1, tk.PAGES)
+
+    def on_up_key(self, event):
+        self._spectrogram_frame.set_preset_time_range(-1)
+
+    def on_shift_up_key(self, event):
+        pass
+
+    def on_down_key(self, event):
+        self._spectrogram_frame.set_preset_time_range(+1)
+
+    def on_shift_down_key(self, event):
+        pass
+
+    def on_page_up_key(self, event):
+        self._spectrogram_frame.fview(tk.SCROLL, -1, tk.UNITS)
+
+    def on_shift_page_up_key(self, event):
+        self._spectrogram_frame.fview(tk.SCROLL, -1, tk.PAGES)
+
+    def on_page_down_key(self, event):
+        self._spectrogram_frame.fview(tk.SCROLL, 1, tk.UNITS)
+
+    def on_shift_page_down_key(self, event):
+        self._spectrogram_frame.fview(tk.SCROLL, 1, tk.PAGES)
+
 
 class DataContext:
     """This class contains data used by a graph pane, including raw file data and axis ranges."""
 
     DEFAULT_TIME_RANGE = AxisRange(rmin=0, rmax=30)
     DEFAULT_FREQUENCY_RANGE = AxisRange(rmin=0, rmax=192000)
     DEFAULT_AMPLITUDE_RANGE = AxisRange(rmin=-1, rmax=1)
@@ -393,15 +461,18 @@
 
         self._menu_recent_main = None
         self._menu_recent_ref = None
         self._menu_analysis = None
         self._menu_image = None
         self._menu_edit = None
         self._menu_file = None
-        self._first_file_open = True    # Track whether this is the first time the user has opened a file.
+        self._first_file_open = True  # Track whether this is the first time the user has opened a file.
+
+        appsettings.instance.read()
+        self._apply_settings()
 
         # Keep track of what cursors have been set:
         self._cursor_stack = []
         self._push_cursor()
 
         self.title(PROGRAM_NAME)
 
@@ -416,14 +487,27 @@
 
         self._create_menus()
         self._create_widgets()
 
         self.bind(DATA_CHANGE_MAIN_EVENT, self._on_data_change_main)
         self.bind(DATA_CHANGE_REF_EVENT, self._on_data_change_ref)
 
+        self.bind('<Left>', self._main_pane.on_left_key)
+        self.bind('<Shift-Left>', self._main_pane.on_shift_left_key)
+        self.bind('<Right>', self._main_pane.on_right_key)
+        self.bind('<Shift-Right>', self._main_pane.on_shift_right_key)
+        self.bind('<Up>', self._main_pane.on_up_key)
+        self.bind('<Shift-Up>', self._main_pane.on_shift_up_key)
+        self.bind('<Down>', self._main_pane.on_down_key)
+        self.bind('<Shift-Down>', self._main_pane.on_shift_down_key)
+        self.bind('<Prior>', self._main_pane.on_page_up_key)
+        self.bind('<Shift-Prior>', self._main_pane.on_shift_page_up_key)
+        self.bind('<Next>', self._main_pane.on_page_down_key)
+        self.bind('<Shift-Next>', self._main_pane.on_shift_page_down_key)
+
         # Allow tk to work out the size of things before we try to draw any graphs:
         self.update_idletasks()
 
         self._main_pane.draw()
         self._ref_pane.draw()
 
         if initialfile is not None:
@@ -524,14 +608,16 @@
 
         # self._menu_file.add_command(label=MENU_TEXT_SAVE, command=self.save_files_as)
         # self._menu_file.add_separator()
         self._menu_file.add_command(label=MENU_TEXT_EXIT, command=self.exit)
         self._menu_file.entryconfigure(MENU_TEXT_EXIT, accelerator='Ctrl+X')
         self.bind("<Control-x>", self.exit_event)
 
+        menubar.add_command(label=MENU_TEXT_SETTINGS, command=self._show_settings)
+
         menubar.add_command(label=MENU_TEXT_ABOUT, command=self._show_about)
 
         self.enable_menu_items()
 
     @staticmethod
     def _populate_file_history(parent_menu_item, historian, method):
         parent_menu_item.delete(0, "end")
@@ -569,15 +655,16 @@
     def _open_main_file_event(self, _):
         self._open_main_file()
 
     def _open_file_dialog(self, title: str):
         initialdir = None
         if self._first_file_open:
             self._first_file_open = False
-            initialdir = Path.home()
+            initialdir = appsettings.instance.data_directory
+
         filepath = tk.filedialog.askopenfilename(title=title, filetypes=self.filetypes,
                                                  initialdir=initialdir)
         return filepath
 
     def _open_main_file(self):
         filepath = self._open_file_dialog("Open an audio file")
         if filepath:
@@ -646,14 +733,16 @@
         if (tk.messagebox.askokcancel(
                 message='Are you sure you want to exit {}?'.format(PROGRAM_NAME),
                 icon='question', title='Exit')):
             for p in chain(self._main_pipelines, self._ref_pipelines):
                 if p:
                     p.shutdown()
 
+            appsettings.instance.write()
+
             self.destroy()
 
     def _on_data_change_main(self, _):
         self._dc_main.on_data_change()
         self._main_pane.draw()
         # Tell the other pane we can accept sync requests (as we have some data):
         sync_source = self._main_pane if self._dc_main.afs else None
@@ -689,7 +778,24 @@
         # New settings values are available to be applied to the application.
         self._ref_pane.on_user_applied_settings(draw_scope)
 
     def _show_about(self):
         window = AboutWindow(self)
         window.grab_set()
         window.wait_window()
+
+    def _show_settings(self):
+        modal = AppSettingsWindow(self, appsettings.instance, lambda: self._on_settings_ok())
+        modal.grab_set()
+        modal.wait_window()
+
+    def _on_settings_ok(self):
+        # Refresh some things from the updated settings values:
+        self._apply_settings()
+        self._main_pane.draw()
+        self._ref_pane.draw()
+
+    @staticmethod
+    def _apply_settings():
+        # Refresh some things from the updated settings values:
+        cmap_file = COLOUR_MAPS[appsettings.instance.colour_map]
+        colourmap.instance.reload_map(cmap_file)
```

### Comparing `batogram-1.0.5/src/batogram/spectrogramgraphframe.py` & `batogram-1.0.6/batogram/spectrogramgraphframe.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import tkinter as tk
+from typing import Tuple
 
 from .constants import MAIN_SPECTROGAM_COMPLETER_EVENT, FONT_SIZE, MIN_F_RANGE, MIN_T_RANGE
 from . import layouts
 from .audiofileservice import RawDataReader, AudioFileService
 from .common import AxisRange
 from .frames import GraphFrame, DrawableFrame
 from .spectrogrammouseservice import SpectrogramMouseService, CursorMode
@@ -44,19 +45,18 @@
     def notify_draw_complete(self):
         self._mouse_service.notify_draw_complete()
 
 
 class SpectrogramGraphFrame(GraphFrame):
     """A graph frame containing a spectrogram."""
 
-    def __init__(self, parent, root, pipeline, data_context, settings, initial_cursor_mode, on_rescale_handler, is_reference=False):
+    def __init__(self, parent: "PanelFrame", root, pipeline, data_context, settings, initial_cursor_mode, is_reference=False):
         super().__init__(parent, root, pipeline, data_context, settings)
 
         self._is_reference = is_reference
-        self._on_rescale_handler = on_rescale_handler
         self._canvas = SpectrogramCanvas(self, height=100, width=100, initial_cursor_mode=initial_cursor_mode)
         self._canvas.grid(row=0, column=0, sticky='nesw')
         self.columnconfigure(0, weight=1)
         self.rowconfigure(0, weight=1)
 
         self._layout = None
         self._histogram_interface: HistogramInterface | None = None
@@ -121,15 +121,16 @@
         # Allow the canvas to catch up with any pending resizes so that we get the right
         # size below:        self._parent = parent
         self.update_idletasks()
 
         width, height = self.get_canvas_size()
         self._layout = layouts.SpectrogramLayout(FONT_SIZE, width, height)
         # Draw the graph axes here in the UI thread, as that is fast and provides responsiveness to the user:
-        graph_completer, data_area = self._layout.draw(self._canvas, time_range, frequency_range, self._settings.show_grid)
+        graph_completer, data_area = self._layout.draw(self._canvas, time_range, frequency_range, self._settings.show_grid,
+                                                       self._settings.zero_based_time)
 
         if afs_data:
             self._update_time_scroller(time_range, afs_data.time_range)
             self._update_frequency_scroller(frequency_range, afs_data.frequency_range)
             if self._pipeline:
                 # Kick off the pipeline which will create a spectrogram in another thread,
                 # and complete by generating an event that will finish drawing the graph in
@@ -186,21 +187,21 @@
                 # Update the manual BnC range to the settings and settings UI:
                 if auto_vrange is not None:
                     self._settings.bnc_manual_min, self._settings.bnc_manual_max = auto_vrange
                     self._settings.on_app_modified_settings()
                 # Update the BnC histogram from the range discovered.
                 self._histogram_interface.show_histogram(histogram)
 
-    def on_zoom_to_rect(self, rect, frequency_clamped: bool):
+    def on_zoom_to_rect(self, rect: Tuple[int, int, int, int]):
         """Rescale to the pixel rectangle provided."""
         if self._layout is None:
             return  # No layout, we can't do anything.
 
         # Convert the canvas coords to axes values:
-        r_values = self._layout.rect_to_values(rect, frequency_clamped)
+        r_values = self._layout.rect_to_values(rect)
 
         # print("Rescaling graph to r_values {}".format(r_values))
 
         l, t, r, b = r_values
         # Sanity, avoid divisions by zero. Shouldn't ever happen...
         if not l < r:
             r = l + 1
@@ -211,33 +212,33 @@
         f_delta, t_delta = t - b, r - l
         if f_delta < MIN_F_RANGE or t_delta < MIN_T_RANGE:
             print("Ignoring insane zoom.")
             return  # Insane zoom requested, ignore it.
 
         # Notify news of this rescale back to the main window so that it can redraw widgets affected:
         # news to widgets that need to know.
-        self._on_rescale_handler(AxisRange(l, r), AxisRange(b, t))
+        self._parent.on_rescale_handler(AxisRange(l, r), AxisRange(b, t))
 
     def on_pan(self, rect):
         """This is called in response to the user dragging a pan line with the mouse."""
         if self._layout is None:
             return  # No layout, we can't do anything.
 
         # The following will clip pan line to the range of the axes:
-        t1, f1, t2, f2 = self._layout.rect_to_values(rect, frequency_clamped=False)
+        t1, f1, t2, f2 = self._layout.rect_to_values(rect)
         dt_value, df_value = t2 - t1, f2 - f1
 
         # print("Panning graph by {}, {}".format(dt_value, df_value))
 
         # Apply the pan:
         t_range, f_range = self._layout.get_data_ranges()
         (l, r), (b, t) = t_range.get_tuple(), f_range.get_tuple()
         l, r, b, t = l - dt_value, r - dt_value, b - df_value, t - df_value
 
-        self._on_rescale_handler(AxisRange(l, r), AxisRange(b, t))
+        self._parent.on_rescale_handler(AxisRange(l, r), AxisRange(b, t))
 
     def on_zoom_about_centre(self, position, factor, frequency_clamped: bool) -> bool:
         """
         Optionally pan so that pixel position is centered, then apply the zoom factor.
         Return True if the new range was sane and we applied it, otherwise false.
         """
 
@@ -270,17 +271,17 @@
         # Apply the zoom:
         l, t, r, b = l * factor, t * factor, r * factor, b * factor
         # Reverse the offset we applied:
         l, t, r, b = l + centre_t_v, t + centre_f_v, r + centre_t_v, b + centre_f_v
 
         if frequency_clamped:
             _, frequency_range = self._layout.get_data_ranges()
-            self._on_rescale_handler(AxisRange(l, r), frequency_range)
+            self._parent.on_rescale_handler(AxisRange(l, r), frequency_range)
         else:
-            self._on_rescale_handler(AxisRange(l, r), AxisRange(b, t))
+            self._parent.on_rescale_handler(AxisRange(l, r), AxisRange(b, t))
 
         return True
 
     def on_mouse_move(self, p_canvas):
         # print("on mouse move")
 
         if p_canvas is None or self._layout is None:
@@ -307,15 +308,15 @@
         _, range_f = self._layout.get_data_ranges()
         axis_fmin, axis_fmax = range_f.get_tuple()
 
         # The total time range available is the data file range minus the time axis range:
         resultant_tmin = (file_tmax - file_tmin) * new_tmin + file_tmin
         resultant_tmax = (file_tmax - file_tmin) * new_tmax + file_tmin
 
-        self._on_rescale_handler(AxisRange(resultant_tmin, resultant_tmax), AxisRange(axis_fmin, axis_fmax))
+        self._parent.on_rescale_handler(AxisRange(resultant_tmin, resultant_tmax), AxisRange(axis_fmin, axis_fmax))
 
     def _scroll_move_frequency(self, _):
         # Scroll frequency to position f which is in the range 0 to 1.0.
 
         data: AudioFileService.RenderingData = self._dc.get_afs_data()
         if data is None:
             return
@@ -327,15 +328,15 @@
         file_fmin, file_fmax = data.frequency_range.get_tuple()
         range_t, _ = self._layout.get_data_ranges()
         axis_tmin, axis_tmax = range_t.get_tuple()
         # The total time range available is the data file range minus the time axis range:
         resultant_fmin = (file_fmax - file_fmin) * new_fmin + file_fmin
         resultant_fmax = (file_fmax - file_fmin) * new_fmax + file_fmin
 
-        self._on_rescale_handler(AxisRange(axis_tmin, axis_tmax), AxisRange(resultant_fmin, resultant_fmax))
+        self._parent.on_rescale_handler(AxisRange(axis_tmin, axis_tmax), AxisRange(resultant_fmin, resultant_fmax))
 
     def _scroll_delta_time(self, sign_s, size):
         # Apply a step to the scroll f which is in the range 0 to 1.0.
 
         data = self._dc.get_afs()
         if data is None:
             return
@@ -343,20 +344,19 @@
         range_t, range_f = self._layout.get_data_ranges()
         axis_t_span = range_t.max - range_t.min
 
         sign = int(sign_s)
         if size == tk.UNITS:
             delta_t = axis_t_span * 0.05 * sign
         elif size == tk.PAGES:
-            delta_t = axis_t_span * 0.9 * sign
+            delta_t = axis_t_span * 0.8 * sign
         else:
             return
 
-        resultant_range = AxisRange(range_t.min + delta_t, range_t.max + delta_t)
-        self._on_rescale_handler(resultant_range, AxisRange(range_f.min, range_f.max))
+        self._parent.on_scroll_handler(delta_t, 0, range_t, range_f)
 
     def _scroll_delta_frequency(self, sign_s, size):
         # Apply a step to the scroll f which is in the range 0 to 1.0.
 
         data = self._dc.get_afs()
         if data is None:
             return
@@ -364,22 +364,44 @@
         range_t, range_f = self._layout.get_data_ranges()
         axis_f_span = range_f.max - range_f.min
 
         sign = int(sign_s)
         # Vertical scrollers increase downward:
         sign = sign * -1.0
         if size == tk.UNITS:
-            delta_t = axis_f_span * 0.05 * sign
+            delta_f = axis_f_span * 0.05 * sign
         elif size == tk.PAGES:
-            delta_t = axis_f_span * 0.9 * sign
+            delta_f = axis_f_span * 0.9 * sign
         else:
             return
 
-        resultant_range = AxisRange(range_f.min + delta_t, range_f.max + delta_t)
-        self._on_rescale_handler(AxisRange(range_t.min, range_t.max), resultant_range)
+        self._parent.on_scroll_handler(0, delta_f, range_t, range_f)
+
+    def set_preset_time_range(self, sign: int):
+        """Zoom the time range in or out, centered on the current range.
+        Positive sign increases the axis range, ie zoom out.
+        """
+
+        time_range, _ = self._layout.get_data_ranges()
+        centre = (time_range.min + time_range.max) / 2
+        span = time_range.max - time_range.min
+
+        if sign > 0:
+            span *= 1.2
+        else:
+            span *= 0.8
+
+        if span < MIN_T_RANGE:
+            # Allow them to zoom back out again, to avoid getting stuck.
+            if sign < 0:
+                print("Ignoring insane zoom in.")
+                return False  # Insane zoom requested, ignore it.
+
+        _, frequency_range = self._layout.get_data_ranges()
+        self._parent.on_rescale_handler(AxisRange(centre - span / 2, centre + span / 2), frequency_range)
 
     def _update_time_scroller(self, axis_range, file_range):
         if self._scroller_t is None:
             return
 
         # Set the time scroller so that the bar represents the visible part of the data,
         # scaled to the range 0 to 1.0.
```

### Comparing `batogram-1.0.5/src/batogram/spectrogrammouseservice.py` & `batogram-1.0.6/batogram/spectrogrammouseservice.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,24 +20,31 @@
 
 import tkinter as tk
 
 from enum import Enum
 from timeit import default_timer as timer
 from typing import Tuple
 
-DRAG_RECTANGLE_COLOUR = "white"
-DRAG_LINE_COLOUR = "white"
+# Grey, so its visible against black and white.
+DRAG_RECTANGLE_COLOUR = "grey"
+DRAG_LINE_COLOUR = "grey"
 ARROW_SHAPE = (16, 20, 6)
 
 
 class CursorMode(Enum):
     CURSOR_ZOOM = 0
     CURSOR_PAN = 1
 
 
+class DragMode(Enum):
+    DRAG_HORIZONTAL = 0
+    DRAG_VERTICAL = 1
+    DRAG_RECTANGLE = 2
+
+
 class MouseState(Enum):
     START = 1
     LEFT_DRAGGING = 2
     MIDDLE_DRAGGING = 3
 
 
 class SpectrogramMouseService:
@@ -58,30 +65,33 @@
         self._state: MouseState = MouseState.START
         self._start_position = None
         self._rect = None
         self._line = None
         self._line1 = None
         self._line2 = None
         self._last_wheel_time = timer()
-        self._is_frequency_clamped: bool = False
         self._canvas_height: int | None = None
+        self._canvas_width: int | None = None
+        self._last_drag_mode: DragMode | None = None
 
         # Left mouse button:
         canvas.bind('<ButtonPress-1>', self._on_button1_press)
-        canvas.bind('<Shift-ButtonPress-1>', self._on_shift_button1_press)
+        canvas.bind('<Shift-ButtonPress-1>', self._on_button1_press)
         canvas.bind('<ButtonRelease-1>', self._on_button1_release)
-        canvas.bind('<Shift-ButtonRelease-1>', self._on_button1_release)
+        canvas.bind('<Shift-ButtonRelease-1>', self._on_shift_button1_release)
         canvas.bind('<B1-Motion>', self._on_button1_move)
+        canvas.bind('<Shift-B1-Motion>', self._on_shift_button1_move)
 
         # Middle mouse button:
         canvas.bind('<ButtonPress-2>', self._on_button2_press)
-        canvas.bind('<Shift-ButtonPress-2>', self._on_shift_button2_press)
+        canvas.bind('<Shift-ButtonPress-2>', self._on_button2_press)
         canvas.bind('<ButtonRelease-2>', self._on_button2_release)
-        canvas.bind('<Shift-ButtonRelease-2>', self._on_button2_release)
+        canvas.bind('<Shift-ButtonRelease-2>', self._on_shift_button2_release)
         canvas.bind('<B2-Motion>', self._on_button2_move)
+        canvas.bind('<Shift-B2-Motion>', self._on_shift_button2_move)
 
         # Right mouse button:
         canvas.bind('<ButtonPress-3>', self._on_button3_press)
         canvas.bind('<ButtonRelease-3>', self._on_button3_release)
         canvas.bind('<B3-Motion>', self._on_button3_move)
 
         # Any mouse motion:
@@ -90,74 +100,83 @@
 
         # Mouse wheel:
         self._bind_wheel()
 
     def _on_button1_press(self, event):
         # print("1+")
         if self._cursor_mode == CursorMode.CURSOR_ZOOM:
-            self._on_zoom_press(event, clamp=False)
+            self._on_zoom_press(event)
         elif self._cursor_mode == CursorMode.CURSOR_PAN:
-            self._on_pan_press(event, clamp=False)
+            self._on_pan_press(event)
 
-    def _on_shift_button1_press(self, event):
+    def _on_button1_move(self, event):
         if self._cursor_mode == CursorMode.CURSOR_ZOOM:
-            self._on_zoom_press(event, clamp=True)
+            self._on_zoom_move(event, is_shift=False)
         elif self._cursor_mode == CursorMode.CURSOR_PAN:
-            self._on_pan_press(event, clamp=True)
+            self._on_pan_move(event, is_shift=False)
 
-    def _on_button1_move(self, event):
+    def _on_shift_button1_move(self, event):
         if self._cursor_mode == CursorMode.CURSOR_ZOOM:
-            self._on_zoom_move(event)
+            self._on_zoom_move(event, is_shift=True)
         elif self._cursor_mode == CursorMode.CURSOR_PAN:
-            self._on_pan_move(event)
+            self._on_pan_move(event, is_shift=True)
 
     def _on_button1_release(self, event):
-        # print("1-")
         if self._cursor_mode == CursorMode.CURSOR_ZOOM:
-            self._on_zoom_release(event)
+            self._on_zoom_release(event, is_shift=False)
         elif self._cursor_mode == CursorMode.CURSOR_PAN:
-            self._on_pan_release(event)
+            self._on_pan_release(event, is_shift=False)
 
-    def _on_button2_press(self, event):
-        # print("2+")
-        self._on_pan_press(event, clamp=False)
+    def _on_shift_button1_release(self, event):
+        if self._cursor_mode == CursorMode.CURSOR_ZOOM:
+            self._on_zoom_release(event, is_shift=True)
+        elif self._cursor_mode == CursorMode.CURSOR_PAN:
+            self._on_pan_release(event, is_shift=True)
 
-    def _on_shift_button2_press(self, event):
+    def _on_button2_press(self, event):
         # print("2+")
-        self._on_pan_press(event, clamp=True)
+        self._on_pan_press(event)
 
     def _on_button2_release(self, event):
         # print("2-")
-        self._on_pan_release(event)
+        self._on_pan_release(event, is_shift=False)
+
+    def _on_shift_button2_release(self, event):
+        # print("2-")
+        self._on_pan_release(event, is_shift=True)
 
     def _on_button2_move(self, event):
         # print("B2 move")
-        self._on_pan_move(event)
+        self._on_pan_move(event, is_shift=False)
+
+    def _on_shift_button2_move(self, event):
+        # print("B2 move")
+        self._on_pan_move(event, is_shift=True)
 
     def _on_button3_press(self, _):
         # print("3+")
         if self._state == MouseState.LEFT_DRAGGING:
             self._reset()
 
     def _on_button3_release(self, event):
         # print("3-")
         pass
 
     def _on_button3_move(self, event):
         pass
 
     def _on_wheel(self, event):
-        print("wheel {}".format(event))
+        # print("wheel {}".format(event))
         if event.delta > 0:
             self._wheel_action(event, self._ZOOM_FACTOR, frequency_clamped=False)
         else:
             self._wheel_action(event, 1.0 / self._ZOOM_FACTOR, frequency_clamped=False)
 
     def _on_shift_wheel(self, event):
-        print("shift wheel {}".format(event))
+        # print("shift wheel {}".format(event))
         if event.delta > 0:
             self._wheel_action(event, self._ZOOM_FACTOR, frequency_clamped=True)
         else:
             self._wheel_action(event, 1.0 / self._ZOOM_FACTOR, frequency_clamped=True)
 
     def _on_wheel_up(self, event):
         # print("up {}".format(event))
@@ -196,107 +215,125 @@
         self._canvas.bind('<Shift-Button-4>', self._on_shift_wheel_up)
         self._canvas.bind('<Button-5>', self._on_wheel_down)
         self._canvas.bind('<Shift-Button-5>', self._on_shift_wheel_down)
         # For Windows:
         self._canvas.bind("<MouseWheel>", self._on_wheel)
         self._canvas.bind("<Shift-MouseWheel>", self._on_shift_wheel)
 
-    def _on_zoom_drag_complete(self, start: Tuple[int, int], end: Tuple[int, int], frequency_clamped: bool):
+    def _on_zoom_drag_complete(self, start: Tuple[int, int], end: Tuple[int, int], mode: DragMode):
         """
         * Coordinates provided are relative to the top left corner of the canvas.
         * "start" and "end" are not in any particular order.
         * Coordinates may be outside the range of the canvas, if the drag moves off the edge.
         """
         # print("rectangle selected: {}, {}".format(start, end))
 
         # Order the coordinates ltrb:
         (l, t), (r, b) = start, end
         if t > b:
             t, b = b, t
         if l > r:
             l, r = r, l
 
-        # Sanity check - did they select a tiny area? If so, do nothing.
-        delta = 10
-        if frequency_clamped:
-            if r - l < delta:
-                return
-        else:
-            if r - l < delta or b - t < delta:
-                return
+        if mode == DragMode.DRAG_HORIZONTAL:
+            t, b = 0, self._canvas_height
+        elif mode == DragMode.DRAG_VERTICAL:
+            l, r = 0, self._canvas_width
+        elif mode == DragMode.DRAG_RECTANGLE:
+            pass
 
-        # Notify whoever it concerns that they need to rescale to the area selected:
-        self._graph_frame.on_zoom_to_rect((l, t, r, b), frequency_clamped)
+    # Notify whoever it concerns that they need to rescale to the area selected:
+        self._graph_frame.on_zoom_to_rect((l, t, r, b))
 
     def _reset(self):
         self._state = MouseState.START
         self._start_position = None
+        self._last_drag_mode = None
         self._delete_canvas_items()
 
-    def _on_zoom_press(self, event, clamp: bool):
+    def _on_zoom_press(self, event):
         self._reset()
         self._canvas_height = self._canvas.winfo_height()
+        self._canvas_width = self._canvas.winfo_width()
         self._state = MouseState.LEFT_DRAGGING
         self._start_position = event.x, event.y
-        self._is_frequency_clamped = clamp
-
-    def _on_pan_press(self, event, clamp: bool):
-        self._reset()
-        self._state = MouseState.MIDDLE_DRAGGING
-        self._start_position = event.x, event.y
-        self._is_frequency_clamped = clamp
 
-    def _on_zoom_move(self, event):
+    def _on_zoom_move(self, event, is_shift: bool):
         if self._state == MouseState.LEFT_DRAGGING:
             # If this is not the first move event, we need to delete the previous rectangle we drew:
             self._delete_canvas_items()
-            if self._is_frequency_clamped:
-                self._line1 = self._canvas.create_line(
-                    self._start_position[0], 0, self._start_position[0], self._canvas_height,
-                    fill=DRAG_RECTANGLE_COLOUR)
-                self._line2 = self._canvas.create_line(
-                    event.x, 0, event.x, self._canvas_height,
-                    fill=DRAG_RECTANGLE_COLOUR)
-            else:
-                self._rect = self._canvas.create_rectangle(*self._start_position, event.x, event.y,
-                                                           outline=DRAG_RECTANGLE_COLOUR)
+            mode: DragMode = self._get_drag_mode(event, is_shift)
+            if mode is not None:
+                if mode == DragMode.DRAG_HORIZONTAL:
+                    self._line1 = self._canvas.create_line(
+                        self._start_position[0], 0, self._start_position[0], self._canvas_height,
+                        fill=DRAG_RECTANGLE_COLOUR)
+                    self._line2 = self._canvas.create_line(
+                        event.x, 0, event.x, self._canvas_height,
+                        fill=DRAG_RECTANGLE_COLOUR)
+                elif mode == DragMode.DRAG_VERTICAL:
+                    self._line1 = self._canvas.create_line(
+                        0, self._start_position[1], self._canvas_width, self._start_position[1],
+                        fill=DRAG_RECTANGLE_COLOUR)
+                    self._line2 = self._canvas.create_line(
+                        0, event.y, self._canvas_width, event.y,
+                        fill=DRAG_RECTANGLE_COLOUR)
+                elif mode == DragMode.DRAG_RECTANGLE:
+                    self._rect = self._canvas.create_rectangle(*self._start_position, event.x, event.y,
+                                                               outline=DRAG_RECTANGLE_COLOUR)
 
-    def _on_pan_move(self, event):
-        if self._state == MouseState.MIDDLE_DRAGGING:
-            self._delete_canvas_items()
-            if self._is_frequency_clamped:
-                self._line = self._canvas.create_line(*self._start_position, event.x, self._start_position[1],
-                                                      fill=DRAG_LINE_COLOUR, arrow=tk.LAST, arrowshape=ARROW_SHAPE)
-            else:
-                self._line = self._canvas.create_line(*self._start_position, event.x, event.y,
-                                                      fill=DRAG_LINE_COLOUR, arrow=tk.LAST, arrowshape=ARROW_SHAPE)
-
-    def _on_zoom_release(self, event):
+    def _on_zoom_release(self, event, is_shift: bool):
         self._delete_canvas_items()
         if self._state == MouseState.LEFT_DRAGGING:
             self._state = MouseState.START
-            start = self._start_position
             end = event.x, event.y
+            if self._start_position != end:
+                mode = self._get_drag_mode(event, is_shift)
+                if mode is not None:
+                    self._on_zoom_drag_complete(self._start_position, end, mode)
+
             self._start_position = None
-            if start != end:
-                self._on_zoom_drag_complete(start, end, self._is_frequency_clamped)
 
-    def _on_pan_release(self, event):
+    def _on_pan_press(self, event):
+        self._reset()
+        self._state = MouseState.MIDDLE_DRAGGING
+        self._start_position = event.x, event.y
+
+    def _on_pan_move(self, event, is_shift: bool):
+        if self._state == MouseState.MIDDLE_DRAGGING:
+            self._delete_canvas_items()
+            mode = self._get_drag_mode(event, is_shift)
+            if mode is not None:
+                if mode == DragMode.DRAG_HORIZONTAL:
+                    self._line = self._canvas.create_line(*self._start_position, event.x, self._start_position[1],
+                                                          fill=DRAG_LINE_COLOUR, arrow=tk.LAST, arrowshape=ARROW_SHAPE)
+                elif mode == DragMode.DRAG_VERTICAL:
+                    self._line = self._canvas.create_line(*self._start_position, self._start_position[0], event.y,
+                                                          fill=DRAG_LINE_COLOUR, arrow=tk.LAST, arrowshape=ARROW_SHAPE)
+                else:
+                    self._line = self._canvas.create_line(*self._start_position, event.x, event.y,
+                                                          fill=DRAG_LINE_COLOUR, arrow=tk.LAST, arrowshape=ARROW_SHAPE)
+
+    def _on_pan_release(self, event, is_shift: bool):
         self._delete_canvas_items()
         if self._state == MouseState.MIDDLE_DRAGGING:
             self._state = MouseState.START
             start = self._start_position
-            if self._is_frequency_clamped:
-                end = event.x, start[1]
-            else:
-                end = event.x, event.y
-            self._start_position = None
-            if start != end:
+            mode = self._get_drag_mode(event, is_shift)
+            if mode is not None:
+                if mode == DragMode.DRAG_HORIZONTAL:
+                    end = event.x, start[1]
+                elif mode == DragMode.DRAG_VERTICAL:
+                    end = start[0], event.y
+                else:
+                    end = event.x, event.y
                 self._graph_frame.on_pan((*start, *end))
 
+            self._start_position = None
+
     def set_cursor_mode(self, mode):
         self._cursor_mode = mode
 
     def notify_draw_complete(self):
         # Rebind to wheel events now that outstanding drawing is complete:
         self._bind_wheel()
 
@@ -317,7 +354,40 @@
             self._line1 = None
         if self._line2 is not None:
             self._canvas.delete(self._line2)
             self._line2 = None
         if self._line is not None:
             self._canvas.delete(self._line)
             self._line = None
+
+    def _get_drag_mode(self, event, is_shift: bool) -> DragMode | None:
+        """
+        Decide if frequency or time is clamped, depending on the current direction
+        of the mouse offset.
+        """
+
+        # Holding down shift keeps to the current mode, if there is one:
+        if is_shift and self._last_drag_mode is not None:
+            return self._last_drag_mode
+
+        # Default: drag too small to care about.
+        mode = None
+        minimum = 10
+        threshold = 30
+
+        # _start_position is None once in a while, not sure how that comes about:
+        if self._start_position is not None:
+
+            delta_x = abs(event.x - self._start_position[0])
+            delta_y = abs(event.y - self._start_position[1])
+
+            if delta_x > minimum or delta_y > minimum:
+                if delta_y < threshold:
+                    mode = DragMode.DRAG_HORIZONTAL
+                elif delta_x < threshold:
+                    mode = DragMode.DRAG_VERTICAL
+                else:
+                    mode = DragMode.DRAG_RECTANGLE
+
+            self._last_drag_mode = mode
+
+        return mode
```

### Comparing `batogram-1.0.5/src/batogram/validatingwidgets.py` & `batogram-1.0.6/batogram/validatingwidgets.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.5/src/batogram/wavfileparser.py` & `batogram-1.0.6/batogram/wavfileparser.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.5/src/batogram.egg-info/PKG-INFO` & `batogram-1.0.6/batogram.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batogram
-Version: 1.0.5
+Version: 1.0.6
 Summary: Batogram is a GUI program for rendering spectrograms from full spectrum recordings of bat calls.
 Author-email: John Mears <john+batogram@themears.co.uk>
 License: Copyright (c) 2023 John Mears
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -33,29 +33,47 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 batogram
 ========
 
-Batogram is an open source application for viewing bat calls spectrograms.
+Batogram is an open source application for viewing bat call spectrograms.
 
 Some capabilities and features: 
 * Rendering of spectrograms from .wav files.
 * Auto selection of many parameters for simple operation.
 * Efficient rendering with graceful handling of larger data files.
-* Pan and scale using the mouse or by manual selection.
+* Pan and scale using the mouse, keys or by manual selection.
 * Handling of multichannel data files, including stereo.
 * Basic side by side comparison of two spectrograms.
 * Display of GUANO metadata, including the ability to click to open the location in Google Maps.
-* Runs on Windows, macOS and Linux operating systems.
+* Runs on Windows, Linux and macOS (experimental) operating systems.
 
 Installation
 ------------
 
+### Windows
+
+There are currently two approaches to installing Batogram on Windows. The first and simplest
+method is as follows:
+
+* Download a Batogram executable for Windows from Github. Available releases are listed 
+[here](https://github.com/jmears63/batogram/releases).
+* Probably Windows Defender will warn you of the danger of downloading such files from unknown
+sources. Assess the risk and decide if you going ahead. Assuming you are, proceed to the
+next step.
+* Copy the downloaded executable to your Windows desktop, so that you can find it when you want it.
+* Double click it on the desktop to run it. The first time you run it, it will take a little longer to start 
+up than usual. You will notice a command window launched alongside Batogram - ignore it. This is to
+aid debugging, and will be removed in a future release.
+
+The second installation method is to install Python on your Windows computer, and then follow the 
+same steps as the Linux installation. If you take this route, I assume you know what you are doing.
+
 ### Linux
 
 On Linux, Batogram is currently installed from the command line using pip, as below.
 You need to have Python 3.10 as a minimum.  
 
     # Create a virtual environment at a convenient location in your home directory:
     mkdir ~/batogram
@@ -63,46 +81,24 @@
     python3 -m venv venv
     source venv/bin/activate
 
     # It's good practice to have pip up to date:
     pip install pip --upgrade
 
     # Install batogram and its dependencies. This may take a few moments.
-    # Obviously, substitute the lastest and greatest version number:
-    pip install batogram-x.y.z.tar.gz
+    pip install batogram
     
     # Batogram is now in PATH. You can run it with this simple command:
     batogram
 
-### Windows
-For now, Batogram is installed onto windows using the following slightly convoluted
-steps. At some point in the future, I will provide a simpler install.
-
-This sequence assumes Windows 11.
-
-* Launch the Microsoft Store. You can do this from the Start menu - search for Microsoft Store,
-and launch it.
-* In the store, search for Python using the upper right menu. Select a version which is
-at least 3.10 - probably, the most recent version. I used version 3.11.
-* Go ahead and install it.
-* Open a windows command prompt - for example, by searching for cmd from the start menu. 
-
-In the command prompt, enter this command to install Batogram and its dependencies, which
-may take a few moments:
-
-    pip install batogram
-
-The install command will finish by displaying a path to batogram.exe. You may wish to copy
-that file to your desktop for convenient launching. Otherwise, you can launch
-Batogram from the command prompt:
-
-    python -m batogram
+### macOS (experimental)
 
-Subsequently you can launch Batogram using that command in the command prompt, or by double
-clicking on batogram.exe on your desktop, if you copied it there in the previous step.
+It should be possible to follow the same steps as the Linux installation to install and run
+batogram. However, I am not an expert on Apple products, and don't have any macOS systems to
+test this on.
 
 Usage
 -----
 
 Refer to files in the docs directory for more information. In particular, see
 [batogram.md](docs/batogram.md) for usage notes.
 
@@ -123,19 +119,21 @@
 For the moment, while the structure of the code is fairly rapid flux, so I am not accepting
 pull requests other than for small fixes. This may change in the future.
 
 Credits
 -------
 
 In no particular order:
-* [Pictogrammers Team](https://www.iconarchive.com/show/material-icons-by-pictogrammers/bat-icon.html)
-* [Tucker Beck](https://code.activestate.com/recipes/576688-tooltip-for-tkinter/)
-* [Remix Icon](https://remixicon.com/)
-* [Kenneth Moreland](https://www.kennethmoreland.com/color-advice/)
-* [David A. Riggs](https://github.com/riggsd/guano-py/blob/master/guano.py)
+* [Pictogrammers Team](https://www.iconarchive.com/show/material-icons-by-pictogrammers/bat-icon.html) for the application icon.
+* [Tucker Beck](https://code.activestate.com/recipes/576688-tooltip-for-tkinter/) for tooltip code.
+* [Remix Icon](https://remixicon.com/) for icons.
+* [Kenneth Moreland](https://www.kennethmoreland.com/color-advice/) for colour maps.
+* [David A. Riggs](https://github.com/riggsd/guano-py/blob/master/guano.py) for GUANO code.
+* [Arnold Andreasson](https://github.com/arnoldandreasson) for testing and insights.
+* [Peter Kovesi](https://colorcet.com/index.html) for colour maps.
 
 About the Author
 ----------------
 
 I am John Mears. I obtained a degree in physics in the University of Oxford
 in the distant past. I have spent much of the last 40 years writing software
 relating to scientific and email seccurity applications. In my spare time I cycle,
```

