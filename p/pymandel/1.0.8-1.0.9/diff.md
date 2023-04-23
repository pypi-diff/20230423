# Comparing `tmp/PyMandel-1.0.8.tar.gz` & `tmp/PyMandel-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMandel-1.0.8.tar", last modified: Sat Feb 25 07:47:38 2023, max compression
+gzip compressed data, was "PyMandel-1.0.9.tar", last modified: Tue Mar  7 23:10:23 2023, max compression
```

## Comparing `PyMandel-1.0.8.tar` & `PyMandel-1.0.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-02-25 07:47:38.469651 PyMandel-1.0.8/
--rw-r--r--   0 steve      (501) staff       (20)    35149 2023-02-24 23:21:44.000000 PyMandel-1.0.8/LICENSE
--rw-r--r--   0 steve      (501) staff       (20)      118 2020-10-18 09:42:00.000000 PyMandel-1.0.8/MANIFEST.in
--rw-r--r--   0 steve      (501) staff       (20)    16969 2023-02-25 07:47:38.469482 PyMandel-1.0.8/PKG-INFO
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-02-25 07:47:38.464599 PyMandel-1.0.8/PyMandel.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)    16969 2023-02-25 07:47:38.000000 PyMandel-1.0.8/PyMandel.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)     1084 2023-02-25 07:47:38.000000 PyMandel-1.0.8/PyMandel.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2023-02-25 07:47:38.000000 PyMandel-1.0.8/PyMandel.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)      135 2023-02-25 07:47:38.000000 PyMandel-1.0.8/PyMandel.egg-info/entry_points.txt
--rw-r--r--   0 steve      (501) staff       (20)       42 2023-02-25 07:47:38.000000 PyMandel-1.0.8/PyMandel.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)       19 2023-02-25 07:47:38.000000 PyMandel-1.0.8/PyMandel.egg-info/top_level.txt
--rw-r--r--   0 steve      (501) staff       (20)    15849 2023-02-24 23:27:53.000000 PyMandel-1.0.8/README.md
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-02-25 07:47:38.466397 PyMandel-1.0.8/colormaps/
--rw-r--r--   0 steve      (501) staff       (20)        0 2020-04-27 13:37:21.000000 PyMandel-1.0.8/colormaps/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)    17382 2021-03-02 16:24:31.000000 PyMandel-1.0.8/colormaps/cet_colormap.py
--rw-r--r--   0 steve      (501) staff       (20)     6408 2021-12-20 14:06:01.000000 PyMandel-1.0.8/colormaps/hsv256_colormap.py
--rw-r--r--   0 steve      (501) staff       (20)     4444 2021-03-02 16:41:52.000000 PyMandel-1.0.8/colormaps/landscape256_colormap.py
--rw-r--r--   0 steve      (501) staff       (20)     2915 2021-05-11 10:54:55.000000 PyMandel-1.0.8/colormaps/make_colormap.py
--rw-r--r--   0 steve      (501) staff       (20)     4388 2021-03-02 16:42:32.000000 PyMandel-1.0.8/colormaps/metallic256_colormap.py
--rw-r--r--   0 steve      (501) staff       (20)     3581 2021-03-02 16:40:25.000000 PyMandel-1.0.8/colormaps/mymap_colormap.py
--rw-r--r--   0 steve      (501) staff       (20)     4661 2021-03-02 16:42:32.000000 PyMandel-1.0.8/colormaps/pastels256_colormap.py
--rw-r--r--   0 steve      (501) staff       (20)     4764 2021-03-02 16:25:36.000000 PyMandel-1.0.8/colormaps/tropical_colormap.py
--rw-r--r--   0 steve      (501) staff       (20)     4346 2021-03-02 16:42:32.000000 PyMandel-1.0.8/colormaps/twilight256_colormap.py
--rw-r--r--   0 steve      (501) staff       (20)    12489 2021-12-20 14:17:37.000000 PyMandel-1.0.8/colormaps/twilights512_colormap.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-02-25 07:47:38.468603 PyMandel-1.0.8/pymandel/
--rw-r--r--   0 steve      (501) staff       (20)      187 2021-03-01 09:14:24.000000 PyMandel-1.0.8/pymandel/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)     1027 2023-02-24 23:21:44.000000 PyMandel-1.0.8/pymandel/__main__.py
--rw-r--r--   0 steve      (501) staff       (20)       23 2023-02-25 07:40:35.000000 PyMandel-1.0.8/pymandel/_version.py
--rw-r--r--   0 steve      (501) staff       (20)     4336 2023-02-24 23:24:53.000000 PyMandel-1.0.8/pymandel/about_dialog.py
--rw-r--r--   0 steve      (501) staff       (20)     5089 2023-02-24 23:21:44.000000 PyMandel-1.0.8/pymandel/app.py
--rw-r--r--   0 steve      (501) staff       (20)    19476 2023-02-24 23:21:44.000000 PyMandel-1.0.8/pymandel/fractal_frame.py
--rw-r--r--   0 steve      (501) staff       (20)     2694 2023-02-24 23:24:54.000000 PyMandel-1.0.8/pymandel/howto_dialog.py
--rw-r--r--   0 steve      (501) staff       (20)    12371 2023-02-25 07:44:48.000000 PyMandel-1.0.8/pymandel/mandelbrot.py
--rw-r--r--   0 steve      (501) staff       (20)     8145 2023-02-24 23:24:54.000000 PyMandel-1.0.8/pymandel/mandelcli.py
--rw-r--r--   0 steve      (501) staff       (20)     3800 2023-02-24 23:24:54.000000 PyMandel-1.0.8/pymandel/menu_bar.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-02-25 07:47:38.469058 PyMandel-1.0.8/pymandel/resources/
--rw-r--r--   0 steve      (501) staff       (20)    68454 2020-04-24 07:44:07.000000 PyMandel-1.0.8/pymandel/resources/pymandel.ico
--rw-r--r--   0 steve      (501) staff       (20)    77618 2020-04-24 07:43:36.000000 PyMandel-1.0.8/pymandel/resources/pymandel.png
--rw-r--r--   0 steve      (501) staff       (20)     8249 2020-04-03 08:02:51.000000 PyMandel-1.0.8/pymandel/resources/thumbnail.gif
--rw-r--r--   0 steve      (501) staff       (20)    27379 2023-02-24 23:24:54.000000 PyMandel-1.0.8/pymandel/settings_frame.py
--rw-r--r--   0 steve      (501) staff       (20)     1845 2023-02-24 23:24:54.000000 PyMandel-1.0.8/pymandel/status_frame.py
--rw-r--r--   0 steve      (501) staff       (20)     5181 2023-02-24 23:35:10.000000 PyMandel-1.0.8/pymandel/strings.py
--rw-r--r--   0 steve      (501) staff       (20)     4972 2023-02-24 23:35:10.000000 PyMandel-1.0.8/pymandel/stringsDE.py
--rw-r--r--   0 steve      (501) staff       (20)     4497 2023-02-24 23:35:10.000000 PyMandel-1.0.8/pymandel/stringsEN.py
--rw-r--r--   0 steve      (501) staff       (20)     4858 2023-02-24 23:35:10.000000 PyMandel-1.0.8/pymandel/stringsES.py
--rw-r--r--   0 steve      (501) staff       (20)     5131 2023-02-24 23:35:10.000000 PyMandel-1.0.8/pymandel/stringsFR.py
--rw-r--r--   0 steve      (501) staff       (20)       38 2023-02-25 07:47:38.469696 PyMandel-1.0.8/setup.cfg
--rw-r--r--   0 steve      (501) staff       (20)     2452 2023-02-24 23:35:47.000000 PyMandel-1.0.8/setup.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-02-25 07:47:38.469291 PyMandel-1.0.8/tests/
--rw-r--r--   0 steve      (501) staff       (20)      470 2021-05-13 10:18:58.000000 PyMandel-1.0.8/tests/test_static.py
--rw-r--r--   0 steve      (501) staff       (20)     1363 2021-05-13 10:20:29.000000 PyMandel-1.0.8/tests/testsuite.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-03-07 23:10:23.408689 PyMandel-1.0.9/
+-rw-r--r--   0 steve      (501) staff       (20)    35149 2023-02-24 23:21:44.000000 PyMandel-1.0.9/LICENSE
+-rw-r--r--   0 steve      (501) staff       (20)      118 2020-10-18 09:42:00.000000 PyMandel-1.0.9/MANIFEST.in
+-rw-r--r--   0 steve      (501) staff       (20)    16978 2023-03-07 23:10:23.408507 PyMandel-1.0.9/PKG-INFO
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-03-07 23:10:23.402339 PyMandel-1.0.9/PyMandel.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)    16978 2023-03-07 23:10:23.000000 PyMandel-1.0.9/PyMandel.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)     1084 2023-03-07 23:10:23.000000 PyMandel-1.0.9/PyMandel.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2023-03-07 23:10:23.000000 PyMandel-1.0.9/PyMandel.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)      135 2023-03-07 23:10:23.000000 PyMandel-1.0.9/PyMandel.egg-info/entry_points.txt
+-rw-r--r--   0 steve      (501) staff       (20)       42 2023-03-07 23:10:23.000000 PyMandel-1.0.9/PyMandel.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)       19 2023-03-07 23:10:23.000000 PyMandel-1.0.9/PyMandel.egg-info/top_level.txt
+-rw-r--r--   0 steve      (501) staff       (20)    15858 2023-03-07 23:10:13.000000 PyMandel-1.0.9/README.md
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-03-07 23:10:23.404065 PyMandel-1.0.9/colormaps/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2020-04-27 13:37:21.000000 PyMandel-1.0.9/colormaps/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)    17382 2021-03-02 16:24:31.000000 PyMandel-1.0.9/colormaps/cet_colormap.py
+-rw-r--r--   0 steve      (501) staff       (20)     6408 2021-12-20 14:06:01.000000 PyMandel-1.0.9/colormaps/hsv256_colormap.py
+-rw-r--r--   0 steve      (501) staff       (20)     4444 2021-03-02 16:41:52.000000 PyMandel-1.0.9/colormaps/landscape256_colormap.py
+-rw-r--r--   0 steve      (501) staff       (20)     3292 2023-03-07 23:10:13.000000 PyMandel-1.0.9/colormaps/make_colormap.py
+-rw-r--r--   0 steve      (501) staff       (20)     4388 2021-03-02 16:42:32.000000 PyMandel-1.0.9/colormaps/metallic256_colormap.py
+-rw-r--r--   0 steve      (501) staff       (20)     3581 2021-03-02 16:40:25.000000 PyMandel-1.0.9/colormaps/mymap_colormap.py
+-rw-r--r--   0 steve      (501) staff       (20)     4661 2021-03-02 16:42:32.000000 PyMandel-1.0.9/colormaps/pastels256_colormap.py
+-rw-r--r--   0 steve      (501) staff       (20)     4764 2021-03-02 16:25:36.000000 PyMandel-1.0.9/colormaps/tropical_colormap.py
+-rw-r--r--   0 steve      (501) staff       (20)     4346 2021-03-02 16:42:32.000000 PyMandel-1.0.9/colormaps/twilight256_colormap.py
+-rw-r--r--   0 steve      (501) staff       (20)    12489 2021-12-20 14:17:37.000000 PyMandel-1.0.9/colormaps/twilights512_colormap.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-03-07 23:10:23.407407 PyMandel-1.0.9/pymandel/
+-rw-r--r--   0 steve      (501) staff       (20)      824 2023-03-07 23:10:13.000000 PyMandel-1.0.9/pymandel/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)     1029 2023-03-07 23:10:13.000000 PyMandel-1.0.9/pymandel/__main__.py
+-rw-r--r--   0 steve      (501) staff       (20)       70 2023-03-07 23:10:13.000000 PyMandel-1.0.9/pymandel/_version.py
+-rw-r--r--   0 steve      (501) staff       (20)     4317 2023-03-07 23:10:13.000000 PyMandel-1.0.9/pymandel/about_dialog.py
+-rw-r--r--   0 steve      (501) staff       (20)     5086 2023-03-07 23:10:13.000000 PyMandel-1.0.9/pymandel/app.py
+-rw-r--r--   0 steve      (501) staff       (20)    19418 2023-03-07 23:10:13.000000 PyMandel-1.0.9/pymandel/fractal_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)     2675 2023-03-07 23:10:13.000000 PyMandel-1.0.9/pymandel/howto_dialog.py
+-rw-r--r--   0 steve      (501) staff       (20)    12380 2023-03-07 23:10:13.000000 PyMandel-1.0.9/pymandel/mandelbrot.py
+-rw-r--r--   0 steve      (501) staff       (20)     9442 2023-03-07 23:10:13.000000 PyMandel-1.0.9/pymandel/mandelcli.py
+-rw-r--r--   0 steve      (501) staff       (20)     3799 2023-03-07 23:10:13.000000 PyMandel-1.0.9/pymandel/menu_bar.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-03-07 23:10:23.407914 PyMandel-1.0.9/pymandel/resources/
+-rw-r--r--   0 steve      (501) staff       (20)    68454 2020-04-24 07:44:07.000000 PyMandel-1.0.9/pymandel/resources/pymandel.ico
+-rw-r--r--   0 steve      (501) staff       (20)    77618 2020-04-24 07:43:36.000000 PyMandel-1.0.9/pymandel/resources/pymandel.png
+-rw-r--r--   0 steve      (501) staff       (20)     8249 2020-04-03 08:02:51.000000 PyMandel-1.0.9/pymandel/resources/thumbnail.gif
+-rw-r--r--   0 steve      (501) staff       (20)    27415 2023-03-07 23:10:13.000000 PyMandel-1.0.9/pymandel/settings_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)     1844 2023-03-07 23:10:13.000000 PyMandel-1.0.9/pymandel/status_frame.py
+-rw-r--r--   0 steve      (501) staff       (20)     5180 2023-03-07 23:10:13.000000 PyMandel-1.0.9/pymandel/strings.py
+-rw-r--r--   0 steve      (501) staff       (20)     4972 2023-02-24 23:35:10.000000 PyMandel-1.0.9/pymandel/stringsDE.py
+-rw-r--r--   0 steve      (501) staff       (20)     4497 2023-02-24 23:35:10.000000 PyMandel-1.0.9/pymandel/stringsEN.py
+-rw-r--r--   0 steve      (501) staff       (20)     4858 2023-02-24 23:35:10.000000 PyMandel-1.0.9/pymandel/stringsES.py
+-rw-r--r--   0 steve      (501) staff       (20)     5131 2023-02-24 23:35:10.000000 PyMandel-1.0.9/pymandel/stringsFR.py
+-rw-r--r--   0 steve      (501) staff       (20)       38 2023-03-07 23:10:23.408736 PyMandel-1.0.9/setup.cfg
+-rw-r--r--   0 steve      (501) staff       (20)     2452 2023-02-24 23:35:47.000000 PyMandel-1.0.9/setup.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-03-07 23:10:23.408201 PyMandel-1.0.9/tests/
+-rw-r--r--   0 steve      (501) staff       (20)      470 2021-05-13 10:18:58.000000 PyMandel-1.0.9/tests/test_static.py
+-rw-r--r--   0 steve      (501) staff       (20)     1363 2021-05-13 10:20:29.000000 PyMandel-1.0.9/tests/testsuite.py
```

### Comparing `PyMandel-1.0.8/LICENSE` & `PyMandel-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PyMandel-1.0.8/PKG-INFO` & `PyMandel-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMandel
-Version: 1.0.8
+Version: 1.0.9
 Summary: PyMandel Fractal Generator Application
 Home-page: https://github.com/semuconsulting/PyMandel
 Author: semuadmin
 Author-email: semuadmin@semuconsulting.com
 License: GPLv3 License
 Project-URL: Bug Tracker, https://github.com/semuconsulting/PyMandel
 Project-URL: Documentation, https://github.com/semuconsulting/PyMandel
@@ -287,19 +287,19 @@
 ## Command Line Utilities
 
 ### mandelcli.py
 
 `pymandelcli` is a command line equivalent to the GUI's Animate function. If PyMandel has been installed using `pip` and the Python 3 scripts (bin) directory is in the user's PATH, it can be invoked thus:
 
 ```shell
-pymandelcli width=480 height=480 frames=20
+pymandelcli --width 480 --height 480 --frames 20
 ``` 
-This will produce a sequence of 20 .png images. Pass `-h` or `-help` for a list of available parameters.
+This will produce a sequence of 20 .png images. Type `pymandelcli -h` for a list of available parameters.
 
-It can import settings from a previously saved metadata file using the import parameter e.g. `import=filename.json`.
+It can import settings from a previously saved metadata file using the import parameter e.g. `--import filename.json`.
 
 In addition to producing animated sequences, the command line utility can be used to create single images at a much higher pixel resolution than would be available via the GUI application on a standard monitor, though render time may be significant.
 
 ** Suggestion ** Use the PyMandel GUI at moderate resolutions to explore fractals and find a location and configuration you like, save the image & metadata, and then use the `pymandelcli` command line utility to import the metadata and create a much higher resolution version of the same image e.g for desktop wallpaper, printing or sharing.
 
 ### make_colormap.py
```

### Comparing `PyMandel-1.0.8/PyMandel.egg-info/PKG-INFO` & `PyMandel-1.0.9/PyMandel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMandel
-Version: 1.0.8
+Version: 1.0.9
 Summary: PyMandel Fractal Generator Application
 Home-page: https://github.com/semuconsulting/PyMandel
 Author: semuadmin
 Author-email: semuadmin@semuconsulting.com
 License: GPLv3 License
 Project-URL: Bug Tracker, https://github.com/semuconsulting/PyMandel
 Project-URL: Documentation, https://github.com/semuconsulting/PyMandel
@@ -287,19 +287,19 @@
 ## Command Line Utilities
 
 ### mandelcli.py
 
 `pymandelcli` is a command line equivalent to the GUI's Animate function. If PyMandel has been installed using `pip` and the Python 3 scripts (bin) directory is in the user's PATH, it can be invoked thus:
 
 ```shell
-pymandelcli width=480 height=480 frames=20
+pymandelcli --width 480 --height 480 --frames 20
 ``` 
-This will produce a sequence of 20 .png images. Pass `-h` or `-help` for a list of available parameters.
+This will produce a sequence of 20 .png images. Type `pymandelcli -h` for a list of available parameters.
 
-It can import settings from a previously saved metadata file using the import parameter e.g. `import=filename.json`.
+It can import settings from a previously saved metadata file using the import parameter e.g. `--import filename.json`.
 
 In addition to producing animated sequences, the command line utility can be used to create single images at a much higher pixel resolution than would be available via the GUI application on a standard monitor, though render time may be significant.
 
 ** Suggestion ** Use the PyMandel GUI at moderate resolutions to explore fractals and find a location and configuration you like, save the image & metadata, and then use the `pymandelcli` command line utility to import the metadata and create a much higher resolution version of the same image e.g for desktop wallpaper, printing or sharing.
 
 ### make_colormap.py
```

### Comparing `PyMandel-1.0.8/PyMandel.egg-info/SOURCES.txt` & `PyMandel-1.0.9/PyMandel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyMandel-1.0.8/README.md` & `PyMandel-1.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -252,19 +252,19 @@
 ## Command Line Utilities
 
 ### mandelcli.py
 
 `pymandelcli` is a command line equivalent to the GUI's Animate function. If PyMandel has been installed using `pip` and the Python 3 scripts (bin) directory is in the user's PATH, it can be invoked thus:
 
 ```shell
-pymandelcli width=480 height=480 frames=20
+pymandelcli --width 480 --height 480 --frames 20
 ``` 
-This will produce a sequence of 20 .png images. Pass `-h` or `-help` for a list of available parameters.
+This will produce a sequence of 20 .png images. Type `pymandelcli -h` for a list of available parameters.
 
-It can import settings from a previously saved metadata file using the import parameter e.g. `import=filename.json`.
+It can import settings from a previously saved metadata file using the import parameter e.g. `--import filename.json`.
 
 In addition to producing animated sequences, the command line utility can be used to create single images at a much higher pixel resolution than would be available via the GUI application on a standard monitor, though render time may be significant.
 
 ** Suggestion ** Use the PyMandel GUI at moderate resolutions to explore fractals and find a location and configuration you like, save the image & metadata, and then use the `pymandelcli` command line utility to import the metadata and create a much higher resolution version of the same image e.g for desktop wallpaper, printing or sharing.
 
 ### make_colormap.py
```

### Comparing `PyMandel-1.0.8/colormaps/cet_colormap.py` & `PyMandel-1.0.9/colormaps/cet_colormap.py`

 * *Files identical despite different names*

### Comparing `PyMandel-1.0.8/colormaps/hsv256_colormap.py` & `PyMandel-1.0.9/colormaps/hsv256_colormap.py`

 * *Files identical despite different names*

### Comparing `PyMandel-1.0.8/colormaps/landscape256_colormap.py` & `PyMandel-1.0.9/colormaps/landscape256_colormap.py`

 * *Files identical despite different names*

### Comparing `PyMandel-1.0.8/colormaps/make_colormap.py` & `PyMandel-1.0.9/colormaps/make_colormap.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 #!/usr/bin/env python
 """
 Command line utility to create numpy color map arrays suitable for use by PyMandel
 from image files containing suitable color gradients e.g. created using GIMP's gradient tool.
 It currently only handles RGB or RGBA formats.
 
-make_colormap mapname=mymap input=mymap.png output=mymap_colormap.py levels=256
+make_colormap --mapname mymap --input mymap.png --output mymap_colormap.py --levels 256
 
 Created on 24 Apr 2020
 
 :author: semuadmin
 :copyright: SEMU Consulting 2020
 :license: BSD 3-Clause
 """
 
 import sys
-
+from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter, SUPPRESS
 from PIL import Image
+from pymandel._version import __version__ as VERSION
+
+EPILOG = (
+    "© 2021 SEMU Consulting GPLv3 license - https://github.com/semuconsulting/PyMandel/"
+)
 
 
 def make_colormap(**kwargs):
     """
     Scan image file and create array of rgb values
 
     :param kwargs: optional keyword args
@@ -41,15 +46,15 @@
         print(f"Invalid image mode {mode} - must be RGB or RGBA")
 
     levels = int(kwargs.get("levels", image.width))
     if levels > image.width:
         levels = image.width
     outfile = kwargs.get("output", mapname + str(levels) + "_colormap.py")
 
-    file = open(outfile, "a")
+    file = open(outfile, "a", encoding="utf-8")
     file.write("from numpy import array\n\n")
     file.write(
         "#****************************************************************************************\n"
         f"# {str(levels)}-level colormap created by make_colormap utility from file {infile}\n"
         "#****************************************************************************************\n"
     )
     file.write(mapname + " = array([ \\\n")
@@ -70,24 +75,27 @@
 
     image.close()
     file.close()
 
     print(str(levels) + "-level colormap file " + outfile + " created")
 
 
-def main(args=None):
-    """ CLI entry point. """
+def main():
+    """CLI entry point."""
 
-    if len(sys.argv) > 1:
-        if sys.argv[1] in {"-h", "--h", "help", "-help", "--help", "-H"}:
-            print(
-                " make_colormap.py is a simple command line utility to create",
-                "a numpy RGB colormap suitable for importing into PyMandel.\n\n",
-                "Usage: make_colormap mapname=mymap input=mymap.png output=mymap_colormap.py levels=256",
-            )
-            sys.exit()
+    arp = ArgumentParser(
+        epilog=EPILOG,
+        formatter_class=ArgumentDefaultsHelpFormatter,
+        argument_default=SUPPRESS,
+    )
+    arp.add_argument("-V", "--version", action="version", version="%(prog)s " + VERSION)
+    arp.add_argument("--mapname", help="Map name", default="mymap")
+    arp.add_argument("--input", help="Input image filename", default="mymap.png")
+    arp.add_argument("--levels", help="Color levels", type=int, default=256)
+    arp.add_argument("--output", help="Output filename", default="mymap_colormap.py")
 
-    make_colormap(**dict(arg.split("=") for arg in sys.argv[1:]))
+    kwargs = vars(arp.parse_args())
+    make_colormap(**kwargs)
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PyMandel-1.0.8/colormaps/metallic256_colormap.py` & `PyMandel-1.0.9/colormaps/metallic256_colormap.py`

 * *Files identical despite different names*

### Comparing `PyMandel-1.0.8/colormaps/mymap_colormap.py` & `PyMandel-1.0.9/colormaps/mymap_colormap.py`

 * *Files identical despite different names*

### Comparing `PyMandel-1.0.8/colormaps/pastels256_colormap.py` & `PyMandel-1.0.9/colormaps/pastels256_colormap.py`

 * *Files identical despite different names*

### Comparing `PyMandel-1.0.8/colormaps/tropical_colormap.py` & `PyMandel-1.0.9/colormaps/tropical_colormap.py`

 * *Files identical despite different names*

### Comparing `PyMandel-1.0.8/colormaps/twilight256_colormap.py` & `PyMandel-1.0.9/colormaps/twilight256_colormap.py`

 * *Files identical despite different names*

### Comparing `PyMandel-1.0.8/colormaps/twilights512_colormap.py` & `PyMandel-1.0.9/colormaps/twilights512_colormap.py`

 * *Files identical despite different names*

### Comparing `PyMandel-1.0.8/pymandel/__main__.py` & `PyMandel-1.0.9/pymandel/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,21 +5,24 @@
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: GPL3
 
 This file is part of PyMandel.
 
-PyMandel is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License
-as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+PyMandel is free software: you can redistribute it and/or modify it under the terms of the
+GNU General Public License as published by the Free Software Foundation, either version 3
+of the License, or (at your option) any later version.
+
+PyMandel is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
+without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+See the GNU General Public License for more details.
 
-PyMandel is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
-of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along with PyMandel. If not, see <https://www.gnu.org/licenses/>. 
+You should have received a copy of the GNU General Public License along with PyMandel.
+If not, see <https://www.gnu.org/licenses/>.
 """
 
 import sys
 from tkinter import Tk
 from pymandel.app import App
```

### Comparing `PyMandel-1.0.8/pymandel/about_dialog.py` & `PyMandel-1.0.9/pymandel/about_dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,24 @@
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: GPL3
 
 This file is part of PyMandel.
 
-PyMandel is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License
-as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+PyMandel is free software: you can redistribute it and/or modify it under the terms of the
+GNU General Public License as published by the Free Software Foundation, either version 3
+of the License, or (at your option) any later version.
+
+PyMandel is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
+without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+See the GNU General Public License for more details.
 
-PyMandel is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
-of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along with PyMandel. If not, see <https://www.gnu.org/licenses/>. 
+You should have received a copy of the GNU General Public License along with PyMandel.
+If not, see <https://www.gnu.org/licenses/>.
 """
 
 import os
 from platform import python_version
 from tkinter import Toplevel, Canvas, Label, Button, PhotoImage, NW
 from webbrowser import open_new_tab
 from numba import __version__ as numba_ver
@@ -53,16 +56,15 @@
         """
 
         self.__app = app  # Reference to main application class
         self.__master = self.__app.get_master()  # Reference to root class (Tk)
         self._dialog = Toplevel()
         self._dialog.title = DLGABOUT
         self._dialog.geometry(
-            "+%d+%d"
-            % (self.__master.winfo_rootx() + 50, self.__master.winfo_rooty() + 50)
+            f"+{self.__master.winfo_rootx() + 50}+{self.__master.winfo_rooty() + 50}"
         )
         self._dialog.attributes("-topmost", "true")
 
         self.body()
 
     def body(self):
         """
```

### Comparing `PyMandel-1.0.8/pymandel/app.py` & `PyMandel-1.0.9/pymandel/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,24 @@
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: GPL3
 
 This file is part of PyMandel.
 
-PyMandel is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License
-as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+PyMandel is free software: you can redistribute it and/or modify it under the terms of the
+GNU General Public License as published by the Free Software Foundation, either version 3
+of the License, or (at your option) any later version.
+
+PyMandel is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
+without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+See the GNU General Public License for more details.
 
-PyMandel is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
-of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along with PyMandel. If not, see <https://www.gnu.org/licenses/>. 
+You should have received a copy of the GNU General Public License along with PyMandel.
+If not, see <https://www.gnu.org/licenses/>.
 """
 
 import os
 from tkinter import N, S, E, W, PhotoImage
 
 from pymandel.about_dialog import AboutDialog
 from pymandel.fractal_frame import FractalFrame
@@ -122,19 +125,19 @@
 
     def toggle_axes(self):
         """
         Toggle plot axes on or off
         """
 
         if self._show_axes:
-            self.frm_fractal._show_axes = False
+            self.frm_fractal.show_axes = False
             self._show_axes = False
             self.menu.option_menu.entryconfig(7, label=MENUSHOWAX)
         else:
-            self.frm_fractal._show_axes = True
+            self.frm_fractal.show_axes = True
             self._show_axes = True
             self.menu.option_menu.entryconfig(7, label=MENUHIDEAX)
 
     def set_status(self, message, color="black"):
         """
         Sets text of status bar
         """
```

### Comparing `PyMandel-1.0.8/pymandel/fractal_frame.py` & `PyMandel-1.0.9/pymandel/fractal_frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,24 @@
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: GPL3
 
 This file is part of PyMandel.
 
-PyMandel is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License
-as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+PyMandel is free software: you can redistribute it and/or modify it under the terms of the
+GNU General Public License as published by the Free Software Foundation, either version 3
+of the License, or (at your option) any later version.
+
+PyMandel is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
+without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+See the GNU General Public License for more details.
 
-PyMandel is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
-of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along with PyMandel. If not, see <https://www.gnu.org/licenses/>. 
+You should have received a copy of the GNU General Public License along with PyMandel.
+If not, see <https://www.gnu.org/licenses/>.
 """
 
 from cmath import polar
 from math import sqrt, log, pi, sin, cos
 from platform import system
 from time import time
 from tkinter import Frame, Canvas, NW, BOTH, YES
@@ -72,15 +75,15 @@
         Frame.__init__(self, self.__master, *args, **kwargs)
 
         self._fractal = None  # Must be instance variable to persist after use
         self._animating = False
         self._setmode = MANDELBROT
         self._setvar = STANDARD
         self._leftclickmode = ZOOMIN
-        self._show_axes = False
+        self.show_axes = False
         self._zoom_rect = None
         self._x_start = None
         self._y_start = None
         self._xaxis = self._yaxis = 0
 
         self.mandelbrot = None
 
@@ -175,15 +178,15 @@
             cy_off,
         )
         self._fractal = ImageTk.PhotoImage(self.mandelbrot.get_image())
         self.can_fractal.create_image(
             0, 0, image=self._fractal, state="normal", anchor=NW
         )
 
-        if self._show_axes:
+        if self.show_axes:
             self.axes(width, height)
         self.can_fractal.update()
 
         if (
             not self.mandelbrot.get_cancel() and not self._animating
         ):  # If plot wasn't cancelled
             end = time()
@@ -403,24 +406,22 @@
         Windows platforms)
         """
 
         if event.keysym == "Shift_L":
             self._leftclickmode = ZOOMOUT
             self.can_fractal.config(cursor="sizing")
 
-        if event.keysym == "Alt_L" or event.keysym == "Control_L":
+        if event.keysym in ("Alt_L", "Control_L"):
             self._leftclickmode = GOJULIA
             self._setmode = JULIA
             self.can_fractal.config(cursor="target")
 
         # Pressing Left or Right button in Julia mode will rotate the Julia Set clockwise
         # or anti-clockwise about its origin
-        if (
-            event.keysym == "Left" or event.keysym == "Right"
-        ) and self._setmode == JULIA:
+        if (event.keysym in ("Left", "Right")) and self._setmode == JULIA:
             if event.keysym == "Left":
                 self.rotate_julia(0.01)
             else:
                 self.rotate_julia(-0.01)
 
             self.plot()
 
@@ -564,15 +565,15 @@
             self.can_fractal.update()
 
             if animatemode == SPIN:  # Spinning Julia animation
                 self.rotate_julia((1 / frames) * 2 * pi)
 
             self.plot()
 
-            if self._show_axes:
+            if self.show_axes:
                 self.axes(width, height)
             self.can_fractal.update()
 
             if self.mandelbrot.get_cancel():
                 return
 
             if settings.get("autosave"):
```

### Comparing `PyMandel-1.0.8/pymandel/howto_dialog.py` & `PyMandel-1.0.9/pymandel/howto_dialog.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,21 +5,24 @@
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: GPL3
 
 This file is part of PyMandel.
 
-PyMandel is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License
-as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+PyMandel is free software: you can redistribute it and/or modify it under the terms of the
+GNU General Public License as published by the Free Software Foundation, either version 3
+of the License, or (at your option) any later version.
+
+PyMandel is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
+without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+See the GNU General Public License for more details.
 
-PyMandel is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
-of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along with PyMandel. If not, see <https://www.gnu.org/licenses/>. 
+You should have received a copy of the GNU General Public License along with PyMandel.
+If not, see <https://www.gnu.org/licenses/>.
 """
 
 from tkinter import Toplevel, Label, Button, LEFT
 from webbrowser import open_new_tab
 
 from pymandel.strings import HELPTXT, COPYRIGHTTXT, DLGHOWTO, GITHUBURL
 
@@ -35,16 +38,15 @@
         """
 
         self.__app = app  # Reference to main application class
         self.__master = self.__app.get_master()  # Reference to root class (Tk)
         self._dialog = Toplevel()
         self._dialog.title = DLGHOWTO
         self._dialog.geometry(
-            "+%d+%d"
-            % (self.__master.winfo_rootx() + 50, self.__master.winfo_rooty() + 50)
+            f"+{self.__master.winfo_rootx() + 50}+{self.__master.winfo_rooty() + 50}"
         )
         self._dialog.attributes("-topmost", "true")
 
         self.body()
 
     def body(self):
         """
```

### Comparing `PyMandel-1.0.8/pymandel/mandelbrot.py` & `PyMandel-1.0.9/pymandel/mandelbrot.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,21 +12,24 @@
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: GPL3
 
 This file is part of PyMandel.
 
-PyMandel is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License
-as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+PyMandel is free software: you can redistribute it and/or modify it under the terms of the
+GNU General Public License as published by the Free Software Foundation, either version 3
+of the License, or (at your option) any later version.
+
+PyMandel is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
+without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+See the GNU General Public License for more details.
 
-PyMandel is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
-of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along with PyMandel. If not, see <https://www.gnu.org/licenses/>. 
+You should have received a copy of the GNU General Public License along with PyMandel.
+If not, see <https://www.gnu.org/licenses/>.
 """
 # pylint: disable=invalid-name
 
 from math import log, sin, sqrt, pi, floor, ceil
 
 from PIL import Image
 from numba import jit, prange
@@ -144,14 +147,15 @@
     Calculates fractal escape scalars i, za for each image pixel
     and returns them for use in color rendering routines.
     """
 
     zx_coord, zy_coord = ptoc(width, height, x_axis, y_axis, zxoff, zyoff, zoom)
     lastz = complex(0, 0)
     per = 0
+    i = 0
 
     z = complex(zx_coord, zy_coord)
     if settype == JULIA:  # Julia or variant
         c = complex(cxoff, cyoff)
     else:  # Mandelbrot or variant
         c = z
```

### Comparing `PyMandel-1.0.8/pymandel/menu_bar.py` & `PyMandel-1.0.9/pymandel/menu_bar.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,24 @@
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: GPL3
 
 This file is part of PyMandel.
 
-PyMandel is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License
-as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+PyMandel is free software: you can redistribute it and/or modify it under the terms of the
+GNU General Public License as published by the Free Software Foundation, either version 3
+of the License, or (at your option) any later version.
+
+PyMandel is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
+without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+See the GNU General Public License for more details.
 
-PyMandel is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
-of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along with PyMandel. If not, see <https://www.gnu.org/licenses/>. 
+You should have received a copy of the GNU General Public License along with PyMandel.
+If not, see <https://www.gnu.org/licenses/>.
 """
 
 from tkinter import Menu
 
 from pymandel.strings import (
     MENUFILE,
     MENUOPTIONS,
```

### Comparing `PyMandel-1.0.8/pymandel/resources/pymandel.ico` & `PyMandel-1.0.9/pymandel/resources/pymandel.ico`

 * *Files identical despite different names*

### Comparing `PyMandel-1.0.8/pymandel/resources/pymandel.png` & `PyMandel-1.0.9/pymandel/resources/pymandel.png`

 * *Files identical despite different names*

### Comparing `PyMandel-1.0.8/pymandel/resources/thumbnail.gif` & `PyMandel-1.0.9/pymandel/resources/thumbnail.gif`

 * *Files identical despite different names*

### Comparing `PyMandel-1.0.8/pymandel/settings_frame.py` & `PyMandel-1.0.9/pymandel/settings_frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,21 +7,24 @@
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: GPL3
 
 This file is part of PyMandel.
 
-PyMandel is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License
-as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+PyMandel is free software: you can redistribute it and/or modify it under the terms of the
+GNU General Public License as published by the Free Software Foundation, either version 3
+of the License, or (at your option) any later version.
+
+PyMandel is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
+without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+See the GNU General Public License for more details.
 
-PyMandel is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
-of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along with PyMandel. If not, see <https://www.gnu.org/licenses/>. 
+You should have received a copy of the GNU General Public License along with PyMandel.
+If not, see <https://www.gnu.org/licenses/>.
 """
 
 from tkinter import (
     ttk,
     Frame,
     Button,
     Label,
@@ -575,15 +578,15 @@
             return False
 
     def is_filename(self, flag):
         """
         Validate if entry represents a valid filename using a regexp.
         """
 
-        return match("^[\w\-. ]+$", flag) and flag != ""
+        return match(r"^[\w\-. ]+$", flag) and flag != ""
 
     def reset(self):
         """
         Reset settings to defaults.
         """
 
         self._settype.set(MODES[0])
@@ -794,15 +797,15 @@
                 "cyoffset": self._cy_off.get(),
                 "theme": self._theme.get(),
                 "shift": self._shift.get(),
             }
         }
 
         try:
-            with open(filename, "w") as outfile:
+            with open(filename, "w", encoding="utf-8") as outfile:
                 dump(jsondata, outfile)
         except OSError:
             self.__app.set_status(METASAVEERROR, "red")
             self._filepath = None
 
         # Return focus to image frame
         self.__app.frm_fractal.focus_set()
@@ -818,15 +821,15 @@
             filepath = filedialog.askopenfilename(
                 initialdir=default,
                 title=SELTITLE,
                 filetypes=(("json files", "*.json"), ("all files", "*.*")),
             )
             if filepath == "":  # User cancelled
                 return
-            with open(filepath, "r") as infile:
+            with open(filepath, "r", encoding="utf-8") as infile:
                 jsondata = infile.read()
         except OSError:
             self.__app.set_status(OPENFILEERROR, "red")
             return
 
         # Parse file
         try:
```

### Comparing `PyMandel-1.0.8/pymandel/status_frame.py` & `PyMandel-1.0.9/pymandel/status_frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,24 @@
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: GPL3
 
 This file is part of PyMandel.
 
-PyMandel is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License
-as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+PyMandel is free software: you can redistribute it and/or modify it under the terms of the
+GNU General Public License as published by the Free Software Foundation, either version 3
+of the License, or (at your option) any later version.
+
+PyMandel is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
+without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+See the GNU General Public License for more details.
 
-PyMandel is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
-of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along with PyMandel. If not, see <https://www.gnu.org/licenses/>. 
+You should have received a copy of the GNU General Public License along with PyMandel.
+If not, see <https://www.gnu.org/licenses/>.
 """
 
 from tkinter import Frame, Label, StringVar, W, E
 
 
 class StatusFrame(Frame):
     """
```

### Comparing `PyMandel-1.0.8/pymandel/strings.py` & `PyMandel-1.0.9/pymandel/strings.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,21 +5,24 @@
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: GPL3
 
 This file is part of PyMandel.
 
-PyMandel is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License
-as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+PyMandel is free software: you can redistribute it and/or modify it under the terms of the
+GNU General Public License as published by the Free Software Foundation, either version 3
+of the License, or (at your option) any later version.
+
+PyMandel is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
+without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+See the GNU General Public License for more details.
 
-PyMandel is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty
-of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along with PyMandel. If not, see <https://www.gnu.org/licenses/>. 
+You should have received a copy of the GNU General Public License along with PyMandel.
+If not, see <https://www.gnu.org/licenses/>.
 """
 # pylint: disable=line-too-long
 
 WIKIURL = "https://en.wikipedia.org/wiki/Mandelbrot_set"
 GITHUBURL = "https://github.com/semuconsulting/PyMandel"
 CETURL = "https://github.com/holoviz/colorcet/blob/master/LICENSE.txt"
 MODULENAME = "pymandel"
```

### Comparing `PyMandel-1.0.8/pymandel/stringsDE.py` & `PyMandel-1.0.9/pymandel/stringsDE.py`

 * *Files identical despite different names*

### Comparing `PyMandel-1.0.8/pymandel/stringsEN.py` & `PyMandel-1.0.9/pymandel/stringsEN.py`

 * *Files identical despite different names*

### Comparing `PyMandel-1.0.8/pymandel/stringsES.py` & `PyMandel-1.0.9/pymandel/stringsES.py`

 * *Files identical despite different names*

### Comparing `PyMandel-1.0.8/pymandel/stringsFR.py` & `PyMandel-1.0.9/pymandel/stringsFR.py`

 * *Files identical despite different names*

### Comparing `PyMandel-1.0.8/setup.py` & `PyMandel-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `PyMandel-1.0.8/tests/testsuite.py` & `PyMandel-1.0.9/tests/testsuite.py`

 * *Files identical despite different names*

