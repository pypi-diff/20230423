# Comparing `tmp/spotube-0.5.2.tar.gz` & `tmp/spotube-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotube-0.5.2.tar", max compression
+gzip compressed data, was "spotube-0.5.3.tar", max compression
```

## Comparing `spotube-0.5.2.tar` & `spotube-0.5.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3184 2023-03-30 19:00:39.900959 spotube-0.5.2/LICENSE
--rw-r--r--   0        0        0     6178 2023-03-30 19:00:39.900959 spotube-0.5.2/README.md
--rw-r--r--   0        0        0      750 2023-03-30 19:04:44.495054 spotube-0.5.2/pyproject.toml
--rw-r--r--   0        0        0       55 2023-03-30 19:00:39.904959 spotube-0.5.2/spotube_package/__init__.py
--rw-r--r--   0        0        0     3165 2023-03-30 19:00:39.904959 spotube-0.5.2/spotube_package/downloader_class.py
--rw-r--r--   0        0        0    15387 2023-03-30 19:00:39.904959 spotube-0.5.2/spotube_package/downloader_utils.py
--rw-r--r--   0        0        0     7263 1970-01-01 00:00:00.000000 spotube-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     3184 2023-04-23 18:05:07.535578 spotube-0.5.3/LICENSE
+-rw-r--r--   0        0        0     6178 2023-04-23 18:05:07.535578 spotube-0.5.3/README.md
+-rw-r--r--   0        0        0      742 2023-04-23 18:08:28.522615 spotube-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0       55 2023-04-23 18:05:07.535578 spotube-0.5.3/spotube/__init__.py
+-rw-r--r--   0        0        0     3165 2023-04-23 18:05:07.535578 spotube-0.5.3/spotube/downloader_class.py
+-rw-r--r--   0        0        0    15422 2023-04-23 18:05:07.535578 spotube-0.5.3/spotube/downloader_utils.py
+-rw-r--r--   0        0        0     7263 1970-01-01 00:00:00.000000 spotube-0.5.3/PKG-INFO
```

### Comparing `spotube-0.5.2/LICENSE` & `spotube-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spotube-0.5.2/README.md` & `spotube-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `spotube-0.5.2/pyproject.toml` & `spotube-0.5.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "spotube"
-version = "0.5.2"
+version = "0.5.3"
 description = "A Python package to download Spotify playlists locally including the cover art, metadata and lyrics by leveraging the Spotify, YouTube and Genius APIs."
 authors = ["GiorgosNik <giorgosnl17@gmail.com>"]
 license = "Free for non-commercial use"
 readme = "README.md"
 repository = 'https://github.com/GiorgosNik/spotube-package'
-packages = [{include = "spotube_package"}]
+packages = [{include = "spotube"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 eyed3 = "^0.9.7"
 lyricsgenius = "^3.0.1"
 pydub = "^0.25.1"
 pytest = "^7.2.2"
```

### Comparing `spotube-0.5.2/spotube_package/downloader_class.py` & `spotube-0.5.3/spotube/downloader_class.py`

 * *Files identical despite different names*

### Comparing `spotube-0.5.2/spotube_package/downloader_utils.py` & `spotube-0.5.3/spotube/downloader_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -341,15 +341,15 @@
             subprocess.Popen(
                 "which ffmpeg",
                 shell=True,
                 stdout=subprocess.PIPE,
                 stderr=subprocess.PIPE,
             ).communicate()[0]
         )
-        if p == "b''":
+        if p == "b''" and not os.path.exists("./ffmpeg"):
             return False
 
     return True
 
 
 # Save the state of the worker thread based on the message
 def handle_message(downloader, message):
```

### Comparing `spotube-0.5.2/PKG-INFO` & `spotube-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotube
-Version: 0.5.2
+Version: 0.5.3
 Summary: A Python package to download Spotify playlists locally including the cover art, metadata and lyrics by leveraging the Spotify, YouTube and Genius APIs.
 Home-page: https://github.com/GiorgosNik/spotube-package
 License: Free for non-commercial use
 Author: GiorgosNik
 Author-email: giorgosnl17@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
```

