# Comparing `tmp/ovos_audio_plugin_simple-0.0.2a2-py3-none-any.whl.zip` & `tmp/ovos_audio_plugin_simple-0.0.2a3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 9311 bytes, number of entries: 8
--rw-r--r--  2.0 unx    10954 b- defN 22-Aug-05 12:10 ovos_audio_plugin_simple/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 22-Aug-05 12:11 ovos_audio_plugin_simple/version.py
--rw-r--r--  2.0 unx    11349 b- defN 22-Aug-05 12:11 ovos_audio_plugin_simple-0.0.2a2.dist-info/LICENSE
--rw-r--r--  2.0 unx      341 b- defN 22-Aug-05 12:11 ovos_audio_plugin_simple-0.0.2a2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Aug-05 12:11 ovos_audio_plugin_simple-0.0.2a2.dist-info/WHEEL
--rw-r--r--  2.0 unx      186 b- defN 22-Aug-05 12:11 ovos_audio_plugin_simple-0.0.2a2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       25 b- defN 22-Aug-05 12:11 ovos_audio_plugin_simple-0.0.2a2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      781 b- defN 22-Aug-05 12:11 ovos_audio_plugin_simple-0.0.2a2.dist-info/RECORD
-8 files, 23905 bytes uncompressed, 7913 bytes compressed:  66.9%
+Zip file size: 9305 bytes, number of entries: 8
+-rw-r--r--  2.0 unx    10943 b- defN 23-Apr-23 01:58 ovos_audio_plugin_simple/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Apr-23 01:58 ovos_audio_plugin_simple/version.py
+-rw-r--r--  2.0 unx    11349 b- defN 23-Apr-23 01:58 ovos_audio_plugin_simple-0.0.2a3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      341 b- defN 23-Apr-23 01:58 ovos_audio_plugin_simple-0.0.2a3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-23 01:58 ovos_audio_plugin_simple-0.0.2a3.dist-info/WHEEL
+-rw-r--r--  2.0 unx      186 b- defN 23-Apr-23 01:58 ovos_audio_plugin_simple-0.0.2a3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       25 b- defN 23-Apr-23 01:58 ovos_audio_plugin_simple-0.0.2a3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      781 b- defN 23-Apr-23 01:58 ovos_audio_plugin_simple-0.0.2a3.dist-info/RECORD
+8 files, 23894 bytes uncompressed, 7907 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: ovos_audio_plugin_simple/__init__.py
 Comment: 
 
 Filename: ovos_audio_plugin_simple/version.py
 Comment: 
 
-Filename: ovos_audio_plugin_simple-0.0.2a2.dist-info/LICENSE
+Filename: ovos_audio_plugin_simple-0.0.2a3.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_audio_plugin_simple-0.0.2a2.dist-info/METADATA
+Filename: ovos_audio_plugin_simple-0.0.2a3.dist-info/METADATA
 Comment: 
 
-Filename: ovos_audio_plugin_simple-0.0.2a2.dist-info/WHEEL
+Filename: ovos_audio_plugin_simple-0.0.2a3.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_audio_plugin_simple-0.0.2a2.dist-info/entry_points.txt
+Filename: ovos_audio_plugin_simple-0.0.2a3.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_audio_plugin_simple-0.0.2a2.dist-info/top_level.txt
+Filename: ovos_audio_plugin_simple-0.0.2a3.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_audio_plugin_simple-0.0.2a2.dist-info/RECORD
+Filename: ovos_audio_plugin_simple-0.0.2a3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_audio_plugin_simple/__init__.py

```diff
@@ -1,15 +1,15 @@
 import mimetypes
 import re
 import signal
 import subprocess
 from distutils.spawn import find_executable
 from time import sleep
 
-from mycroft_bus_client.message import Message
+from ovos_bus_client import Message
 from ovos_plugin_common_play.ocp.status import TrackState, MediaState, PlayerState
 from ovos_plugin_manager.templates.audio import AudioBackend
 from ovos_utils.log import LOG
 from requests import Session
 
 
 def find_mime(path):
```

## ovos_audio_plugin_simple/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 2
-VERSION_ALPHA = 2
+VERSION_ALPHA = 3
 # END_VERSION_BLOCK
```

## Comparing `ovos_audio_plugin_simple-0.0.2a2.dist-info/LICENSE` & `ovos_audio_plugin_simple-0.0.2a3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ovos_audio_plugin_simple-0.0.2a2.dist-info/RECORD` & `ovos_audio_plugin_simple-0.0.2a3.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-ovos_audio_plugin_simple/__init__.py,sha256=pWX-wj-lzjWqaW20JNwglWfAtrUVCJ8aFlXiEHJazhA,10954
-ovos_audio_plugin_simple/version.py,sha256=afVkQ7_AdQfLgFZ-hJN_LyKZAc5EOc9ZSwssDiyGXfM,177
-ovos_audio_plugin_simple-0.0.2a2.dist-info/LICENSE,sha256=fYHkowW9JcaEcqCPTXYBayNJ9J1lGdYVb7Mf9oy6oEY,11349
-ovos_audio_plugin_simple-0.0.2a2.dist-info/METADATA,sha256=Vf021WlDPtJ0n91j9QzwVEfuA4lDz3VssXCawKD0270,341
-ovos_audio_plugin_simple-0.0.2a2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-ovos_audio_plugin_simple-0.0.2a2.dist-info/entry_points.txt,sha256=9BLpnjirJzeim9wM6pKDKQaR23IkuvJzuKl72t8_tYs,186
-ovos_audio_plugin_simple-0.0.2a2.dist-info/top_level.txt,sha256=YNw4wRuGlHldkXtE2loAH3YViSvS_VvWQfAX-xz_vrM,25
-ovos_audio_plugin_simple-0.0.2a2.dist-info/RECORD,,
+ovos_audio_plugin_simple/__init__.py,sha256=KxNkFtJNdfSIRT2M-ykDpjwBiW287F7q6G9jtrDSkZE,10943
+ovos_audio_plugin_simple/version.py,sha256=zGGpi5TVnl3sfIR-mw8qdnI3aEKn4IkPu207d0eIqb8,177
+ovos_audio_plugin_simple-0.0.2a3.dist-info/LICENSE,sha256=fYHkowW9JcaEcqCPTXYBayNJ9J1lGdYVb7Mf9oy6oEY,11349
+ovos_audio_plugin_simple-0.0.2a3.dist-info/METADATA,sha256=SjqfAjS3_bwDr8ayyxub6m95koUKYKIZMt8Fty0jK30,341
+ovos_audio_plugin_simple-0.0.2a3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ovos_audio_plugin_simple-0.0.2a3.dist-info/entry_points.txt,sha256=9BLpnjirJzeim9wM6pKDKQaR23IkuvJzuKl72t8_tYs,186
+ovos_audio_plugin_simple-0.0.2a3.dist-info/top_level.txt,sha256=YNw4wRuGlHldkXtE2loAH3YViSvS_VvWQfAX-xz_vrM,25
+ovos_audio_plugin_simple-0.0.2a3.dist-info/RECORD,,
```

