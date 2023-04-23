# Comparing `tmp/glority-tidevice-0.0.3.tar.gz` & `tmp/glority-tidevice-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glority-tidevice-0.0.3.tar", last modified: Fri Nov 18 02:53:34 2022, max compression
+gzip compressed data, was "glority-tidevice-0.4.0.tar", last modified: Sun Apr 23 12:51:52 2023, max compression
```

## Comparing `glority-tidevice-0.0.3.tar` & `glority-tidevice-0.4.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxrwx   0        0        0        0 2022-11-18 02:53:34.113562 glority-tidevice-0.0.3/
--rw-rw-rw-   0        0        0       89 2022-11-18 02:53:33.000000 glority-tidevice-0.0.3/AUTHORS
--rw-rw-rw-   0        0        0      149 2022-11-18 02:53:33.000000 glority-tidevice-0.0.3/ChangeLog
--rw-rw-rw-   0        0        0     2022 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/DEVELOP.md
--rw-rw-rw-   0        0        0     1064 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      457 2022-11-18 02:53:34.113562 glority-tidevice-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      847 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/PROTOCOL.md
--rw-rw-rw-   0        0        0    13216 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/README.md
--rw-rw-rw-   0        0        0    11568 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/README_EN.md
-drwxrwxrwx   0        0        0        0 2022-11-18 02:53:33.901562 glority-tidevice-0.0.3/assets/
--rw-rw-rw-   0        0        0    12630 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/assets/tidevice-logo.png
-drwxrwxrwx   0        0        0        0 2022-11-18 02:53:33.910564 glority-tidevice-0.0.3/examples/
--rw-rw-rw-   0        0        0      120 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/examples/get_bundle_id_from_ipa.py
--rw-rw-rw-   0        0        0      757 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/examples/read_properties.py
-drwxrwxrwx   0        0        0        0 2022-11-18 02:53:33.945564 glority-tidevice-0.0.3/glority_tidevice.egg-info/
--rw-rw-rw-   0        0        0      457 2022-11-18 02:53:33.000000 glority-tidevice-0.0.3/glority_tidevice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1332 2022-11-18 02:53:33.000000 glority-tidevice-0.0.3/glority_tidevice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-18 02:53:33.000000 glority-tidevice-0.0.3/glority_tidevice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2022-11-18 02:53:33.000000 glority-tidevice-0.0.3/glority_tidevice.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-11-18 02:53:33.000000 glority-tidevice-0.0.3/glority_tidevice.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       47 2022-11-18 02:53:33.000000 glority-tidevice-0.0.3/glority_tidevice.egg-info/pbr.json
--rw-rw-rw-   0        0        0      145 2022-11-18 02:53:33.000000 glority-tidevice-0.0.3/glority_tidevice.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-11-18 02:53:33.000000 glority-tidevice-0.0.3/glority_tidevice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      289 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/release.sh
--rw-rw-rw-   0        0        0      375 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/requirements.txt
-drwxrwxrwx   0        0        0        0 2022-11-18 02:53:33.972563 glority-tidevice-0.0.3/scripts/
--rw-rw-rw-   0        0        0     4012 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/scripts/ipa_sign.sh
--rw-rw-rw-   0        0        0    17538 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/scripts/plistdump-tcp-proxy.py
--rw-rw-rw-   0        0        0       15 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/scripts/requirements.txt
--rw-rw-rw-   0        0        0     2979 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/scripts/run-usbmuxd-proxy.sh
--rw-rw-rw-   0        0        0      274 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/scripts/simple-capture.sh
--rw-rw-rw-   0        0        0     3201 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/scripts/uitest_screenrecord.py
--rw-rw-rw-   0        0        0      734 2022-11-18 02:53:34.115564 glority-tidevice-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      226 2022-10-19 02:37:26.000000 glority-tidevice-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-18 02:53:33.993562 glority-tidevice-0.0.3/tests/
--rw-rw-rw-   0        0        0      291 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/tests/conftest.py
--rw-rw-rw-   0        0        0       45 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/tests/runtest.sh
--rw-rw-rw-   0        0        0      228 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/tests/test_device.py
--rw-rw-rw-   0        0        0      474 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/tests/test_ipautil.py
--rw-rw-rw-   0        0        0     2002 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/tests/test_usbmux.py
-drwxrwxrwx   0        0        0        0 2022-11-18 02:53:34.108563 glority-tidevice-0.0.3/tidevice/
--rw-rw-rw-   0        0        0      349 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/tidevice/__init__.py
--rw-rw-rw-   0        0        0    30644 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/tidevice/__main__.py
--rw-rw-rw-   0        0        0      171 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/tidevice/_compat.py
--rw-rw-rw-   0        0        0      768 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/tidevice/_crash.py
--rw-rw-rw-   0        0        0    41275 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/tidevice/_device.py
--rw-rw-rw-   0        0        0    13829 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/tidevice/_hexdump.py
--rw-rw-rw-   0        0        0     6055 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/tidevice/_imagemounter.py
--rw-rw-rw-   0        0        0     9935 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/tidevice/_installation.py
--rw-rw-rw-   0        0        0    39153 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/tidevice/_instruments.py
--rw-rw-rw-   0        0        0     3171 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/tidevice/_ipautil.py
--rw-rw-rw-   0        0        0    11838 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/tidevice/_perf.py
--rw-rw-rw-   0        0        0    11907 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/tidevice/_proto.py
--rw-rw-rw-   0        0        0     2980 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/tidevice/_relay.py
--rw-rw-rw-   0        0        0     7598 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/tidevice/_safe_socket.py
--rw-rw-rw-   0        0        0     3237 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/tidevice/_ssl.py
--rw-rw-rw-   0        0        0    14128 2022-11-18 02:50:02.000000 glority-tidevice-0.0.3/tidevice/_sync.py
--rw-rw-rw-   0        0        0      609 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/tidevice/_types.py
--rw-rw-rw-   0        0        0     5399 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/tidevice/_usbmux.py
--rw-rw-rw-   0        0        0     6799 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/tidevice/_utils.py
--rw-rw-rw-   0        0        0      242 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/tidevice/_version.py
--rw-rw-rw-   0        0        0     7803 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/tidevice/_wdaproxy.py
--rw-rw-rw-   0        0        0    18769 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/tidevice/bplist.py
--rw-rw-rw-   0        0        0      590 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/tidevice/exceptions.py
--rw-rw-rw-   0        0        0    31289 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/tidevice/plistlib2.py
--rw-rw-rw-   0        0        0     3423 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/tidevice/requests_usbmux.py
--rw-rw-rw-   0        0        0     3004 2022-08-25 14:34:52.000000 glority-tidevice-0.0.3/tidevice/struct2.py
+drwxrwxrwx   0        0        0        0 2023-04-23 12:51:52.294419 glority-tidevice-0.4.0/
+-rw-rw-rw-   0        0        0       89 2023-04-23 12:51:51.000000 glority-tidevice-0.4.0/AUTHORS
+-rw-rw-rw-   0        0        0      175 2023-04-23 12:51:51.000000 glority-tidevice-0.4.0/ChangeLog
+-rw-rw-rw-   0        0        0     2022 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/DEVELOP.md
+-rw-rw-rw-   0        0        0     1064 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0      457 2023-04-23 12:51:52.294419 glority-tidevice-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      847 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/PROTOCOL.md
+-rw-rw-rw-   0        0        0    13216 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/README.md
+-rw-rw-rw-   0        0        0    11568 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/README_EN.md
+drwxrwxrwx   0        0        0        0 2023-04-23 12:51:51.933893 glority-tidevice-0.4.0/assets/
+-rw-rw-rw-   0        0        0    12630 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/assets/tidevice-logo.png
+drwxrwxrwx   0        0        0        0 2023-04-23 12:51:51.947892 glority-tidevice-0.4.0/examples/
+-rw-rw-rw-   0        0        0      120 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/examples/get_bundle_id_from_ipa.py
+-rw-rw-rw-   0        0        0      757 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/examples/read_properties.py
+drwxrwxrwx   0        0        0        0 2023-04-23 12:51:51.999897 glority-tidevice-0.4.0/glority_tidevice.egg-info/
+-rw-rw-rw-   0        0        0      457 2023-04-23 12:51:51.000000 glority-tidevice-0.4.0/glority_tidevice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1332 2023-04-23 12:51:51.000000 glority-tidevice-0.4.0/glority_tidevice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 12:51:51.000000 glority-tidevice-0.4.0/glority_tidevice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-04-23 12:51:51.000000 glority-tidevice-0.4.0/glority_tidevice.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-11-18 02:53:33.000000 glority-tidevice-0.4.0/glority_tidevice.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       47 2023-04-23 12:51:51.000000 glority-tidevice-0.4.0/glority_tidevice.egg-info/pbr.json
+-rw-rw-rw-   0        0        0      145 2023-04-23 12:51:51.000000 glority-tidevice-0.4.0/glority_tidevice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-23 12:51:51.000000 glority-tidevice-0.4.0/glority_tidevice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      289 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/release.sh
+-rw-rw-rw-   0        0        0      375 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 12:51:52.045892 glority-tidevice-0.4.0/scripts/
+-rw-rw-rw-   0        0        0     4012 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/scripts/ipa_sign.sh
+-rw-rw-rw-   0        0        0    17538 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/scripts/plistdump-tcp-proxy.py
+-rw-rw-rw-   0        0        0       15 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/scripts/requirements.txt
+-rw-rw-rw-   0        0        0     2979 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/scripts/run-usbmuxd-proxy.sh
+-rw-rw-rw-   0        0        0      274 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/scripts/simple-capture.sh
+-rw-rw-rw-   0        0        0     3201 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/scripts/uitest_screenrecord.py
+-rw-rw-rw-   0        0        0      734 2023-04-23 12:51:52.298417 glority-tidevice-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      226 2022-10-19 02:37:26.000000 glority-tidevice-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 12:51:52.086898 glority-tidevice-0.4.0/tests/
+-rw-rw-rw-   0        0        0      291 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/tests/conftest.py
+-rw-rw-rw-   0        0        0       45 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/tests/runtest.sh
+-rw-rw-rw-   0        0        0      228 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/tests/test_device.py
+-rw-rw-rw-   0        0        0      474 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/tests/test_ipautil.py
+-rw-rw-rw-   0        0        0     2002 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/tests/test_usbmux.py
+drwxrwxrwx   0        0        0        0 2023-04-23 12:51:52.287418 glority-tidevice-0.4.0/tidevice/
+-rw-rw-rw-   0        0        0      349 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/tidevice/__init__.py
+-rw-rw-rw-   0        0        0    30644 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/tidevice/__main__.py
+-rw-rw-rw-   0        0        0      171 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/tidevice/_compat.py
+-rw-rw-rw-   0        0        0      768 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/tidevice/_crash.py
+-rw-rw-rw-   0        0        0    41275 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/tidevice/_device.py
+-rw-rw-rw-   0        0        0    13829 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/tidevice/_hexdump.py
+-rw-rw-rw-   0        0        0     6058 2023-04-23 12:47:52.000000 glority-tidevice-0.4.0/tidevice/_imagemounter.py
+-rw-rw-rw-   0        0        0     9935 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/tidevice/_installation.py
+-rw-rw-rw-   0        0        0    39153 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/tidevice/_instruments.py
+-rw-rw-rw-   0        0        0     3171 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/tidevice/_ipautil.py
+-rw-rw-rw-   0        0        0    11838 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/tidevice/_perf.py
+-rw-rw-rw-   0        0        0    11907 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/tidevice/_proto.py
+-rw-rw-rw-   0        0        0     2980 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/tidevice/_relay.py
+-rw-rw-rw-   0        0        0     7598 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/tidevice/_safe_socket.py
+-rw-rw-rw-   0        0        0     3237 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/tidevice/_ssl.py
+-rw-rw-rw-   0        0        0    14128 2022-11-18 02:50:02.000000 glority-tidevice-0.4.0/tidevice/_sync.py
+-rw-rw-rw-   0        0        0      609 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/tidevice/_types.py
+-rw-rw-rw-   0        0        0     5399 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/tidevice/_usbmux.py
+-rw-rw-rw-   0        0        0     6799 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/tidevice/_utils.py
+-rw-rw-rw-   0        0        0      242 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/tidevice/_version.py
+-rw-rw-rw-   0        0        0     7803 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/tidevice/_wdaproxy.py
+-rw-rw-rw-   0        0        0    18769 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/tidevice/bplist.py
+-rw-rw-rw-   0        0        0      590 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/tidevice/exceptions.py
+-rw-rw-rw-   0        0        0    31289 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/tidevice/plistlib2.py
+-rw-rw-rw-   0        0        0     3423 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/tidevice/requests_usbmux.py
+-rw-rw-rw-   0        0        0     3004 2022-08-25 14:34:52.000000 glority-tidevice-0.4.0/tidevice/struct2.py
```

### Comparing `glority-tidevice-0.0.3/DEVELOP.md` & `glority-tidevice-0.4.0/DEVELOP.md`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/LICENSE` & `glority-tidevice-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/PROTOCOL.md` & `glority-tidevice-0.4.0/PROTOCOL.md`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/README.md` & `glority-tidevice-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/README_EN.md` & `glority-tidevice-0.4.0/README_EN.md`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/assets/tidevice-logo.png` & `glority-tidevice-0.4.0/assets/tidevice-logo.png`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/examples/read_properties.py` & `glority-tidevice-0.4.0/examples/read_properties.py`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/glority_tidevice.egg-info/SOURCES.txt` & `glority-tidevice-0.4.0/glority_tidevice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/scripts/ipa_sign.sh` & `glority-tidevice-0.4.0/scripts/ipa_sign.sh`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/scripts/plistdump-tcp-proxy.py` & `glority-tidevice-0.4.0/scripts/plistdump-tcp-proxy.py`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/scripts/run-usbmuxd-proxy.sh` & `glority-tidevice-0.4.0/scripts/run-usbmuxd-proxy.sh`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/scripts/uitest_screenrecord.py` & `glority-tidevice-0.4.0/scripts/uitest_screenrecord.py`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/setup.cfg` & `glority-tidevice-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/tests/test_usbmux.py` & `glority-tidevice-0.4.0/tests/test_usbmux.py`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/tidevice/__main__.py` & `glority-tidevice-0.4.0/tidevice/__main__.py`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/tidevice/_crash.py` & `glority-tidevice-0.4.0/tidevice/_crash.py`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/tidevice/_device.py` & `glority-tidevice-0.4.0/tidevice/_device.py`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/tidevice/_hexdump.py` & `glority-tidevice-0.4.0/tidevice/_hexdump.py`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/tidevice/_imagemounter.py` & `glority-tidevice-0.4.0/tidevice/_imagemounter.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     # https://github.com/JinjunHan/iOSDeviceSupport
     github_repo = "JinjunHan/iOSDeviceSupport"
     zip_name = f"{version}.zip"
 
     # the code.aliyun slowlly
     # gitee requires login
     # aliyun_url = f"https://code.aliyun.com/hanjinjun/iOSDeviceSupoort/raw/master/DeviceSupport/{zip_name}"
-    origin_url = f"https://github.com/{github_repo}/raw/master/DeviceSupport/{zip_name}"
+    origin_url = f"https://github.com/{github_repo}/raw/master/iOSDeviceSupport/{zip_name}"
     mirror_url = origin_url.replace("https://github.com", "https://tool.appetizer.io")
     return (mirror_url, origin_url)
 
 def cache_developer_image(version: str) -> str:
     """
     download developer image from github to local
     return image_zip_path
```

### Comparing `glority-tidevice-0.0.3/tidevice/_installation.py` & `glority-tidevice-0.4.0/tidevice/_installation.py`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/tidevice/_instruments.py` & `glority-tidevice-0.4.0/tidevice/_instruments.py`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/tidevice/_ipautil.py` & `glority-tidevice-0.4.0/tidevice/_ipautil.py`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/tidevice/_perf.py` & `glority-tidevice-0.4.0/tidevice/_perf.py`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/tidevice/_proto.py` & `glority-tidevice-0.4.0/tidevice/_proto.py`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/tidevice/_relay.py` & `glority-tidevice-0.4.0/tidevice/_relay.py`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/tidevice/_safe_socket.py` & `glority-tidevice-0.4.0/tidevice/_safe_socket.py`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/tidevice/_ssl.py` & `glority-tidevice-0.4.0/tidevice/_ssl.py`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/tidevice/_sync.py` & `glority-tidevice-0.4.0/tidevice/_sync.py`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/tidevice/_types.py` & `glority-tidevice-0.4.0/tidevice/_types.py`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/tidevice/_usbmux.py` & `glority-tidevice-0.4.0/tidevice/_usbmux.py`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/tidevice/_utils.py` & `glority-tidevice-0.4.0/tidevice/_utils.py`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/tidevice/_wdaproxy.py` & `glority-tidevice-0.4.0/tidevice/_wdaproxy.py`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/tidevice/bplist.py` & `glority-tidevice-0.4.0/tidevice/bplist.py`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/tidevice/exceptions.py` & `glority-tidevice-0.4.0/tidevice/exceptions.py`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/tidevice/plistlib2.py` & `glority-tidevice-0.4.0/tidevice/plistlib2.py`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/tidevice/requests_usbmux.py` & `glority-tidevice-0.4.0/tidevice/requests_usbmux.py`

 * *Files identical despite different names*

### Comparing `glority-tidevice-0.0.3/tidevice/struct2.py` & `glority-tidevice-0.4.0/tidevice/struct2.py`

 * *Files identical despite different names*

