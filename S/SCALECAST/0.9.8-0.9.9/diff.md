# Comparing `tmp/SCALECAST-0.9.8.tar.gz` & `tmp/SCALECAST-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SCALECAST-0.9.8.tar", last modified: Wed May 11 17:16:45 2022, max compression
+gzip compressed data, was "SCALECAST-0.9.9.tar", last modified: Thu May 12 15:26:52 2022, max compression
```

## Comparing `SCALECAST-0.9.8.tar` & `SCALECAST-0.9.9.tar`

### file list

```diff
@@ -1,66 +1,74 @@
-drwxrwxrwx   0        0        0        0 2022-05-11 17:16:44.990992 SCALECAST-0.9.8/
--rw-rw-rw-   0        0        0     5351 2021-08-20 21:51:12.000000 SCALECAST-0.9.8/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0      514 2022-05-06 19:58:00.000000 SCALECAST-0.9.8/Contributing.md
--rw-rw-rw-   0        0        0      113 2021-07-01 20:28:53.000000 SCALECAST-0.9.8/MANIFEST
--rw-rw-rw-   0        0        0     8360 2022-05-11 17:16:45.024032 SCALECAST-0.9.8/PKG-INFO
--rw-rw-rw-   0        0        0     6960 2022-05-10 17:14:01.000000 SCALECAST-0.9.8/README.md
-drwxrwxrwx   0        0        0        0 2022-05-11 17:16:27.571571 SCALECAST-0.9.8/__pycache__/
--rw-rw-rw-   0        0        0    42267 2021-06-18 17:53:02.000000 SCALECAST-0.9.8/__pycache__/Forecaster.cpython-37.pyc
--rw-rw-rw-   0        0        0    49906 2021-06-30 19:52:12.000000 SCALECAST-0.9.8/__pycache__/Forecaster.cpython-38.pyc
--rw-rw-rw-   0        0        0     1336 2021-06-18 17:53:07.000000 SCALECAST-0.9.8/__pycache__/Grids.cpython-37.pyc
--rw-rw-rw-   0        0        0     1222 2021-07-01 17:43:48.000000 SCALECAST-0.9.8/__pycache__/Grids.cpython-38.pyc
-drwxrwxrwx   0        0        0        0 2022-05-11 17:16:29.344573 SCALECAST-0.9.8/assets/
--rw-rw-rw-   0        0        0    34887 2021-08-12 20:39:50.000000 SCALECAST-0.9.8/assets/logo2.png
--rw-rw-rw-   0        0        0    69106 2022-01-10 20:57:42.000000 SCALECAST-0.9.8/assets/main_forecast.png
--rw-rw-rw-   0        0        0    94886 2022-01-10 20:57:23.000000 SCALECAST-0.9.8/assets/main_forecast_test_set.png
-drwxrwxrwx   0        0        0        0 2022-05-11 17:16:32.977191 SCALECAST-0.9.8/docs/
--rw-rw-rw-   0        0        0      101 2022-01-26 03:34:19.000000 SCALECAST-0.9.8/docs/0.17
-drwxrwxrwx   0        0        0        0 2022-05-11 17:16:35.647076 SCALECAST-0.9.8/docs/Forecaster/
-drwxrwxrwx   0        0        0        0 2022-05-11 17:16:35.850203 SCALECAST-0.9.8/docs/Forecaster/.ipynb_checkpoints/
--rw-rw-rw-   0        0        0     7090 2022-05-05 14:29:05.000000 SCALECAST-0.9.8/docs/Forecaster/.ipynb_checkpoints/ForecasterGlobals-checkpoint.ipynb
--rw-rw-rw-   0        0        0      614 2022-03-24 14:32:18.000000 SCALECAST-0.9.8/docs/Forecaster/Forecaster.rst
--rw-rw-rw-   0        0        0     7090 2022-05-05 14:29:05.000000 SCALECAST-0.9.8/docs/Forecaster/ForecasterGlobals.ipynb
--rw-rw-rw-   0        0        0     1247 2022-03-24 19:19:20.000000 SCALECAST-0.9.8/docs/Forecaster/GridGenerator.rst
--rw-rw-rw-   0        0        0     1830 2022-03-24 19:35:11.000000 SCALECAST-0.9.8/docs/Forecaster/MVForecaster.rst
--rw-rw-rw-   0        0        0     1820 2022-03-24 19:19:09.000000 SCALECAST-0.9.8/docs/Forecaster/Multiseries.rst
--rw-rw-rw-   0        0        0     2010 2022-04-15 16:37:18.000000 SCALECAST-0.9.8/docs/Forecaster/Notebook.rst
--rw-rw-rw-   0        0        0     2827 2022-03-24 14:12:07.000000 SCALECAST-0.9.8/docs/Forecaster/_forecast.rst
--rw-rw-rw-   0        0        0        0 2022-01-25 04:28:35.000000 SCALECAST-0.9.8/docs/Forecaster/warnings.log
--rw-rw-rw-   0        0        0      634 2022-01-25 18:18:10.000000 SCALECAST-0.9.8/docs/Makefile
--rw-rw-rw-   0        0        0     4928 2022-05-06 16:23:42.000000 SCALECAST-0.9.8/docs/about.rst
--rw-rw-rw-   0        0        0    21518 2022-05-11 17:00:24.000000 SCALECAST-0.9.8/docs/change_log.md
--rw-rw-rw-   0        0        0     1715 2022-03-31 15:38:57.000000 SCALECAST-0.9.8/docs/conf.py
--rw-rw-rw-   0        0        0     1993 2022-04-04 18:35:40.000000 SCALECAST-0.9.8/docs/index.rst
--rw-rw-rw-   0        0        0     4415 2022-05-06 16:25:26.000000 SCALECAST-0.9.8/docs/initialization.rst
--rw-rw-rw-   0        0        0      809 2022-01-26 22:17:03.000000 SCALECAST-0.9.8/docs/installation.rst
--rwxrwxrwx   0        0        0      795 2022-01-25 18:18:10.000000 SCALECAST-0.9.8/docs/make.bat
--rw-rw-rw-   0        0        0      197 2022-03-25 12:34:51.000000 SCALECAST-0.9.8/docs/requirements.txt
--rw-rw-rw-   0        0        0        0 2022-01-25 15:02:41.000000 SCALECAST-0.9.8/docs/warnings.log
--rw-rw-rw-   0        0        0     1077 2021-06-30 19:58:30.000000 SCALECAST-0.9.8/license.txt
--rw-rw-rw-   0        0        0      115 2022-05-11 17:16:45.119311 SCALECAST-0.9.8/setup.cfg
--rw-rw-rw-   0        0        0     1247 2022-05-06 16:06:40.000000 SCALECAST-0.9.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-05-11 17:16:20.522366 SCALECAST-0.9.8/src/
-drwxrwxrwx   0        0        0        0 2022-05-11 17:16:37.544204 SCALECAST-0.9.8/src/SCALECAST.egg-info/
--rw-rw-rw-   0        0        0     8360 2022-05-11 17:16:00.000000 SCALECAST-0.9.8/src/SCALECAST.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1695 2022-05-11 17:16:19.000000 SCALECAST-0.9.8/src/SCALECAST.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-11 17:16:00.000000 SCALECAST-0.9.8/src/SCALECAST.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      129 2022-05-11 17:16:00.000000 SCALECAST-0.9.8/src/SCALECAST.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-05-11 17:16:00.000000 SCALECAST-0.9.8/src/SCALECAST.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-05-11 17:16:40.600065 SCALECAST-0.9.8/src/scalecast/
--rw-rw-rw-   0        0        0   171311 2022-05-06 21:07:00.000000 SCALECAST-0.9.8/src/scalecast/Forecaster.py
--rw-rw-rw-   0        0        0     3706 2022-04-26 22:01:25.000000 SCALECAST-0.9.8/src/scalecast/GridGenerator.py
--rw-rw-rw-   0        0        0    71853 2022-05-11 16:11:44.000000 SCALECAST-0.9.8/src/scalecast/MVForecaster.py
--rw-rw-rw-   0        0        0       21 2022-05-11 17:15:39.000000 SCALECAST-0.9.8/src/scalecast/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-11 17:16:44.694095 SCALECAST-0.9.8/src/scalecast/__pycache__/
--rw-rw-rw-   0        0        0   142491 2022-04-29 19:14:17.000000 SCALECAST-0.9.8/src/scalecast/__pycache__/Forecaster.cpython-38.pyc
--rw-rw-rw-   0        0        0     3486 2022-03-24 19:45:26.000000 SCALECAST-0.9.8/src/scalecast/__pycache__/GridGenerator.cpython-38.pyc
--rw-rw-rw-   0        0        0     1283 2022-04-05 18:08:37.000000 SCALECAST-0.9.8/src/scalecast/__pycache__/Grids.cpython-38.pyc
--rw-rw-rw-   0        0        0    59742 2022-04-21 13:00:24.000000 SCALECAST-0.9.8/src/scalecast/__pycache__/MVForecaster.cpython-38.pyc
--rw-rw-rw-   0        0        0    51637 2022-03-24 02:48:23.000000 SCALECAST-0.9.8/src/scalecast/__pycache__/MVForecaster_dev_.cpython-38.pyc
--rw-rw-rw-   0        0        0     1096 2022-04-21 13:00:27.000000 SCALECAST-0.9.8/src/scalecast/__pycache__/MVGrids.cpython-38.pyc
--rw-rw-rw-   0        0        0      157 2022-05-11 17:15:59.000000 SCALECAST-0.9.8/src/scalecast/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0     1472 2022-03-24 19:14:43.000000 SCALECAST-0.9.8/src/scalecast/__pycache__/multiseries.cpython-38.pyc
--rw-rw-rw-   0        0        0     5640 2022-03-24 14:24:58.000000 SCALECAST-0.9.8/src/scalecast/__pycache__/notebook.cpython-38.pyc
--rw-rw-rw-   0        0        0     2273 2022-04-05 20:26:54.000000 SCALECAST-0.9.8/src/scalecast/__pycache__/results_vis_mv.cpython-38.pyc
--rw-rw-rw-   0        0        0     1120 2022-03-24 15:09:03.000000 SCALECAST-0.9.8/src/scalecast/multiseries.py
--rw-rw-rw-   0        0        0     8561 2022-04-15 16:34:31.000000 SCALECAST-0.9.8/src/scalecast/notebook.py
+drwxrwxrwx   0        0        0        0 2022-05-12 15:26:52.367512 SCALECAST-0.9.9/
+-rw-rw-rw-   0        0        0     5351 2021-08-20 21:51:12.000000 SCALECAST-0.9.9/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0      514 2022-05-06 19:58:00.000000 SCALECAST-0.9.9/Contributing.md
+-rw-rw-rw-   0        0        0      113 2021-07-01 20:28:53.000000 SCALECAST-0.9.9/MANIFEST
+-rw-rw-rw-   0        0        0    44766 2022-05-12 15:26:52.414387 SCALECAST-0.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0    33905 2022-05-12 15:26:09.000000 SCALECAST-0.9.9/README.md
+drwxrwxrwx   0        0        0        0 2022-05-12 15:26:33.536538 SCALECAST-0.9.9/README_files/
+-rw-rw-rw-   0        0        0    50630 2022-05-12 15:26:09.000000 SCALECAST-0.9.9/README_files/README_17_0.png
+-rw-rw-rw-   0        0        0    47791 2022-05-12 15:26:09.000000 SCALECAST-0.9.9/README_files/README_19_0.png
+-rw-rw-rw-   0        0        0    39445 2022-05-12 15:26:09.000000 SCALECAST-0.9.9/README_files/README_21_0.png
+-rw-rw-rw-   0        0        0   143544 2022-05-12 15:26:09.000000 SCALECAST-0.9.9/README_files/README_39_0.png
+-rw-rw-rw-   0        0        0   133790 2022-05-12 15:26:09.000000 SCALECAST-0.9.9/README_files/README_41_0.png
+-rw-rw-rw-   0        0        0   118751 2022-05-12 15:26:09.000000 SCALECAST-0.9.9/README_files/README_43_0.png
+-rw-rw-rw-   0        0        0    28748 2022-05-12 15:26:09.000000 SCALECAST-0.9.9/README_files/README_50_0.png
+-rw-rw-rw-   0        0        0   118523 2022-05-11 20:20:48.000000 SCALECAST-0.9.9/README_files/README_51_0.png
+-rw-rw-rw-   0        0        0   120955 2022-05-12 15:26:09.000000 SCALECAST-0.9.9/README_files/README_52_0.png
+drwxrwxrwx   0        0        0        0 2022-05-12 15:26:35.101553 SCALECAST-0.9.9/__pycache__/
+-rw-rw-rw-   0        0        0    42267 2021-06-18 17:53:02.000000 SCALECAST-0.9.9/__pycache__/Forecaster.cpython-37.pyc
+-rw-rw-rw-   0        0        0    49906 2021-06-30 19:52:12.000000 SCALECAST-0.9.9/__pycache__/Forecaster.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1336 2021-06-18 17:53:07.000000 SCALECAST-0.9.9/__pycache__/Grids.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1222 2021-07-01 17:43:48.000000 SCALECAST-0.9.9/__pycache__/Grids.cpython-38.pyc
+drwxrwxrwx   0        0        0        0 2022-05-12 15:26:35.710937 SCALECAST-0.9.9/assets/
+-rw-rw-rw-   0        0        0    34887 2021-08-12 20:39:50.000000 SCALECAST-0.9.9/assets/logo2.png
+drwxrwxrwx   0        0        0        0 2022-05-12 15:26:39.175318 SCALECAST-0.9.9/docs/
+-rw-rw-rw-   0        0        0      101 2022-01-26 03:34:19.000000 SCALECAST-0.9.9/docs/0.17
+drwxrwxrwx   0        0        0        0 2022-05-12 15:26:41.684699 SCALECAST-0.9.9/docs/Forecaster/
+drwxrwxrwx   0        0        0        0 2022-05-12 15:26:42.188054 SCALECAST-0.9.9/docs/Forecaster/.ipynb_checkpoints/
+-rw-rw-rw-   0        0        0     7090 2022-05-05 14:29:05.000000 SCALECAST-0.9.9/docs/Forecaster/.ipynb_checkpoints/ForecasterGlobals-checkpoint.ipynb
+-rw-rw-rw-   0        0        0      614 2022-03-24 14:32:18.000000 SCALECAST-0.9.9/docs/Forecaster/Forecaster.rst
+-rw-rw-rw-   0        0        0     7090 2022-05-05 14:29:05.000000 SCALECAST-0.9.9/docs/Forecaster/ForecasterGlobals.ipynb
+-rw-rw-rw-   0        0        0     1247 2022-03-24 19:19:20.000000 SCALECAST-0.9.9/docs/Forecaster/GridGenerator.rst
+-rw-rw-rw-   0        0        0     1830 2022-03-24 19:35:11.000000 SCALECAST-0.9.9/docs/Forecaster/MVForecaster.rst
+-rw-rw-rw-   0        0        0     1820 2022-03-24 19:19:09.000000 SCALECAST-0.9.9/docs/Forecaster/Multiseries.rst
+-rw-rw-rw-   0        0        0     2010 2022-04-15 16:37:18.000000 SCALECAST-0.9.9/docs/Forecaster/Notebook.rst
+-rw-rw-rw-   0        0        0     2827 2022-03-24 14:12:07.000000 SCALECAST-0.9.9/docs/Forecaster/_forecast.rst
+-rw-rw-rw-   0        0        0        0 2022-01-25 04:28:35.000000 SCALECAST-0.9.9/docs/Forecaster/warnings.log
+-rw-rw-rw-   0        0        0      634 2022-01-25 18:18:10.000000 SCALECAST-0.9.9/docs/Makefile
+-rw-rw-rw-   0        0        0     4928 2022-05-06 16:23:42.000000 SCALECAST-0.9.9/docs/about.rst
+-rw-rw-rw-   0        0        0    21728 2022-05-12 15:18:06.000000 SCALECAST-0.9.9/docs/change_log.md
+-rw-rw-rw-   0        0        0     1715 2022-03-31 15:38:57.000000 SCALECAST-0.9.9/docs/conf.py
+-rw-rw-rw-   0        0        0     1993 2022-04-04 18:35:40.000000 SCALECAST-0.9.9/docs/index.rst
+-rw-rw-rw-   0        0        0     4415 2022-05-06 16:25:26.000000 SCALECAST-0.9.9/docs/initialization.rst
+-rw-rw-rw-   0        0        0      809 2022-01-26 22:17:03.000000 SCALECAST-0.9.9/docs/installation.rst
+-rwxrwxrwx   0        0        0      795 2022-01-25 18:18:10.000000 SCALECAST-0.9.9/docs/make.bat
+-rw-rw-rw-   0        0        0      197 2022-03-25 12:34:51.000000 SCALECAST-0.9.9/docs/requirements.txt
+-rw-rw-rw-   0        0        0        0 2022-01-25 15:02:41.000000 SCALECAST-0.9.9/docs/warnings.log
+-rw-rw-rw-   0        0        0     1077 2021-06-30 19:58:30.000000 SCALECAST-0.9.9/license.txt
+-rw-rw-rw-   0        0        0      115 2022-05-12 15:26:52.476887 SCALECAST-0.9.9/setup.cfg
+-rw-rw-rw-   0        0        0     1253 2022-05-11 20:17:45.000000 SCALECAST-0.9.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-05-12 15:26:25.923776 SCALECAST-0.9.9/src/
+drwxrwxrwx   0        0        0        0 2022-05-12 15:26:44.865562 SCALECAST-0.9.9/src/SCALECAST.egg-info/
+-rw-rw-rw-   0        0        0    44766 2022-05-12 15:26:10.000000 SCALECAST-0.9.9/src/SCALECAST.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1897 2022-05-12 15:26:24.000000 SCALECAST-0.9.9/src/SCALECAST.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-05-12 15:26:10.000000 SCALECAST-0.9.9/src/SCALECAST.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      129 2022-05-12 15:26:10.000000 SCALECAST-0.9.9/src/SCALECAST.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2022-05-12 15:26:10.000000 SCALECAST-0.9.9/src/SCALECAST.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-05-12 15:26:48.030997 SCALECAST-0.9.9/src/scalecast/
+-rw-rw-rw-   0        0        0   169742 2022-05-11 18:50:15.000000 SCALECAST-0.9.9/src/scalecast/Forecaster.py
+-rw-rw-rw-   0        0        0     3706 2022-04-26 22:01:25.000000 SCALECAST-0.9.9/src/scalecast/GridGenerator.py
+-rw-rw-rw-   0        0        0    71858 2022-05-11 18:49:47.000000 SCALECAST-0.9.9/src/scalecast/MVForecaster.py
+-rw-rw-rw-   0        0        0       21 2022-05-12 15:18:21.000000 SCALECAST-0.9.9/src/scalecast/__init__.py
+drwxrwxrwx   0        0        0        0 2022-05-12 15:26:52.068470 SCALECAST-0.9.9/src/scalecast/__pycache__/
+-rw-rw-rw-   0        0        0   142491 2022-04-29 19:14:17.000000 SCALECAST-0.9.9/src/scalecast/__pycache__/Forecaster.cpython-38.pyc
+-rw-rw-rw-   0        0        0     3486 2022-03-24 19:45:26.000000 SCALECAST-0.9.9/src/scalecast/__pycache__/GridGenerator.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1283 2022-04-05 18:08:37.000000 SCALECAST-0.9.9/src/scalecast/__pycache__/Grids.cpython-38.pyc
+-rw-rw-rw-   0        0        0    59742 2022-04-21 13:00:24.000000 SCALECAST-0.9.9/src/scalecast/__pycache__/MVForecaster.cpython-38.pyc
+-rw-rw-rw-   0        0        0    51637 2022-03-24 02:48:23.000000 SCALECAST-0.9.9/src/scalecast/__pycache__/MVForecaster_dev_.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1096 2022-04-21 13:00:27.000000 SCALECAST-0.9.9/src/scalecast/__pycache__/MVGrids.cpython-38.pyc
+-rw-rw-rw-   0        0        0      157 2022-05-12 15:19:03.000000 SCALECAST-0.9.9/src/scalecast/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1472 2022-03-24 19:14:43.000000 SCALECAST-0.9.9/src/scalecast/__pycache__/multiseries.cpython-38.pyc
+-rw-rw-rw-   0        0        0     5640 2022-03-24 14:24:58.000000 SCALECAST-0.9.9/src/scalecast/__pycache__/notebook.cpython-38.pyc
+-rw-rw-rw-   0        0        0     2273 2022-04-05 20:26:54.000000 SCALECAST-0.9.9/src/scalecast/__pycache__/results_vis_mv.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1120 2022-03-24 15:09:03.000000 SCALECAST-0.9.9/src/scalecast/multiseries.py
+-rw-rw-rw-   0        0        0     8561 2022-04-15 16:34:31.000000 SCALECAST-0.9.9/src/scalecast/notebook.py
```

### Comparing `SCALECAST-0.9.8/CODE_OF_CONDUCT.md` & `SCALECAST-0.9.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/Contributing.md` & `SCALECAST-0.9.9/Contributing.md`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/__pycache__/Forecaster.cpython-37.pyc` & `SCALECAST-0.9.9/__pycache__/Forecaster.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/__pycache__/Forecaster.cpython-38.pyc` & `SCALECAST-0.9.9/__pycache__/Forecaster.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/__pycache__/Grids.cpython-37.pyc` & `SCALECAST-0.9.9/__pycache__/Grids.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/__pycache__/Grids.cpython-38.pyc` & `SCALECAST-0.9.9/__pycache__/Grids.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/assets/logo2.png` & `SCALECAST-0.9.9/assets/logo2.png`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/docs/Forecaster/.ipynb_checkpoints/ForecasterGlobals-checkpoint.ipynb` & `SCALECAST-0.9.9/docs/Forecaster/.ipynb_checkpoints/ForecasterGlobals-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/docs/Forecaster/Forecaster.rst` & `SCALECAST-0.9.9/docs/Forecaster/Forecaster.rst`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/docs/Forecaster/ForecasterGlobals.ipynb` & `SCALECAST-0.9.9/docs/Forecaster/ForecasterGlobals.ipynb`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/docs/Forecaster/GridGenerator.rst` & `SCALECAST-0.9.9/docs/Forecaster/GridGenerator.rst`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/docs/Forecaster/MVForecaster.rst` & `SCALECAST-0.9.9/docs/Forecaster/MVForecaster.rst`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/docs/Forecaster/Multiseries.rst` & `SCALECAST-0.9.9/docs/Forecaster/Multiseries.rst`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/docs/Forecaster/Notebook.rst` & `SCALECAST-0.9.9/docs/Forecaster/Notebook.rst`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/docs/Forecaster/_forecast.rst` & `SCALECAST-0.9.9/docs/Forecaster/_forecast.rst`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/docs/Makefile` & `SCALECAST-0.9.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/docs/about.rst` & `SCALECAST-0.9.9/docs/about.rst`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/docs/change_log.md` & `SCALECAST-0.9.9/docs/change_log.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 # Changelog
 All notable changes to this project will be documented in this file. We keep track of changes in this file since v0.1.8. The source code for most releases is available on [GitHub](https://github.com/mikekeith52/scalecast).
 
+## [0.9.9] - 2022-05-12
+### Added
+### Changed
+- warning logs now called after `Forecaster` and `MVForecaster` objects are initiated
+- No more `get_funcs()` method, a bad idea from the start
+### Fixed
+
+
 ## [0.9.8] - 2022-05-11
 ### Added
 - added the `corr()` and `corr_lags()` methods to the `MVForecaster` object
 ### Changed
 ### Fixed
 
 ## [0.9.7] - 2022-05-10
```

### Comparing `SCALECAST-0.9.8/docs/conf.py` & `SCALECAST-0.9.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/docs/index.rst` & `SCALECAST-0.9.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/docs/initialization.rst` & `SCALECAST-0.9.9/docs/initialization.rst`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/docs/installation.rst` & `SCALECAST-0.9.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/docs/make.bat` & `SCALECAST-0.9.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/license.txt` & `SCALECAST-0.9.9/license.txt`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/setup.py` & `SCALECAST-0.9.9/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 
 from setuptools import setup, find_packages
 import shutil
 from src.scalecast.__init__ import __version__ as version
+import os
 
-logo = """<p align="center">
-  <img src="https://github.com/mikekeith52/scalecast/blob/main/assets/logo2.png" />
-</p>"""
+if os.path.exists('warnings.log'):
+  os.remove('warnings.log')
+  os.system('jupyter nbconvert --execute --to markdown README.ipynb')
 
-long_description = open('README.md', 'r', encoding="UTF-8").read().replace(logo,"")
+long_description = open('README.md', 'r', encoding="UTF-8").read()
 
 setup(
   name = 'SCALECAST',
   version = version,
   license='MIT',
   description="The practitioner's time series forecasting library",
   long_description=long_description,
```

### Comparing `SCALECAST-0.9.8/src/SCALECAST.egg-info/SOURCES.txt` & `SCALECAST-0.9.9/src/SCALECAST.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 CODE_OF_CONDUCT.md
 Contributing.md
 MANIFEST
 README.md
 license.txt
 setup.cfg
 setup.py
+README_files/README_17_0.png
+README_files/README_19_0.png
+README_files/README_21_0.png
+README_files/README_39_0.png
+README_files/README_41_0.png
+README_files/README_43_0.png
+README_files/README_50_0.png
+README_files/README_51_0.png
+README_files/README_52_0.png
 __pycache__/Forecaster.cpython-37.pyc
 __pycache__/Forecaster.cpython-38.pyc
 __pycache__/Grids.cpython-37.pyc
 __pycache__/Grids.cpython-38.pyc
 assets/logo2.png
-assets/main_forecast.png
-assets/main_forecast_test_set.png
 docs/0.17
 docs/Makefile
 docs/about.rst
 docs/change_log.md
 docs/conf.py
 docs/index.rst
 docs/initialization.rst
```

### Comparing `SCALECAST-0.9.8/src/scalecast/Forecaster.py` & `SCALECAST-0.9.9/src/scalecast/Forecaster.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,18 +24,14 @@
 )
 from statsmodels.tsa.stattools import adfuller
 from statsmodels.graphics.tsaplots import plot_acf, plot_pacf
 from statsmodels.tsa.seasonal import seasonal_decompose
 
 import copy
 
-# LOGGING
-logging.basicConfig(filename="warnings.log", level=logging.WARNING)
-logging.captureWarnings(True)
-
 # sklearn imports below
 from sklearn.linear_model import LinearRegression as mlr_
 from sklearn.neural_network import MLPRegressor as mlp_
 from sklearn.ensemble import GradientBoostingRegressor as gbt_
 from xgboost import XGBRegressor as xgboost_
 from lightgbm import LGBMRegressor as lightgbm_
 from sklearn.ensemble import RandomForestRegressor as rf_
@@ -179,65 +175,14 @@
     "#7FFFD4",
     "#A52A2A",
     "#DCDCDC",
     "#E6E6FA",
     "#BDB76B",
     "#DEB887",
 ] * 10
-_adder_funcs_ = [
-    'add_ar_terms',
-    'add_AR_terms',
-    'add_seasonal_regressors',
-    'add_time_trend',
-    'add_other_regressor',
-    'add_covid19_regressor',
-    'add_combo_regressors',
-    'add_poly_terms',
-    'add_exp_terms',
-    'add_logged_terms',
-    'add_pt_terms',
-    'add_diffed_terms',
-    'add_lagged_terms',
-    'add_sklearn_estimator',
-    'add_cycle',
-]
-_exporter_funcs_ = [
-    'export',
-    'export_summary_stats',
-    'export_feature_importance',
-    'export_validation_grid',
-    'all_feature_info_to_excel',
-    'all_validation_grids_to_excel',
-    'export_Xvars_df',
-    'export_forecasts_with_cis',
-    'export_test_set_preds_with_cis',
-    'export_fitted_vals',
-]
-_setter_funcs_ = [
-    'set_last_future_date',
-    'set_test_length',
-    'set_validation_length',
-    'set_cilevel',
-    'set_bootstrap_samples',
-    'set_estimator',
-    'set_validation_metric',
-]
-_plotter_funcs_ = [
-    'plot_acf',
-    'plot_pacf',
-    'plot_periodogram',
-    'seasonal_decompose',
-    'plot',
-    'plot_test_set',
-    'plot_fitted',
-]
-_getter_funcs_ = [
-    'get_regressor_names',
-    'get_freq',
-]
 _not_hyperparams_ = ["Xvars", "normalizer", "tuned", "plot_loss","plot_loss_test"]
 
 # DESCRIPTIVE ERRORS
 class ForecastError(Exception):
     class CannotDiff(Exception):
         pass
 
@@ -268,14 +213,16 @@
         self.init_dates = list(current_dates)
         self.cilevel = 0.95
         self.bootstrap_samples = 100
         for key, value in kwargs.items():
             setattr(self, key, value)
 
         self.typ_set()  # ensures that the passed values are the right types
+        logging.basicConfig(filename="warnings.log", level=logging.WARNING)
+        logging.captureWarnings(True)
 
     def __copy__(self):
         obj = type(self).__new__(self.__class__)
         obj.__dict__.update(self.__dict__)
         return obj
 
     def __deepcopy__(self):
@@ -324,27 +271,14 @@
             self.validation_length,
             self.validation_metric,
             list(self.history.keys()),
             self.cilevel,
             self.bootstrap_samples,
             None if not hasattr(self,'estimator') else self.estimator)
 
-    def get_funcs(self,which) -> list:
-        """ returns a group of functions based on what's passed to `which`
-        
-        Args:
-            which (str): one of {'adder','exporter','setter','plotter','getter'}
-        
-        Returns:
-            (list): the names of the relevant functions
-
-        >>> f.get_funcs('adder')
-        """
-        return globals()[f'_{which}_funcs_']
-
     def _split_data(self, X, y, test_length, tune):
         X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=test_length, shuffle=False)
         X_test, y_test = (X_test, y_test) if not tune else (X_test[:-self.test_length], y_test[:-self.test_length])
         return X_train, X_test, y_train, y_test
 
     def _validate_no_test_only(self,models):
         descriptive_assert(
```

### Comparing `SCALECAST-0.9.8/src/scalecast/GridGenerator.py` & `SCALECAST-0.9.9/src/scalecast/GridGenerator.py`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/src/scalecast/MVForecaster.py` & `SCALECAST-0.9.9/src/scalecast/MVForecaster.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,18 +19,14 @@
     _normalizer_,
     _determine_best_by_,
     _colors_,
     ForecastError
 )
 import copy
 
-# LOGGING
-logging.basicConfig(filename="warnings.log", level=logging.WARNING)
-logging.captureWarnings(True)
-
 _series_colors_ = [
     '#0000FF',
     '#00FFFF', 
     '#7393B3', 
     '#088F8F', 
     '#0096FF', 
     '#F0FFFF', 
@@ -142,14 +138,17 @@
 
         if names is not None: # checking for these objects is how we know whether user supplied names later
             names = list(names)
             self.name_series_map = {names[i]:[f'series{i+1}',f'y{i+1}'] for i in range(self.n_series)}
             self.y_name_map = {f'y{i+1}':names[i] for i in range(self.n_series)}
             self.series_name_map = {f'series{i+1}':names[i] for i in range(self.n_series)}
 
+        logging.basicConfig(filename="warnings.log", level=logging.WARNING)
+        logging.captureWarnings(True)
+
     def __repr__(self):
         return """MVForecaster(
     DateStartActuals={}
     DateEndActuals={}
     Freq={}
     N_actuals={}
     N_series={}
```

### Comparing `SCALECAST-0.9.8/src/scalecast/__pycache__/Forecaster.cpython-38.pyc` & `SCALECAST-0.9.9/src/scalecast/__pycache__/Forecaster.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/src/scalecast/__pycache__/GridGenerator.cpython-38.pyc` & `SCALECAST-0.9.9/src/scalecast/__pycache__/GridGenerator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/src/scalecast/__pycache__/Grids.cpython-38.pyc` & `SCALECAST-0.9.9/src/scalecast/__pycache__/Grids.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/src/scalecast/__pycache__/MVForecaster.cpython-38.pyc` & `SCALECAST-0.9.9/src/scalecast/__pycache__/MVForecaster.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/src/scalecast/__pycache__/MVForecaster_dev_.cpython-38.pyc` & `SCALECAST-0.9.9/src/scalecast/__pycache__/MVForecaster_dev_.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/src/scalecast/__pycache__/MVGrids.cpython-38.pyc` & `SCALECAST-0.9.9/src/scalecast/__pycache__/MVGrids.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/src/scalecast/__pycache__/multiseries.cpython-38.pyc` & `SCALECAST-0.9.9/src/scalecast/__pycache__/multiseries.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/src/scalecast/__pycache__/notebook.cpython-38.pyc` & `SCALECAST-0.9.9/src/scalecast/__pycache__/notebook.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/src/scalecast/__pycache__/results_vis_mv.cpython-38.pyc` & `SCALECAST-0.9.9/src/scalecast/__pycache__/results_vis_mv.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/src/scalecast/multiseries.py` & `SCALECAST-0.9.9/src/scalecast/multiseries.py`

 * *Files identical despite different names*

### Comparing `SCALECAST-0.9.8/src/scalecast/notebook.py` & `SCALECAST-0.9.9/src/scalecast/notebook.py`

 * *Files identical despite different names*

