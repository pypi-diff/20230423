# Comparing `tmp/cc12703_uiautomator2-2.7.2.tar.gz` & `tmp/cc12703_uiautomator2-2.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cc12703_uiautomator2-2.7.2.tar", last modified: Thu Feb 23 04:02:01 2023, max compression
+gzip compressed data, was "dist/cc12703_uiautomator2-2.7.3.tar", last modified: Tue Feb 28 02:50:49 2023, max compression
```

## Comparing `cc12703_uiautomator2-2.7.2.tar` & `cc12703_uiautomator2-2.7.3.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-23 04:02:01.000000 cc12703_uiautomator2-2.7.2/
--rw-r--r--   0 runner    (1001) docker     (116)       59 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/ABOUT.rst
--rw-r--r--   0 runner    (1001) docker     (116)      227 2023-02-23 04:02:01.000000 cc12703_uiautomator2-2.7.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (116)    23774 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (116)      376 2023-02-23 04:02:01.000000 cc12703_uiautomator2-2.7.2/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (116)      639 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/DEVELOP.md
--rw-r--r--   0 runner    (1001) docker     (116)     1064 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      167 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)      737 2023-02-23 04:02:01.000000 cc12703_uiautomator2-2.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2375 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/QUICK_REFERENCE.md
--rw-r--r--   0 runner    (1001) docker     (116)    56078 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (116)    10682 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/XPATH.md
--rw-r--r--   0 runner    (1001) docker     (116)     1593 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/appveyor.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-23 04:02:01.000000 cc12703_uiautomator2-2.7.2/cc12703_uiautomator2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      737 2023-02-23 04:02:01.000000 cc12703_uiautomator2-2.7.2/cc12703_uiautomator2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1852 2023-02-23 04:02:01.000000 cc12703_uiautomator2-2.7.2/cc12703_uiautomator2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-23 04:02:01.000000 cc12703_uiautomator2-2.7.2/cc12703_uiautomator2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       61 2023-02-23 04:02:01.000000 cc12703_uiautomator2-2.7.2/cc12703_uiautomator2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-23 04:01:56.000000 cc12703_uiautomator2-2.7.2/cc12703_uiautomator2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       47 2023-02-23 04:02:01.000000 cc12703_uiautomator2-2.7.2/cc12703_uiautomator2.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (116)      296 2023-02-23 04:02:01.000000 cc12703_uiautomator2-2.7.2/cc12703_uiautomator2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       13 2023-02-23 04:02:01.000000 cc12703_uiautomator2-2.7.2/cc12703_uiautomator2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      232 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)      812 2023-02-23 04:02:01.000000 cc12703_uiautomator2-2.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      158 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-23 04:02:01.000000 cc12703_uiautomator2-2.7.2/uiautomator2/
--rw-r--r--   0 runner    (1001) docker     (116)    70764 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8106 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)      289 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/_proto.py
--rw-r--r--   0 runner    (1001) docker     (116)    21311 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/_selector.py
--rw-r--r--   0 runner    (1001) docker     (116)      643 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/abcd.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-23 04:02:01.000000 cc12703_uiautomator2-2.7.2/uiautomator2/assets/
--rw-r--r--   0 runner    (1001) docker     (116)        6 2023-02-23 04:01:24.000000 cc12703_uiautomator2-2.7.2/uiautomator2/assets/apk_version.txt
--rw-r--r--   0 runner    (1001) docker     (116)  1061950 2023-02-23 04:01:24.000000 cc12703_uiautomator2-2.7.2/uiautomator2/assets/app-uiautomator-test.apk
--rw-r--r--   0 runner    (1001) docker     (116)  2191186 2023-02-23 04:01:24.000000 cc12703_uiautomator2-2.7.2/uiautomator2/assets/app-uiautomator.apk
--rwxr-xr-x   0 runner    (1001) docker     (116)      570 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/assets/sync.sh
--rw-r--r--   0 runner    (1001) docker     (116)     2643 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-23 04:02:01.000000 cc12703_uiautomator2-2.7.2/uiautomator2/ext/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-23 04:02:01.000000 cc12703_uiautomator2-2.7.2/uiautomator2/ext/htmlreport/
--rw-r--r--   0 runner    (1001) docker     (116)      405 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/ext/htmlreport/README.md
--rw-r--r--   0 runner    (1001) docker     (116)     5572 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/ext/htmlreport/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-23 04:02:01.000000 cc12703_uiautomator2-2.7.2/uiautomator2/ext/htmlreport/assets/
--rw-r--r--   0 runner    (1001) docker     (116)     4802 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/ext/htmlreport/assets/index.html
--rw-r--r--   0 runner    (1001) docker     (116)    61137 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/ext/htmlreport/assets/pig.jpg
--rw-r--r--   0 runner    (1001) docker     (116)     1190 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/ext/htmlreport/assets/simplehttpserver.py
--rw-r--r--   0 runner    (1001) docker     (116)       29 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/ext/htmlreport/assets/start.bat
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-23 04:02:01.000000 cc12703_uiautomator2-2.7.2/uiautomator2/ext/info/
--rw-r--r--   0 runner    (1001) docker     (116)     2645 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/ext/info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    28515 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/ext/info/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-23 04:02:01.000000 cc12703_uiautomator2-2.7.2/uiautomator2/ext/perf/
--rw-r--r--   0 runner    (1001) docker     (116)     2852 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/ext/perf/README.md
--rw-r--r--   0 runner    (1001) docker     (116)    12382 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/ext/perf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    41467 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/ext/perf/net.png
--rw-r--r--   0 runner    (1001) docker     (116)    26928 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/ext/perf/summary.png
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-23 04:02:01.000000 cc12703_uiautomator2-2.7.2/uiautomator2/ext/xpath/
--rw-r--r--   0 runner    (1001) docker     (116)       88 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/ext/xpath/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      227 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/ext/xpath/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-23 04:02:01.000000 cc12703_uiautomator2-2.7.2/uiautomator2/ext-archived/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-23 04:02:01.000000 cc12703_uiautomator2-2.7.2/uiautomator2/ext-archived/aircv/
--rw-r--r--   0 runner    (1001) docker     (116)     4180 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/ext-archived/aircv/README.md
--rw-r--r--   0 runner    (1001) docker     (116)    18456 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/ext-archived/aircv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-23 04:02:01.000000 cc12703_uiautomator2-2.7.2/uiautomator2/ext-archived/ocr/
--rw-r--r--   0 runner    (1001) docker     (116)      947 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/ext-archived/ocr/README.md
--rw-r--r--   0 runner    (1001) docker     (116)     2494 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/ext-archived/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3307 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/ext-archived/ocr/baiduOCR.py
--rw-r--r--   0 runner    (1001) docker     (116)    10564 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/image.py
--rw-r--r--   0 runner    (1001) docker     (116)    15113 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/init.py
--rw-r--r--   0 runner    (1001) docker     (116)     1801 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/messagebox.py
--rw-r--r--   0 runner    (1001) docker     (116)     3776 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/screenrecord.py
--rw-r--r--   0 runner    (1001) docker     (116)     3507 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/settings.py
--rw-r--r--   0 runner    (1001) docker     (116)     1761 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/swipe.py
--rw-r--r--   0 runner    (1001) docker     (116)     6086 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     4900 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/version.py
--rw-r--r--   0 runner    (1001) docker     (116)     9758 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/watcher.py
--rw-r--r--   0 runner    (1001) docker     (116)     6703 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/webview.py
--rw-r--r--   0 runner    (1001) docker     (116)    14506 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/widget.py
--rw-r--r--   0 runner    (1001) docker     (116)    28843 2023-02-23 04:01:23.000000 cc12703_uiautomator2-2.7.2/uiautomator2/xpath.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-28 02:50:49.000000 cc12703_uiautomator2-2.7.3/
+-rw-r--r--   0 runner    (1001) docker     (116)       59 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/ABOUT.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      206 2023-02-28 02:50:49.000000 cc12703_uiautomator2-2.7.3/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (116)    23774 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (116)      371 2023-02-28 02:50:49.000000 cc12703_uiautomator2-2.7.3/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (116)      639 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/DEVELOP.md
+-rw-r--r--   0 runner    (1001) docker     (116)     1064 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      167 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)      737 2023-02-28 02:50:49.000000 cc12703_uiautomator2-2.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2375 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/QUICK_REFERENCE.md
+-rw-r--r--   0 runner    (1001) docker     (116)    56078 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)    10682 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/XPATH.md
+-rw-r--r--   0 runner    (1001) docker     (116)     1593 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/appveyor.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-28 02:50:49.000000 cc12703_uiautomator2-2.7.3/cc12703_uiautomator2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      737 2023-02-28 02:50:49.000000 cc12703_uiautomator2-2.7.3/cc12703_uiautomator2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1852 2023-02-28 02:50:49.000000 cc12703_uiautomator2-2.7.3/cc12703_uiautomator2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-28 02:50:49.000000 cc12703_uiautomator2-2.7.3/cc12703_uiautomator2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       61 2023-02-28 02:50:49.000000 cc12703_uiautomator2-2.7.3/cc12703_uiautomator2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-28 02:50:44.000000 cc12703_uiautomator2-2.7.3/cc12703_uiautomator2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)       47 2023-02-28 02:50:49.000000 cc12703_uiautomator2-2.7.3/cc12703_uiautomator2.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (116)      296 2023-02-28 02:50:49.000000 cc12703_uiautomator2-2.7.3/cc12703_uiautomator2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       13 2023-02-28 02:50:49.000000 cc12703_uiautomator2-2.7.3/cc12703_uiautomator2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      232 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      812 2023-02-28 02:50:49.000000 cc12703_uiautomator2-2.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      158 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-28 02:50:49.000000 cc12703_uiautomator2-2.7.3/uiautomator2/
+-rw-r--r--   0 runner    (1001) docker     (116)    70813 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8106 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      289 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/_proto.py
+-rw-r--r--   0 runner    (1001) docker     (116)    21311 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/_selector.py
+-rw-r--r--   0 runner    (1001) docker     (116)      643 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/abcd.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-28 02:50:49.000000 cc12703_uiautomator2-2.7.3/uiautomator2/assets/
+-rw-r--r--   0 runner    (1001) docker     (116)        6 2023-02-28 02:50:08.000000 cc12703_uiautomator2-2.7.3/uiautomator2/assets/apk_version.txt
+-rw-r--r--   0 runner    (1001) docker     (116)  1061950 2023-02-28 02:50:08.000000 cc12703_uiautomator2-2.7.3/uiautomator2/assets/app-uiautomator-test.apk
+-rw-r--r--   0 runner    (1001) docker     (116)  2191186 2023-02-28 02:50:08.000000 cc12703_uiautomator2-2.7.3/uiautomator2/assets/app-uiautomator.apk
+-rwxr-xr-x   0 runner    (1001) docker     (116)      570 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/assets/sync.sh
+-rw-r--r--   0 runner    (1001) docker     (116)     2643 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-28 02:50:49.000000 cc12703_uiautomator2-2.7.3/uiautomator2/ext/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-28 02:50:49.000000 cc12703_uiautomator2-2.7.3/uiautomator2/ext/htmlreport/
+-rw-r--r--   0 runner    (1001) docker     (116)      405 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/ext/htmlreport/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)     5572 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/ext/htmlreport/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-28 02:50:49.000000 cc12703_uiautomator2-2.7.3/uiautomator2/ext/htmlreport/assets/
+-rw-r--r--   0 runner    (1001) docker     (116)     4802 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/ext/htmlreport/assets/index.html
+-rw-r--r--   0 runner    (1001) docker     (116)    61137 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/ext/htmlreport/assets/pig.jpg
+-rw-r--r--   0 runner    (1001) docker     (116)     1190 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/ext/htmlreport/assets/simplehttpserver.py
+-rw-r--r--   0 runner    (1001) docker     (116)       29 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/ext/htmlreport/assets/start.bat
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-28 02:50:49.000000 cc12703_uiautomator2-2.7.3/uiautomator2/ext/info/
+-rw-r--r--   0 runner    (1001) docker     (116)     2645 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/ext/info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    28515 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/ext/info/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-28 02:50:49.000000 cc12703_uiautomator2-2.7.3/uiautomator2/ext/perf/
+-rw-r--r--   0 runner    (1001) docker     (116)     2852 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/ext/perf/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)    12382 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/ext/perf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    41467 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/ext/perf/net.png
+-rw-r--r--   0 runner    (1001) docker     (116)    26928 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/ext/perf/summary.png
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-28 02:50:49.000000 cc12703_uiautomator2-2.7.3/uiautomator2/ext/xpath/
+-rw-r--r--   0 runner    (1001) docker     (116)       88 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/ext/xpath/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)      227 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/ext/xpath/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-28 02:50:49.000000 cc12703_uiautomator2-2.7.3/uiautomator2/ext-archived/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-28 02:50:49.000000 cc12703_uiautomator2-2.7.3/uiautomator2/ext-archived/aircv/
+-rw-r--r--   0 runner    (1001) docker     (116)     4180 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/ext-archived/aircv/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)    18456 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/ext-archived/aircv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-28 02:50:49.000000 cc12703_uiautomator2-2.7.3/uiautomator2/ext-archived/ocr/
+-rw-r--r--   0 runner    (1001) docker     (116)      947 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/ext-archived/ocr/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)     2494 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/ext-archived/ocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3307 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/ext-archived/ocr/baiduOCR.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10564 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/image.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15113 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/init.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1801 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/messagebox.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3776 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/screenrecord.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3507 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/settings.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1761 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/swipe.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6086 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4900 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/version.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9758 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/watcher.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6703 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/webview.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14506 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/widget.py
+-rw-r--r--   0 runner    (1001) docker     (116)    28843 2023-02-28 02:50:07.000000 cc12703_uiautomator2-2.7.3/uiautomator2/xpath.py
```

### Comparing `cc12703_uiautomator2-2.7.2/CHANGELOG` & `cc12703_uiautomator2-2.7.3/CHANGELOG`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/DEVELOP.md` & `cc12703_uiautomator2-2.7.3/DEVELOP.md`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/LICENSE` & `cc12703_uiautomator2-2.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/PKG-INFO` & `cc12703_uiautomator2-2.7.3/cc12703_uiautomator2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cc12703_uiautomator2
-Version: 2.7.2
+Name: cc12703-uiautomator2
+Version: 2.7.3
 Summary: Python Wrapper for Google Android UiAutomator2 test tool
 Home-page: https://github.com/cc12703/uiautomator2
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 License: MIT
 Description: Documentation in <https://github.com/openatx/uiautomator2>
```

### Comparing `cc12703_uiautomator2-2.7.2/QUICK_REFERENCE.md` & `cc12703_uiautomator2-2.7.3/QUICK_REFERENCE.md`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/README.md` & `cc12703_uiautomator2-2.7.3/README.md`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/XPATH.md` & `cc12703_uiautomator2-2.7.3/XPATH.md`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/appveyor.yml` & `cc12703_uiautomator2-2.7.3/appveyor.yml`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/cc12703_uiautomator2.egg-info/PKG-INFO` & `cc12703_uiautomator2-2.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cc12703-uiautomator2
-Version: 2.7.2
+Name: cc12703_uiautomator2
+Version: 2.7.3
 Summary: Python Wrapper for Google Android UiAutomator2 test tool
 Home-page: https://github.com/cc12703/uiautomator2
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 License: MIT
 Description: Documentation in <https://github.com/openatx/uiautomator2>
```

### Comparing `cc12703_uiautomator2-2.7.2/cc12703_uiautomator2.egg-info/SOURCES.txt` & `cc12703_uiautomator2-2.7.3/cc12703_uiautomator2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/setup.cfg` & `cc12703_uiautomator2-2.7.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/__init__.py` & `cc12703_uiautomator2-2.7.3/uiautomator2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1989,14 +1989,19 @@
         subprocess.call([adbutils.adb_path(), "-s", addr, "wait-for-device"],
                         timeout=2)
     except subprocess.TimeoutExpired:
         raise ConnectError("Fail execute", "adb connect " + addr)
     return connect_usb(addr)
 
 
+
+def disconnect_adb_wifi(addr) :
+    subprocess.call([adbutils.adb_path(), "disconnect", addr])
+
+
 def connect_usb(serial: Optional[str] = None, init: bool = False) -> Device:
     """
     Args:
         serial (str): android device serial
 
     Returns:
         Device
@@ -2031,10 +2036,9 @@
     if _addr is None:
         raise ConnectError("addr is invalid or atx-agent is not running", addr)
     del addr
     return Device(_addr)
 
 
 
-def cfg(key: str, val: str) :
-    _cfg[key] = val
+
```

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/__main__.py` & `cc12703_uiautomator2-2.7.3/uiautomator2/__main__.py`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/_selector.py` & `cc12703_uiautomator2-2.7.3/uiautomator2/_selector.py`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/abcd.py` & `cc12703_uiautomator2-2.7.3/uiautomator2/abcd.py`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/assets/app-uiautomator-test.apk` & `cc12703_uiautomator2-2.7.3/uiautomator2/assets/app-uiautomator-test.apk`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/assets/app-uiautomator.apk` & `cc12703_uiautomator2-2.7.3/uiautomator2/assets/app-uiautomator.apk`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/assets/sync.sh` & `cc12703_uiautomator2-2.7.3/uiautomator2/assets/sync.sh`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/exceptions.py` & `cc12703_uiautomator2-2.7.3/uiautomator2/exceptions.py`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/ext/htmlreport/__init__.py` & `cc12703_uiautomator2-2.7.3/uiautomator2/ext/htmlreport/__init__.py`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/ext/htmlreport/assets/index.html` & `cc12703_uiautomator2-2.7.3/uiautomator2/ext/htmlreport/assets/index.html`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/ext/htmlreport/assets/pig.jpg` & `cc12703_uiautomator2-2.7.3/uiautomator2/ext/htmlreport/assets/pig.jpg`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/ext/htmlreport/assets/simplehttpserver.py` & `cc12703_uiautomator2-2.7.3/uiautomator2/ext/htmlreport/assets/simplehttpserver.py`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/ext/info/__init__.py` & `cc12703_uiautomator2-2.7.3/uiautomator2/ext/info/__init__.py`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/ext/info/conf.py` & `cc12703_uiautomator2-2.7.3/uiautomator2/ext/info/conf.py`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/ext/perf/README.md` & `cc12703_uiautomator2-2.7.3/uiautomator2/ext/perf/README.md`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/ext/perf/__init__.py` & `cc12703_uiautomator2-2.7.3/uiautomator2/ext/perf/__init__.py`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/ext/perf/net.png` & `cc12703_uiautomator2-2.7.3/uiautomator2/ext/perf/net.png`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/ext/perf/summary.png` & `cc12703_uiautomator2-2.7.3/uiautomator2/ext/perf/summary.png`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/ext-archived/aircv/README.md` & `cc12703_uiautomator2-2.7.3/uiautomator2/ext-archived/aircv/README.md`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/ext-archived/aircv/__init__.py` & `cc12703_uiautomator2-2.7.3/uiautomator2/ext-archived/aircv/__init__.py`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/ext-archived/ocr/README.md` & `cc12703_uiautomator2-2.7.3/uiautomator2/ext-archived/ocr/README.md`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/ext-archived/ocr/__init__.py` & `cc12703_uiautomator2-2.7.3/uiautomator2/ext-archived/ocr/__init__.py`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/ext-archived/ocr/baiduOCR.py` & `cc12703_uiautomator2-2.7.3/uiautomator2/ext-archived/ocr/baiduOCR.py`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/image.py` & `cc12703_uiautomator2-2.7.3/uiautomator2/image.py`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/init.py` & `cc12703_uiautomator2-2.7.3/uiautomator2/init.py`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/messagebox.py` & `cc12703_uiautomator2-2.7.3/uiautomator2/messagebox.py`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/screenrecord.py` & `cc12703_uiautomator2-2.7.3/uiautomator2/screenrecord.py`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/settings.py` & `cc12703_uiautomator2-2.7.3/uiautomator2/settings.py`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/swipe.py` & `cc12703_uiautomator2-2.7.3/uiautomator2/swipe.py`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/utils.py` & `cc12703_uiautomator2-2.7.3/uiautomator2/utils.py`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/version.py` & `cc12703_uiautomator2-2.7.3/uiautomator2/version.py`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/watcher.py` & `cc12703_uiautomator2-2.7.3/uiautomator2/watcher.py`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/webview.py` & `cc12703_uiautomator2-2.7.3/uiautomator2/webview.py`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/widget.py` & `cc12703_uiautomator2-2.7.3/uiautomator2/widget.py`

 * *Files identical despite different names*

### Comparing `cc12703_uiautomator2-2.7.2/uiautomator2/xpath.py` & `cc12703_uiautomator2-2.7.3/uiautomator2/xpath.py`

 * *Files identical despite different names*

