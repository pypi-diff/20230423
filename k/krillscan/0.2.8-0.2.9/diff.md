# Comparing `tmp/krillscan-0.2.8.tar.gz` & `tmp/krillscan-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krillscan-0.2.8.tar", last modified: Fri Apr 21 14:10:57 2023, max compression
+gzip compressed data, was "krillscan-0.2.9.tar", last modified: Sun Apr 23 13:33:32 2023, max compression
```

## Comparing `krillscan-0.2.8.tar` & `krillscan-0.2.9.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 14:10:57.260922 krillscan-0.2.8/
--rw-rw-rw-   0        0        0     8520 2023-04-21 14:10:57.260922 krillscan-0.2.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-21 14:10:57.102414 krillscan-0.2.8/krillscan/
--rw-rw-rw-   0        0        0      121 2023-04-21 13:49:36.000000 krillscan-0.2.8/krillscan/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:10:57.119049 krillscan-0.2.8/krillscan/echolab2/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:10:57.119049 krillscan-0.2.8/krillscan/echolab2/instruments/
--rw-rw-rw-   0        0        0   159358 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/EK60.py
--rw-rw-rw-   0        0        0   193943 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/EK80.py
--rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/__init__.py
--rw-rw-rw-   0        0        0     3283 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/echosounder.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:10:57.134686 krillscan-0.2.8/krillscan/echolab2/instruments/util/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/util/__init__.py
--rw-rw-rw-   0        0        0     5456 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/util/annotation_data.py
--rw-rw-rw-   0        0        0     8274 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/util/bottom_data.py
--rw-rw-rw-   0        0        0     6783 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/util/date_conversion.py
--rw-rw-rw-   0        0        0     3698 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/util/ek80_datagram_example.py
--rw-rw-rw-   0        0        0     8616 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/util/motion_data.py
--rw-rw-rw-   0        0        0    24904 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/util/nmea_data.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:10:57.151543 krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/
--rw-rw-rw-   0        0        0      410 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/__init__.py
--rw-rw-rw-   0        0        0       23 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/_version.py
--rw-rw-rw-   0        0        0     7181 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/nmea.py
--rw-rw-rw-   0        0        0     2014 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/nmea_file.py
--rw-rw-rw-   0        0        0     3415 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/nmea_utils.py
--rw-rw-rw-   0        0        0      902 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/seatalk_utils.py
--rw-rw-rw-   0        0        0     2050 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/stream.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:10:57.151543 krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/types/
--rw-rw-rw-   0        0        0       85 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:10:57.167169 krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/
--rw-rw-rw-   0        0        0      127 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/__init__.py
--rw-rw-rw-   0        0        0     3937 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/ash.py
--rw-rw-rw-   0        0        0     1382 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/grm.py
--rw-rw-rw-   0        0        0      634 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/rdi.py
--rw-rw-rw-   0        0        0     1196 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/srf.py
--rw-rw-rw-   0        0        0     3675 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/sxn.py
--rw-rw-rw-   0        0        0     3404 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/tnl.py
--rw-rw-rw-   0        0        0     2099 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/ubx.py
--rw-rw-rw-   0        0        0    34150 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/types/talker.py
--rw-rw-rw-   0        0        0     1141 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/util/read_idx_example.py
--rw-rw-rw-   0        0        0    26010 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/util/simrad_calibration.py
--rw-rw-rw-   0        0        0    78275 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/util/simrad_parsers.py
--rw-rw-rw-   0        0        0    21140 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/util/simrad_raw_file.py
--rw-rw-rw-   0        0        0    11377 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/util/simrad_signal_proc.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:10:57.167169 krillscan-0.2.8/krillscan/echolab2/instruments/util/vincenty/
--rw-rw-rw-   0        0        0     3179 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/instruments/util/vincenty/__init__.py
--rw-rw-rw-   0        0        0    67919 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/ping_data.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:10:57.167169 krillscan-0.2.8/krillscan/echolab2/plotting/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/plotting/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:10:57.182793 krillscan-0.2.8/krillscan/echolab2/plotting/matplotlib/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/plotting/matplotlib/__init__.py
--rw-rw-rw-   0        0        0    16178 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/plotting/matplotlib/echogram.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:10:57.182793 krillscan-0.2.8/krillscan/echolab2/plotting/qt/
-drwxrwxrwx   0        0        0        0 2023-04-21 14:10:57.214048 krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/
--rw-rw-rw-   0        0        0    26210 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/QEchogramViewer.py
--rw-rw-rw-   0        0        0    19146 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/QEnhancedImage.py
--rw-rw-rw-   0        0        0    20595 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/QEnhancedImage_threaded.py
--rw-rw-rw-   0        0        0    20668 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/QIVDimensionLine.py
--rw-rw-rw-   0        0        0    15704 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/QIVGrid.py
--rw-rw-rw-   0        0        0     6629 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/QIVHudText.py
--rw-rw-rw-   0        0        0     7732 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/QIVLine.py
--rw-rw-rw-   0        0        0    17957 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/QIVMarker.py
--rw-rw-rw-   0        0        0     7030 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/QIVMarkerText.py
--rw-rw-rw-   0        0        0    13085 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/QIVPolygon.py
--rw-rw-rw-   0        0        0    12899 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/QIVPolygonItem.py
--rw-rw-rw-   0        0        0    12600 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/QIVRubberBandLine.py
--rw-rw-rw-   0        0        0    12009 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/QImageViewer.py
--rw-rw-rw-   0        0        0    12665 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/QImageViewer_threaded.py
--rw-rw-rw-   0        0        0    61143 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/QViewerBase.py
--rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/__init__.py
--rw-rw-rw-   0        0        0     8890 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/imageAdjustmentsDlg.py
--rw-rw-rw-   0        0        0     7787 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/imageAdjustmentsDlg_simple.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:10:57.214048 krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/ui/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/ui/__init__.py
--rw-rw-rw-   0        0        0    17722 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/ui/ui_imageAdjustmentsDlg.py
--rw-rw-rw-   0        0        0    14034 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/ui/ui_imageAdjustmentsDlg_simple.py
--rw-rw-rw-   0        0        0     1615 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/ui/ui_simple.py
--rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/plotting/qt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:10:57.214048 krillscan-0.2.8/krillscan/echolab2/plotting/qt/ui/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/plotting/qt/ui/__init__.py
--rw-rw-rw-   0        0        0     2379 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/plotting/qt/ui/ui_echogram_viewer.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:10:57.229672 krillscan-0.2.8/krillscan/echolab2/processing/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/processing/__init__.py
--rw-rw-rw-   0        0        0    10904 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/processing/afsc_bot_detector.py
--rw-rw-rw-   0        0        0     3347 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/processing/batch_utils.py
--rw-rw-rw-   0        0        0     9669 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/processing/grid.py
--rw-rw-rw-   0        0        0    21422 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/processing/line.py
--rw-rw-rw-   0        0        0    22367 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/processing/mask.py
--rw-rw-rw-   0        0        0    75289 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echolab2/processing/processed_data.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:10:57.260922 krillscan-0.2.8/krillscan/echopy/
--rw-rw-rw-   0        0        0      758 2023-04-21 13:50:02.000000 krillscan-0.2.8/krillscan/echopy/__init__.py
--rw-rw-rw-   0        0        0     1515 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echopy/cmaps.py
--rw-rw-rw-   0        0        0      267 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echopy/correct_absorption.py
--rw-rw-rw-   0        0        0      248 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echopy/correct_es60triangle.py
--rw-rw-rw-   0        0        0      250 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echopy/correct_soundspeed.py
--rw-rw-rw-   0        0        0     3372 2023-04-21 13:50:19.000000 krillscan-0.2.8/krillscan/echopy/get_background.py
--rw-rw-rw-   0        0        0     5966 2023-04-21 13:50:51.000000 krillscan-0.2.8/krillscan/echopy/mask_attenuated.py
--rw-rw-rw-   0        0        0     7763 2023-04-21 13:51:06.000000 krillscan-0.2.8/krillscan/echopy/mask_impulse.py
--rw-rw-rw-   0        0        0     1358 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echopy/mask_multifrequency.py
--rw-rw-rw-   0        0        0     2609 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echopy/mask_range.py
--rw-rw-rw-   0        0        0    21355 2023-04-21 13:51:18.000000 krillscan-0.2.8/krillscan/echopy/mask_seabed.py
--rw-rw-rw-   0        0        0    10771 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echopy/mask_shoals.py
--rw-rw-rw-   0        0        0     2511 2023-04-21 13:51:29.000000 krillscan-0.2.8/krillscan/echopy/mask_signal2noise.py
--rw-rw-rw-   0        0        0      873 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echopy/mask_stationary.py
--rw-rw-rw-   0        0        0     7131 2023-04-21 13:51:37.000000 krillscan-0.2.8/krillscan/echopy/mask_transient.py
--rw-rw-rw-   0        0        0    13405 2023-04-21 13:42:55.000000 krillscan-0.2.8/krillscan/echopy/read_calibration.py
--rw-rw-rw-   0        0        0    17793 2023-04-21 13:50:29.000000 krillscan-0.2.8/krillscan/echopy/resample.py
--rw-rw-rw-   0        0        0     5841 2023-04-21 13:50:38.000000 krillscan-0.2.8/krillscan/echopy/transform.py
--rw-rw-rw-   0        0        0    57079 2023-04-21 14:02:47.000000 krillscan-0.2.8/krillscan/krillscan.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:10:57.119049 krillscan-0.2.8/krillscan.egg-info/
--rw-rw-rw-   0        0        0     8520 2023-04-21 14:10:56.000000 krillscan-0.2.8/krillscan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4821 2023-04-21 14:10:57.000000 krillscan-0.2.8/krillscan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 14:10:56.000000 krillscan-0.2.8/krillscan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-04-21 14:10:56.000000 krillscan-0.2.8/krillscan.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-21 14:10:56.000000 krillscan-0.2.8/krillscan.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 14:10:57.260922 krillscan-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0      890 2023-04-21 14:09:58.000000 krillscan-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 13:33:32.107857 krillscan-0.2.9/
+-rw-rw-rw-   0        0        0     8325 2023-04-23 13:33:32.107857 krillscan-0.2.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-23 13:33:31.938557 krillscan-0.2.9/krillscan/
+-rw-rw-rw-   0        0        0      121 2023-04-21 13:49:36.000000 krillscan-0.2.9/krillscan/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 13:33:31.954179 krillscan-0.2.9/krillscan/echolab2/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 13:33:31.954179 krillscan-0.2.9/krillscan/echolab2/instruments/
+-rw-rw-rw-   0        0        0   159358 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/EK60.py
+-rw-rw-rw-   0        0        0   193943 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/EK80.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/__init__.py
+-rw-rw-rw-   0        0        0     3283 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/echosounder.py
+drwxrwxrwx   0        0        0        0 2023-04-23 13:33:31.985430 krillscan-0.2.9/krillscan/echolab2/instruments/util/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/__init__.py
+-rw-rw-rw-   0        0        0     5456 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/annotation_data.py
+-rw-rw-rw-   0        0        0     8274 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/bottom_data.py
+-rw-rw-rw-   0        0        0     6783 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/date_conversion.py
+-rw-rw-rw-   0        0        0     3698 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/ek80_datagram_example.py
+-rw-rw-rw-   0        0        0     8616 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/motion_data.py
+-rw-rw-rw-   0        0        0    24904 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/nmea_data.py
+drwxrwxrwx   0        0        0        0 2023-04-23 13:33:31.991943 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/
+-rw-rw-rw-   0        0        0      410 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/_version.py
+-rw-rw-rw-   0        0        0     7181 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/nmea.py
+-rw-rw-rw-   0        0        0     2014 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/nmea_file.py
+-rw-rw-rw-   0        0        0     3415 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/nmea_utils.py
+-rw-rw-rw-   0        0        0      902 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/seatalk_utils.py
+-rw-rw-rw-   0        0        0     2050 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/stream.py
+drwxrwxrwx   0        0        0        0 2023-04-23 13:33:31.991943 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/
+-rw-rw-rw-   0        0        0       85 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 13:33:32.007587 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/
+-rw-rw-rw-   0        0        0      127 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/__init__.py
+-rw-rw-rw-   0        0        0     3937 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/ash.py
+-rw-rw-rw-   0        0        0     1382 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/grm.py
+-rw-rw-rw-   0        0        0      634 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/rdi.py
+-rw-rw-rw-   0        0        0     1196 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/srf.py
+-rw-rw-rw-   0        0        0     3675 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/sxn.py
+-rw-rw-rw-   0        0        0     3404 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/tnl.py
+-rw-rw-rw-   0        0        0     2099 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/ubx.py
+-rw-rw-rw-   0        0        0    34150 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/talker.py
+-rw-rw-rw-   0        0        0     1141 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/read_idx_example.py
+-rw-rw-rw-   0        0        0    26010 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/simrad_calibration.py
+-rw-rw-rw-   0        0        0    78275 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/simrad_parsers.py
+-rw-rw-rw-   0        0        0    21140 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/simrad_raw_file.py
+-rw-rw-rw-   0        0        0    11377 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/simrad_signal_proc.py
+drwxrwxrwx   0        0        0        0 2023-04-23 13:33:32.007587 krillscan-0.2.9/krillscan/echolab2/instruments/util/vincenty/
+-rw-rw-rw-   0        0        0     3179 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/instruments/util/vincenty/__init__.py
+-rw-rw-rw-   0        0        0    67919 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/ping_data.py
+drwxrwxrwx   0        0        0        0 2023-04-23 13:33:32.023211 krillscan-0.2.9/krillscan/echolab2/plotting/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 13:33:32.023211 krillscan-0.2.9/krillscan/echolab2/plotting/matplotlib/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/matplotlib/__init__.py
+-rw-rw-rw-   0        0        0    16178 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/matplotlib/echogram.py
+drwxrwxrwx   0        0        0        0 2023-04-23 13:33:32.023211 krillscan-0.2.9/krillscan/echolab2/plotting/qt/
+drwxrwxrwx   0        0        0        0 2023-04-23 13:33:32.054457 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/
+-rw-rw-rw-   0        0        0    26210 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QEchogramViewer.py
+-rw-rw-rw-   0        0        0    19146 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QEnhancedImage.py
+-rw-rw-rw-   0        0        0    20595 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QEnhancedImage_threaded.py
+-rw-rw-rw-   0        0        0    20668 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVDimensionLine.py
+-rw-rw-rw-   0        0        0    15704 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVGrid.py
+-rw-rw-rw-   0        0        0     6629 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVHudText.py
+-rw-rw-rw-   0        0        0     7732 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVLine.py
+-rw-rw-rw-   0        0        0    17957 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVMarker.py
+-rw-rw-rw-   0        0        0     7030 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVMarkerText.py
+-rw-rw-rw-   0        0        0    13085 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVPolygon.py
+-rw-rw-rw-   0        0        0    12899 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVPolygonItem.py
+-rw-rw-rw-   0        0        0    12600 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVRubberBandLine.py
+-rw-rw-rw-   0        0        0    12009 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QImageViewer.py
+-rw-rw-rw-   0        0        0    12665 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QImageViewer_threaded.py
+-rw-rw-rw-   0        0        0    61143 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QViewerBase.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/__init__.py
+-rw-rw-rw-   0        0        0     8890 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/imageAdjustmentsDlg.py
+-rw-rw-rw-   0        0        0     7787 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/imageAdjustmentsDlg_simple.py
+drwxrwxrwx   0        0        0        0 2023-04-23 13:33:32.054457 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/ui/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/ui/__init__.py
+-rw-rw-rw-   0        0        0    17722 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/ui/ui_imageAdjustmentsDlg.py
+-rw-rw-rw-   0        0        0    14034 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/ui/ui_imageAdjustmentsDlg_simple.py
+-rw-rw-rw-   0        0        0     1615 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/ui/ui_simple.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 13:33:32.054457 krillscan-0.2.9/krillscan/echolab2/plotting/qt/ui/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/ui/__init__.py
+-rw-rw-rw-   0        0        0     2379 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/plotting/qt/ui/ui_echogram_viewer.py
+drwxrwxrwx   0        0        0        0 2023-04-23 13:33:32.070084 krillscan-0.2.9/krillscan/echolab2/processing/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/processing/__init__.py
+-rw-rw-rw-   0        0        0    10904 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/processing/afsc_bot_detector.py
+-rw-rw-rw-   0        0        0     3347 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/processing/batch_utils.py
+-rw-rw-rw-   0        0        0     9669 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/processing/grid.py
+-rw-rw-rw-   0        0        0    21422 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/processing/line.py
+-rw-rw-rw-   0        0        0    22367 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/processing/mask.py
+-rw-rw-rw-   0        0        0    75289 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echolab2/processing/processed_data.py
+drwxrwxrwx   0        0        0        0 2023-04-23 13:33:32.107857 krillscan-0.2.9/krillscan/echopy/
+-rw-rw-rw-   0        0        0      758 2023-04-21 13:50:02.000000 krillscan-0.2.9/krillscan/echopy/__init__.py
+-rw-rw-rw-   0        0        0     1515 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echopy/cmaps.py
+-rw-rw-rw-   0        0        0      267 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echopy/correct_absorption.py
+-rw-rw-rw-   0        0        0      248 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echopy/correct_es60triangle.py
+-rw-rw-rw-   0        0        0      250 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echopy/correct_soundspeed.py
+-rw-rw-rw-   0        0        0     3372 2023-04-21 13:50:19.000000 krillscan-0.2.9/krillscan/echopy/get_background.py
+-rw-rw-rw-   0        0        0     5966 2023-04-21 13:50:51.000000 krillscan-0.2.9/krillscan/echopy/mask_attenuated.py
+-rw-rw-rw-   0        0        0     7763 2023-04-21 13:51:06.000000 krillscan-0.2.9/krillscan/echopy/mask_impulse.py
+-rw-rw-rw-   0        0        0     1358 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echopy/mask_multifrequency.py
+-rw-rw-rw-   0        0        0     2609 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echopy/mask_range.py
+-rw-rw-rw-   0        0        0    21355 2023-04-21 13:51:18.000000 krillscan-0.2.9/krillscan/echopy/mask_seabed.py
+-rw-rw-rw-   0        0        0    10771 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echopy/mask_shoals.py
+-rw-rw-rw-   0        0        0     2511 2023-04-21 13:51:29.000000 krillscan-0.2.9/krillscan/echopy/mask_signal2noise.py
+-rw-rw-rw-   0        0        0      873 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echopy/mask_stationary.py
+-rw-rw-rw-   0        0        0     7131 2023-04-21 13:51:37.000000 krillscan-0.2.9/krillscan/echopy/mask_transient.py
+-rw-rw-rw-   0        0        0    13405 2023-04-21 13:42:55.000000 krillscan-0.2.9/krillscan/echopy/read_calibration.py
+-rw-rw-rw-   0        0        0    17793 2023-04-21 13:50:29.000000 krillscan-0.2.9/krillscan/echopy/resample.py
+-rw-rw-rw-   0        0        0     5841 2023-04-21 13:50:38.000000 krillscan-0.2.9/krillscan/echopy/transform.py
+-rw-rw-rw-   0        0        0    57129 2023-04-23 13:30:28.000000 krillscan-0.2.9/krillscan/krillscan.py
+drwxrwxrwx   0        0        0        0 2023-04-23 13:33:31.954179 krillscan-0.2.9/krillscan.egg-info/
+-rw-rw-rw-   0        0        0     8325 2023-04-23 13:33:31.000000 krillscan-0.2.9/krillscan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4821 2023-04-23 13:33:31.000000 krillscan-0.2.9/krillscan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 13:33:31.000000 krillscan-0.2.9/krillscan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-04-23 13:33:31.000000 krillscan-0.2.9/krillscan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-23 13:33:31.000000 krillscan-0.2.9/krillscan.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 13:33:32.107857 krillscan-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      890 2023-04-23 13:32:41.000000 krillscan-0.2.9/setup.py
```

### Comparing `krillscan-0.2.8/PKG-INFO` & `krillscan-0.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krillscan
-Version: 0.2.8
+Version: 0.2.9
 Summary: A python module for automatic analysis of backscatter data from vessels of opportunity
 Home-page: 
 Author: Sebastian Menze
 Author-email: sebastian.menze@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
@@ -16,23 +16,19 @@
 - stores echograms and NASC tables as NetCDF, HDF or .csv files
 - detects krill swarms and can send near-real-time acoustic registrations via email
 
 ![dataflow](dataflow.JPG)
 
 ## Installation
 
-Krillscan was written in python 3.9 and can be run from the source code, from inside a docker container or as compiled executable. We added the compiled **krillscan.exe** to the latest distribution in this repository. To download the krillscan module with python try:
+Krillscan was written in python 3.9 and can be run from the source code, from inside a docker container or as compiled executable. To download the krillscan module with python try:
 ```python
 pip install krillscan
 ```
 
-You will also need to install this library manually and store it into your curent working folder
-
-https://github.com/CI-CMG/pyEcholab
-
 ## Operation
 
 ### Automatic processing
 
 Here I describe how to operate krillscan from inside python, instructions for the docker container are found below. After opening a python prompt and installing krillscan, you need to create or download a settings.ini file that tells krillscan where to look for incoming files and where to store processed data and contains processing and data transfer parameters. The file should be a text files following this pattern: 
 
 ```
@@ -192,9 +188,15 @@
 
 - You can add or remove areas of the detection mask (shown as red overlay) using double clicks to draw a polygon of you choice. Once finished with drawing press enter to apply the change and update the NASC accordingly.
 
 ![fig_inspect](fig_inspect.png)
 
 
 
+## Acknowledgements
+
+
+
+
+
 ## Run krillscan automatic processing from a Docker container
```

### Comparing `krillscan-0.2.8/krillscan/echolab2/instruments/EK60.py` & `krillscan-0.2.9/krillscan/echolab2/instruments/EK60.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/instruments/EK80.py` & `krillscan-0.2.9/krillscan/echolab2/instruments/EK80.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/instruments/echosounder.py` & `krillscan-0.2.9/krillscan/echolab2/instruments/echosounder.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/instruments/util/annotation_data.py` & `krillscan-0.2.9/krillscan/echolab2/instruments/util/annotation_data.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/instruments/util/bottom_data.py` & `krillscan-0.2.9/krillscan/echolab2/instruments/util/bottom_data.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/instruments/util/date_conversion.py` & `krillscan-0.2.9/krillscan/echolab2/instruments/util/date_conversion.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/instruments/util/ek80_datagram_example.py` & `krillscan-0.2.9/krillscan/echolab2/instruments/util/ek80_datagram_example.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/instruments/util/motion_data.py` & `krillscan-0.2.9/krillscan/echolab2/instruments/util/motion_data.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/instruments/util/nmea_data.py` & `krillscan-0.2.9/krillscan/echolab2/instruments/util/nmea_data.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/nmea.py` & `krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/nmea.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/nmea_file.py` & `krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/nmea_file.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/nmea_utils.py` & `krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/nmea_utils.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/seatalk_utils.py` & `krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/seatalk_utils.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/stream.py` & `krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/stream.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/ash.py` & `krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/ash.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/grm.py` & `krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/grm.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/rdi.py` & `krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/rdi.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/srf.py` & `krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/srf.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/sxn.py` & `krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/sxn.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/tnl.py` & `krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/tnl.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/ubx.py` & `krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/ubx.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/instruments/util/pynmea2/types/talker.py` & `krillscan-0.2.9/krillscan/echolab2/instruments/util/pynmea2/types/talker.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/instruments/util/read_idx_example.py` & `krillscan-0.2.9/krillscan/echolab2/instruments/util/read_idx_example.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/instruments/util/simrad_calibration.py` & `krillscan-0.2.9/krillscan/echolab2/instruments/util/simrad_calibration.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/instruments/util/simrad_parsers.py` & `krillscan-0.2.9/krillscan/echolab2/instruments/util/simrad_parsers.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/instruments/util/simrad_raw_file.py` & `krillscan-0.2.9/krillscan/echolab2/instruments/util/simrad_raw_file.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/instruments/util/simrad_signal_proc.py` & `krillscan-0.2.9/krillscan/echolab2/instruments/util/simrad_signal_proc.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/instruments/util/vincenty/__init__.py` & `krillscan-0.2.9/krillscan/echolab2/instruments/util/vincenty/__init__.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/ping_data.py` & `krillscan-0.2.9/krillscan/echolab2/ping_data.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/plotting/matplotlib/echogram.py` & `krillscan-0.2.9/krillscan/echolab2/plotting/matplotlib/echogram.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/QEchogramViewer.py` & `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QEchogramViewer.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/QEnhancedImage.py` & `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QEnhancedImage.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/QEnhancedImage_threaded.py` & `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QEnhancedImage_threaded.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/QIVDimensionLine.py` & `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVDimensionLine.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/QIVGrid.py` & `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVGrid.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/QIVHudText.py` & `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVHudText.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/QIVLine.py` & `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVLine.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/QIVMarker.py` & `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVMarker.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/QIVMarkerText.py` & `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVMarkerText.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/QIVPolygon.py` & `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVPolygon.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/QIVPolygonItem.py` & `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVPolygonItem.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/QIVRubberBandLine.py` & `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QIVRubberBandLine.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/QImageViewer.py` & `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QImageViewer.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/QImageViewer_threaded.py` & `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QImageViewer_threaded.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/QViewerBase.py` & `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/QViewerBase.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/imageAdjustmentsDlg.py` & `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/imageAdjustmentsDlg.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/imageAdjustmentsDlg_simple.py` & `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/imageAdjustmentsDlg_simple.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/ui/ui_imageAdjustmentsDlg.py` & `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/ui/ui_imageAdjustmentsDlg.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/ui/ui_imageAdjustmentsDlg_simple.py` & `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/ui/ui_imageAdjustmentsDlg_simple.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/plotting/qt/QImageViewer/ui/ui_simple.py` & `krillscan-0.2.9/krillscan/echolab2/plotting/qt/QImageViewer/ui/ui_simple.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/plotting/qt/ui/ui_echogram_viewer.py` & `krillscan-0.2.9/krillscan/echolab2/plotting/qt/ui/ui_echogram_viewer.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/processing/afsc_bot_detector.py` & `krillscan-0.2.9/krillscan/echolab2/processing/afsc_bot_detector.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/processing/batch_utils.py` & `krillscan-0.2.9/krillscan/echolab2/processing/batch_utils.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/processing/grid.py` & `krillscan-0.2.9/krillscan/echolab2/processing/grid.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/processing/line.py` & `krillscan-0.2.9/krillscan/echolab2/processing/line.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/processing/mask.py` & `krillscan-0.2.9/krillscan/echolab2/processing/mask.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echolab2/processing/processed_data.py` & `krillscan-0.2.9/krillscan/echolab2/processing/processed_data.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echopy/__init__.py` & `krillscan-0.2.9/krillscan/echopy/__init__.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echopy/cmaps.py` & `krillscan-0.2.9/krillscan/echopy/cmaps.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echopy/get_background.py` & `krillscan-0.2.9/krillscan/echopy/get_background.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echopy/mask_attenuated.py` & `krillscan-0.2.9/krillscan/echopy/mask_attenuated.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echopy/mask_impulse.py` & `krillscan-0.2.9/krillscan/echopy/mask_impulse.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echopy/mask_multifrequency.py` & `krillscan-0.2.9/krillscan/echopy/mask_multifrequency.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echopy/mask_range.py` & `krillscan-0.2.9/krillscan/echopy/mask_range.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echopy/mask_seabed.py` & `krillscan-0.2.9/krillscan/echopy/mask_seabed.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echopy/mask_shoals.py` & `krillscan-0.2.9/krillscan/echopy/mask_shoals.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echopy/mask_signal2noise.py` & `krillscan-0.2.9/krillscan/echopy/mask_signal2noise.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echopy/mask_stationary.py` & `krillscan-0.2.9/krillscan/echopy/mask_stationary.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echopy/mask_transient.py` & `krillscan-0.2.9/krillscan/echopy/mask_transient.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echopy/read_calibration.py` & `krillscan-0.2.9/krillscan/echopy/read_calibration.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echopy/resample.py` & `krillscan-0.2.9/krillscan/echopy/resample.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/echopy/transform.py` & `krillscan-0.2.9/krillscan/echopy/transform.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/krillscan/krillscan.py` & `krillscan-0.2.9/krillscan/krillscan.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,15 +256,15 @@
         
         self.t=[-1,-1]
         self.plotwindow_startsecond=0
         self.plotwindow_length=0
   
         
     def settings_edit(self):
-        os.startfile('settings.ini')    
+        os.startfile(self.ini_file)    
    
                   
     def showfoldefunc(self):    
          os.startfile(self.workpath)
          
     def openfiles_fun(self):
         
@@ -696,25 +696,26 @@
         app = QtWidgets.QApplication(sys.argv)
         app.setApplicationName("Krillscan")    
         app.setStyleSheet(qdarktheme.load_stylesheet())
         w = MainWindow()
         sys.exit(app.exec_())
              
     
-    def start(self):
+    def start(self,ini_file):
         print('start')
+        self.ini_file = ini_file
         self.callback_process_active=False
         self.callback_email_active=False
         # self.callback_plot_active=False
         self.df_files=pd.DataFrame([])
         # self.echogram=pd.DataFrame([])    
         self.positions=pd.DataFrame([])    
         
         config = configparser.ConfigParser()
-        config.read('settings.ini')            
+        config.read(self.ini_file)            
         self.workpath=  str(config['GENERAL']['target_folder'])  
         
         print('work dir: ' +os.getcwd())
         print('source dir: ' + str(config['GENERAL']['source_folder'])  )
         print('target dir: ' +self.workpath)
                
 
@@ -738,15 +739,15 @@
         # df_sv=pd.DataFrame( [] )
         positions=pd.DataFrame( []  )
                 
         # breakpoint()
         
         # print('Echsounder data are: ')
         self.config = configparser.ConfigParser()
-        self.config.read('settings.ini')   
+        self.config.read(self.ini_file)   
         
         # rawfile=r"E:\KRILL-2023\D20230129-T065613.raw"
         # rawfile=r"./source_folder\D20230128-T105149.raw"
    
         try:     
             raw_obj = EK80.EK80()
             raw_obj.read_raw(rawfile)
@@ -907,15 +908,15 @@
         # print(positions)
                
         return xr_sv, positions , xr_sv_raw
 
     def callback_process_raw(self):
               
       config = configparser.ConfigParser()
-      config.read('settings.ini')            
+      config.read(self.ini_file)            
       self.folder_source=  str(config['GENERAL']['source_folder'])  
         
       if (self.callback_process_active==False) :
           
         self.callback_process_active==True
         # self.workpath=  os.path.join(self.folder_source,'krill_data')     
         # os.chdir(self.workpath)
@@ -1106,15 +1107,15 @@
     def detect_krill_swarms(self,xr_sv,positions):
          # sv= self.echodata[rawfile][ 120000.0] 
          # sv= self.ekdata[ 120000.0]          
          # 
          # breakpoint()
          
          config = configparser.ConfigParser()
-         config.read('settings.ini')            
+         config.read(self.ini_file)            
          f=float(config['GENERAL']['scrutinization_frequency'])
                   
          surface_exclusion_depth_m    = float(self.config['PROCESSING']['surface_exclusion_depth_m'] )
          maximum_depth_m    = float(self.config['PROCESSING']['maximum_depth_m'] )
 
          
             
@@ -1263,15 +1264,15 @@
     #     print('start')
 
     def callback_email(self):
       if  (self.callback_email_active==False) :      
         self.callback_email_active==True
         print('checking wether to send email')
         self.config = configparser.ConfigParser()
-        self.config.read('settings.ini')   
+        self.config.read(self.ini_file)   
                 
         emailfrom = self.config['EMAIL']['email_from']
         emailto = self.config['EMAIL']['email_to']
         password = str(self.config['EMAIL']['pw'])
         # fileToSend = r"D20220212-T180420_nasctable.h5"
         # username = "raw2nasc"
         # password = "raw2nasckrill"
@@ -1321,15 +1322,15 @@
                     msg["Subject"] = "Krillscan data from "+ self.config['GENERAL']['vessel_name']+' ' +files_to_send[0][-30:-13]+'_to_'+files_to_send[-1][-30:-13]
                   
                     msgtext = str(dict(self.config['GENERAL']))
                     msg.attach(MIMEText( msgtext   ,'plain'))
     
                     loczip = msg["Subject"]+'.zip'
                     zip = zipfile.ZipFile(loczip, "w", zipfile.ZIP_DEFLATED)
-                    zip.write('settings.ini')
+                    zip.write(self.ini_file)
     
                     for fi in files_to_send:   
                         zip.write(fi,arcname=fi[-30:]  )                                  
     
                     if send_echograms>0:                       
                         for fi in files_to_send:      
                             
@@ -1396,11 +1397,11 @@
                                         
         
         self.callback_email_active==False
         
 #%%
 
 ks=krillscan_class()
-# ks.start()
+# ks.start('settings.ini')
 
 
 # ks.stop()
```

### Comparing `krillscan-0.2.8/krillscan.egg-info/PKG-INFO` & `krillscan-0.2.9/krillscan.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krillscan
-Version: 0.2.8
+Version: 0.2.9
 Summary: A python module for automatic analysis of backscatter data from vessels of opportunity
 Home-page: 
 Author: Sebastian Menze
 Author-email: sebastian.menze@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
@@ -16,23 +16,19 @@
 - stores echograms and NASC tables as NetCDF, HDF or .csv files
 - detects krill swarms and can send near-real-time acoustic registrations via email
 
 ![dataflow](dataflow.JPG)
 
 ## Installation
 
-Krillscan was written in python 3.9 and can be run from the source code, from inside a docker container or as compiled executable. We added the compiled **krillscan.exe** to the latest distribution in this repository. To download the krillscan module with python try:
+Krillscan was written in python 3.9 and can be run from the source code, from inside a docker container or as compiled executable. To download the krillscan module with python try:
 ```python
 pip install krillscan
 ```
 
-You will also need to install this library manually and store it into your curent working folder
-
-https://github.com/CI-CMG/pyEcholab
-
 ## Operation
 
 ### Automatic processing
 
 Here I describe how to operate krillscan from inside python, instructions for the docker container are found below. After opening a python prompt and installing krillscan, you need to create or download a settings.ini file that tells krillscan where to look for incoming files and where to store processed data and contains processing and data transfer parameters. The file should be a text files following this pattern: 
 
 ```
@@ -192,9 +188,15 @@
 
 - You can add or remove areas of the detection mask (shown as red overlay) using double clicks to draw a polygon of you choice. Once finished with drawing press enter to apply the change and update the NASC accordingly.
 
 ![fig_inspect](fig_inspect.png)
 
 
 
+## Acknowledgements
+
+
+
+
+
 ## Run krillscan automatic processing from a Docker container
```

### Comparing `krillscan-0.2.8/krillscan.egg-info/SOURCES.txt` & `krillscan-0.2.9/krillscan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `krillscan-0.2.8/setup.py` & `krillscan-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "readme.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="krillscan",
-    version="0.2.8",
+    version="0.2.9",
     description="A python module for automatic analysis of backscatter data from vessels of opportunity",
     long_description=README,
     long_description_content_type="text/markdown",
     url="",
     author="Sebastian Menze",
     author_email="sebastian.menze@gmail.com",
     classifiers=[
```

