# Comparing `tmp/Range_Announcer-1.1.0.tar.gz` & `tmp/Range_Announcer-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Range_Announcer-1.1.0.tar", last modified: Mon Jan 16 22:57:43 2023, max compression
+gzip compressed data, was "Range_Announcer-1.2.0.tar", last modified: Sun Apr 23 18:43:43 2023, max compression
```

## Comparing `Range_Announcer-1.1.0.tar` & `Range_Announcer-1.2.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-01-16 22:57:43.747295 Range_Announcer-1.1.0/
--rw-rw-rw-   0        0        0     1555 2023-01-09 20:15:46.000000 Range_Announcer-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      113 2023-01-09 21:55:13.000000 Range_Announcer-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4069 2023-01-16 22:57:43.747295 Range_Announcer-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2762 2023-01-11 06:22:25.000000 Range_Announcer-1.1.0/README.md
--rw-rw-rw-   0        0        0      101 2023-01-08 01:45:03.000000 Range_Announcer-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0     1575 2023-01-16 22:57:43.749294 Range_Announcer-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-01-16 22:57:43.603350 Range_Announcer-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-01-16 22:57:43.634340 Range_Announcer-1.1.0/src/Range_Announcer.egg-info/
--rw-rw-rw-   0        0        0     4069 2023-01-16 22:57:43.000000 Range_Announcer-1.1.0/src/Range_Announcer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      862 2023-01-16 22:57:43.000000 Range_Announcer-1.1.0/src/Range_Announcer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-16 22:57:43.000000 Range_Announcer-1.1.0/src/Range_Announcer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      132 2023-01-16 22:57:43.000000 Range_Announcer-1.1.0/src/Range_Announcer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2023-01-16 22:57:43.000000 Range_Announcer-1.1.0/src/Range_Announcer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-01-16 22:57:43.000000 Range_Announcer-1.1.0/src/Range_Announcer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-01-16 22:57:43.666328 Range_Announcer-1.1.0/src/range_announcer/
--rw-rw-rw-   0        0        0        0 2023-01-08 07:27:00.000000 Range_Announcer-1.1.0/src/range_announcer/__init__.py
--rw-rw-rw-   0        0        0     5987 2023-01-14 18:41:46.000000 Range_Announcer-1.1.0/src/range_announcer/__main__.py
--rw-rw-rw-   0        0        0     2701 2023-01-16 22:54:53.000000 Range_Announcer-1.1.0/src/range_announcer/announcer.py
--rw-rw-rw-   0        0        0      314 2023-01-09 09:34:53.000000 Range_Announcer-1.1.0/src/range_announcer/rangeannouncer.json
-drwxrwxrwx   0        0        0        0 2023-01-16 22:57:43.745295 Range_Announcer-1.1.0/src/range_announcer/sound/
--rw-rw-rw-   0        0        0   402442 2023-01-02 07:57:05.000000 Range_Announcer-1.1.0/src/range_announcer/sound/15_minutes.mp3
--rw-rw-rw-   0        0        0   295786 2023-01-02 07:56:09.000000 Range_Announcer-1.1.0/src/range_announcer/sound/30_minutes.mp3
--rw-rw-rw-   0        0        0   418761 2023-01-02 07:57:52.000000 Range_Announcer-1.1.0/src/range_announcer/sound/5_minutes.mp3
--rw-rw-rw-   0        0        0  7385306 2015-05-05 12:55:19.000000 Range_Announcer-1.1.0/src/range_announcer/sound/BackInBlack.mp3
--rw-rw-rw-   0        0        0   454470 2023-01-02 07:58:33.000000 Range_Announcer-1.1.0/src/range_announcer/sound/closed.mp3
--rw-rw-rw-   0        0        0    34476 2022-12-08 21:41:26.000000 Range_Announcer-1.1.0/src/range_announcer/sound/complete.wav
--rw-rw-rw-   0        0        0   333128 2023-01-02 07:55:19.000000 Range_Announcer-1.1.0/src/range_announcer/sound/one_hour.mp3
--rw-rw-rw-   0        0        0      164 2023-01-01 20:35:20.000000 Range_Announcer-1.1.0/src/range_announcer/sound/playsound.py
--rw-rw-rw-   0        0        0     5698 2023-01-09 21:24:28.000000 Range_Announcer-1.1.0/src/range_announcer/sunrise.py
--rw-rw-rw-   0        0        0     1871 2023-01-15 20:43:33.000000 Range_Announcer-1.1.0/src/range_announcer/switch.py
--rw-rw-rw-   0        0        0     5227 2023-01-09 05:01:29.000000 Range_Announcer-1.1.0/src/range_announcer/timezone.py
+drwxrwxrwx   0        0        0        0 2023-04-23 18:43:43.606398 Range_Announcer-1.2.0/
+-rw-rw-rw-   0        0        0     1555 2023-01-09 20:15:46.000000 Range_Announcer-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0      113 2023-01-09 21:55:13.000000 Range_Announcer-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4069 2023-04-23 18:43:43.606398 Range_Announcer-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2762 2023-01-11 06:22:25.000000 Range_Announcer-1.2.0/README.md
+-rw-rw-rw-   0        0        0      101 2023-01-08 01:45:03.000000 Range_Announcer-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1575 2023-04-23 18:43:43.606398 Range_Announcer-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-23 18:43:43.580762 Range_Announcer-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-23 18:43:43.590767 Range_Announcer-1.2.0/src/Range_Announcer.egg-info/
+-rw-rw-rw-   0        0        0     4069 2023-04-23 18:43:43.000000 Range_Announcer-1.2.0/src/Range_Announcer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      862 2023-04-23 18:43:43.000000 Range_Announcer-1.2.0/src/Range_Announcer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 18:43:43.000000 Range_Announcer-1.2.0/src/Range_Announcer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      132 2023-04-23 18:43:43.000000 Range_Announcer-1.2.0/src/Range_Announcer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2023-04-23 18:43:43.000000 Range_Announcer-1.2.0/src/Range_Announcer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-23 18:43:43.000000 Range_Announcer-1.2.0/src/Range_Announcer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 18:43:43.606398 Range_Announcer-1.2.0/src/range_announcer/
+-rw-rw-rw-   0        0        0        0 2023-01-08 07:27:00.000000 Range_Announcer-1.2.0/src/range_announcer/__init__.py
+-rw-rw-rw-   0        0        0     5987 2023-01-14 18:41:46.000000 Range_Announcer-1.2.0/src/range_announcer/__main__.py
+-rw-rw-rw-   0        0        0     2701 2023-01-16 22:54:53.000000 Range_Announcer-1.2.0/src/range_announcer/announcer.py
+-rw-rw-rw-   0        0        0      314 2023-01-09 09:34:53.000000 Range_Announcer-1.2.0/src/range_announcer/rangeannouncer.json
+drwxrwxrwx   0        0        0        0 2023-04-23 18:43:43.606398 Range_Announcer-1.2.0/src/range_announcer/sound/
+-rw-rw-rw-   0        0        0   402442 2023-01-02 07:57:05.000000 Range_Announcer-1.2.0/src/range_announcer/sound/15_minutes.mp3
+-rw-rw-rw-   0        0        0   295786 2023-01-02 07:56:09.000000 Range_Announcer-1.2.0/src/range_announcer/sound/30_minutes.mp3
+-rw-rw-rw-   0        0        0   418761 2023-01-02 07:57:52.000000 Range_Announcer-1.2.0/src/range_announcer/sound/5_minutes.mp3
+-rw-rw-rw-   0        0        0  7385306 2015-05-05 12:55:19.000000 Range_Announcer-1.2.0/src/range_announcer/sound/BackInBlack.mp3
+-rw-rw-rw-   0        0        0   454470 2023-01-02 07:58:33.000000 Range_Announcer-1.2.0/src/range_announcer/sound/closed.mp3
+-rw-rw-rw-   0        0        0    34476 2022-12-08 21:41:26.000000 Range_Announcer-1.2.0/src/range_announcer/sound/complete.wav
+-rw-rw-rw-   0        0        0   333128 2023-01-02 07:55:19.000000 Range_Announcer-1.2.0/src/range_announcer/sound/one_hour.mp3
+-rw-rw-rw-   0        0        0      164 2023-01-01 20:35:20.000000 Range_Announcer-1.2.0/src/range_announcer/sound/playsound.py
+-rw-rw-rw-   0        0        0     5698 2023-01-09 21:24:28.000000 Range_Announcer-1.2.0/src/range_announcer/sunrise.py
+-rw-rw-rw-   0        0        0     1934 2023-04-23 18:05:57.000000 Range_Announcer-1.2.0/src/range_announcer/switch.py
+-rw-rw-rw-   0        0        0     5227 2023-01-09 05:01:29.000000 Range_Announcer-1.2.0/src/range_announcer/timezone.py
```

### Comparing `Range_Announcer-1.1.0/LICENSE` & `Range_Announcer-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Range_Announcer-1.1.0/PKG-INFO` & `Range_Announcer-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Range_Announcer
-Version: 1.1.0
+Version: 1.2.0
 Summary: Announce range closure as sunset approaches
 Home-page: https://github.com/CrazyVikingProductions/range_announcer
 Author: Michael J. Swenson
 Author-email: mikswenson@gmail.com
 Project-URL: Bug Reports, https://github.com/CrazyVikingProductions/range_announcer/issues
 Project-URL: Source, https://github.com/CrazyVikingProductions/range_announcer
 Keywords: sunset closure announce
```

### Comparing `Range_Announcer-1.1.0/README.md` & `Range_Announcer-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `Range_Announcer-1.1.0/setup.cfg` & `Range_Announcer-1.2.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2052 616e 6765 5f41 6e6e 6f75 6e63   = Range_Announc
 00000020: 6572 0d0a 7665 7273 696f 6e20 3d20 312e  er..version = 1.
-00000030: 312e 300d 0a64 6573 6372 6970 7469 6f6e  1.0..description
+00000030: 322e 300d 0a64 6573 6372 6970 7469 6f6e  2.0..description
 00000040: 203d 2041 6e6e 6f75 6e63 6520 7261 6e67   = Announce rang
 00000050: 6520 636c 6f73 7572 6520 6173 2073 756e  e closure as sun
 00000060: 7365 7420 6170 7072 6f61 6368 6573 0d0a  set approaches..
 00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000080: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
 00000090: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
 000000a0: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
```

### Comparing `Range_Announcer-1.1.0/src/Range_Announcer.egg-info/PKG-INFO` & `Range_Announcer-1.2.0/src/Range_Announcer.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Range-Announcer
-Version: 1.1.0
+Version: 1.2.0
 Summary: Announce range closure as sunset approaches
 Home-page: https://github.com/CrazyVikingProductions/range_announcer
 Author: Michael J. Swenson
 Author-email: mikswenson@gmail.com
 Project-URL: Bug Reports, https://github.com/CrazyVikingProductions/range_announcer/issues
 Project-URL: Source, https://github.com/CrazyVikingProductions/range_announcer
 Keywords: sunset closure announce
```

### Comparing `Range_Announcer-1.1.0/src/Range_Announcer.egg-info/SOURCES.txt` & `Range_Announcer-1.2.0/src/Range_Announcer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Range_Announcer-1.1.0/src/range_announcer/__main__.py` & `Range_Announcer-1.2.0/src/range_announcer/__main__.py`

 * *Files identical despite different names*

### Comparing `Range_Announcer-1.1.0/src/range_announcer/announcer.py` & `Range_Announcer-1.2.0/src/range_announcer/announcer.py`

 * *Files identical despite different names*

### Comparing `Range_Announcer-1.1.0/src/range_announcer/sound/15_minutes.mp3` & `Range_Announcer-1.2.0/src/range_announcer/sound/15_minutes.mp3`

 * *Files identical despite different names*

### Comparing `Range_Announcer-1.1.0/src/range_announcer/sound/30_minutes.mp3` & `Range_Announcer-1.2.0/src/range_announcer/sound/30_minutes.mp3`

 * *Files identical despite different names*

### Comparing `Range_Announcer-1.1.0/src/range_announcer/sound/5_minutes.mp3` & `Range_Announcer-1.2.0/src/range_announcer/sound/5_minutes.mp3`

 * *Files identical despite different names*

### Comparing `Range_Announcer-1.1.0/src/range_announcer/sound/BackInBlack.mp3` & `Range_Announcer-1.2.0/src/range_announcer/sound/BackInBlack.mp3`

 * *Files identical despite different names*

### Comparing `Range_Announcer-1.1.0/src/range_announcer/sound/closed.mp3` & `Range_Announcer-1.2.0/src/range_announcer/sound/closed.mp3`

 * *Files identical despite different names*

### Comparing `Range_Announcer-1.1.0/src/range_announcer/sound/complete.wav` & `Range_Announcer-1.2.0/src/range_announcer/sound/complete.wav`

 * *Files identical despite different names*

### Comparing `Range_Announcer-1.1.0/src/range_announcer/sound/one_hour.mp3` & `Range_Announcer-1.2.0/src/range_announcer/sound/one_hour.mp3`

 * *Files identical despite different names*

### Comparing `Range_Announcer-1.1.0/src/range_announcer/sunrise.py` & `Range_Announcer-1.2.0/src/range_announcer/sunrise.py`

 * *Files identical despite different names*

### Comparing `Range_Announcer-1.1.0/src/range_announcer/switch.py` & `Range_Announcer-1.2.0/src/range_announcer/switch.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,7 +45,8 @@
 
     def off(self):
         try:
             logger.info(f'Turning switch off.')
             requests.put(self.off_url, timeout=self.switch_timeout)
         except (requests.exceptions.ConnectTimeout, TimeoutError, ConnectionError) as ex:
             logger.error(f'Switch failed to turn off: {ex}')
+            raise # This is a failure that needs to bubble up
```

### Comparing `Range_Announcer-1.1.0/src/range_announcer/timezone.py` & `Range_Announcer-1.2.0/src/range_announcer/timezone.py`

 * *Files identical despite different names*

