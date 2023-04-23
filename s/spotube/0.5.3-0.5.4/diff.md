# Comparing `tmp/spotube-0.5.3.tar.gz` & `tmp/spotube-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotube-0.5.3.tar", max compression
+gzip compressed data, was "spotube-0.5.4.tar", max compression
```

## Comparing `spotube-0.5.3.tar` & `spotube-0.5.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3184 2023-04-23 18:05:07.535578 spotube-0.5.3/LICENSE
--rw-r--r--   0        0        0     6178 2023-04-23 18:05:07.535578 spotube-0.5.3/README.md
--rw-r--r--   0        0        0      742 2023-04-23 18:08:28.522615 spotube-0.5.3/pyproject.toml
--rw-r--r--   0        0        0       55 2023-04-23 18:05:07.535578 spotube-0.5.3/spotube/__init__.py
--rw-r--r--   0        0        0     3165 2023-04-23 18:05:07.535578 spotube-0.5.3/spotube/downloader_class.py
--rw-r--r--   0        0        0    15422 2023-04-23 18:05:07.535578 spotube-0.5.3/spotube/downloader_utils.py
--rw-r--r--   0        0        0     7263 1970-01-01 00:00:00.000000 spotube-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     3184 2023-04-23 19:06:37.024075 spotube-0.5.4/LICENSE
+-rw-r--r--   0        0        0     6178 2023-04-23 19:06:37.024075 spotube-0.5.4/README.md
+-rw-r--r--   0        0        0      742 2023-04-23 19:10:07.551084 spotube-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0       40 2023-04-23 19:06:37.024075 spotube-0.5.4/spotube/__init__.py
+-rw-r--r--   0        0        0     3196 2023-04-23 19:06:37.024075 spotube-0.5.4/spotube/downloader_class.py
+-rw-r--r--   0        0        0    15638 2023-04-23 19:06:37.024075 spotube-0.5.4/spotube/downloader_utils.py
+-rw-r--r--   0        0        0     7263 1970-01-01 00:00:00.000000 spotube-0.5.4/PKG-INFO
```

### Comparing `spotube-0.5.3/LICENSE` & `spotube-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spotube-0.5.3/README.md` & `spotube-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `spotube-0.5.3/pyproject.toml` & `spotube-0.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spotube"
-version = "0.5.3"
+version = "0.5.4"
 description = "A Python package to download Spotify playlists locally including the cover art, metadata and lyrics by leveraging the Spotify, YouTube and Genius APIs."
 authors = ["GiorgosNik <giorgosnl17@gmail.com>"]
 license = "Free for non-commercial use"
 readme = "README.md"
 repository = 'https://github.com/GiorgosNik/spotube-package'
 packages = [{include = "spotube"}]
```

### Comparing `spotube-0.5.3/spotube/downloader_class.py` & `spotube-0.5.4/spotube/downloader_class.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 import threading
 import queue
-import spotube_package.downloader_utils as utils
+from . import downloader_utils as utils
 import os
 import subprocess
 from zipfile import ZipFile
 import urllib.request
 
 class downloader:
     def __init__(
         self,
         spotify_client_id,
         spotify_client_secret,
         genius_api_key,
         directory="./Songs",
+        display_bar=True
     ):
         # Initialise the tracking values
         self.progress = 0
         self.working = False
         self.total = None
         self.current_song = None
         self.eta = None
         self.thread = None
         self.spotify_client_id = spotify_client_id
         self.spotify_client_secret = spotify_client_secret
         self.genius_api_key = genius_api_key
         self.directory = directory
+        self.display_bar = display_bar
 
         # Set the channel that will handle the messages from the worker
         self.channel = queue.Queue()
 
         # Set the channel that will handle the messages from the worker
         self.termination_channel = queue.Queue()
 
         # Perform authentication for LyricsGenius and Spotify APIs
         self.tokens = utils.auth_handler(
             self.spotify_client_id, self.spotify_client_secret, self.genius_api_key
         )
 
-        # For testing
-        # utils.download_ffmpeg()
-
         if not utils.ffmpeg_installed():  # pragma: no cover
             os_name = utils.get_os_name()
             utils.download_ffmpeg(os_type = os_name)
 
     def set_directory(self, directory):
         self.directory = directory
 
@@ -53,14 +52,15 @@
             target=utils.download_playlist,
             args=[
                 link,
                 self.tokens,
                 self.channel,
                 self.termination_channel,
                 self.directory,
+                self.display_bar
             ],
         )
         self.working = True
         self.thread.start()
 
     def stop_downloader(self):
         self.termination_channel.put("EXIT")
```

### Comparing `spotube-0.5.3/spotube/downloader_utils.py` & `spotube-0.5.4/spotube/downloader_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,33 +177,48 @@
         "duration": duration,
         "url": cover_art,
     }
 
     return info_dict
 
 
-def download_playlist(playlist_url, tokens, channel, termination_channel, directory):
+def download_playlist(
+    playlist_url, tokens, channel, termination_channel, directory, display_bar=True
+):
     # Set up the folder for the songs
     if not os.path.isdir(directory):
         os.mkdir(directory)
 
     audio_downloader = create_audio_downloader(directory)
 
     songs = get_songs(playlist_url, tokens["spotify"])
 
+    if display_bar:
+        file = None
+    else:
+        file = open(os.devnull, "w")
+
     # Set the tqdm progress bar
     playlist_size = len(songs)
     playlist_progress = tqdm(
-        total=playlist_size, desc="Playlist Progress", position=0, leave=False
+        total=playlist_size,
+        desc="Playlist Progress",
+        position=0,
+        leave=False,
+        file=file,
     )
 
     for song in songs:
         # Set song progress bar
         song_progress = tqdm(
-            total=4, desc=song["track"]["name"], position=1, leave=False
+            total=4,
+            desc=song["track"]["name"],
+            position=1,
+            leave=False,
+            file=file,
         )
 
         # Retrieve Formatted Song Data
         song_progress.set_description(song_progress.desc + ": Formatting Information")
         song_progress.update(n=1)
         info_dict = format_song_data(song)
```

### Comparing `spotube-0.5.3/PKG-INFO` & `spotube-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotube
-Version: 0.5.3
+Version: 0.5.4
 Summary: A Python package to download Spotify playlists locally including the cover art, metadata and lyrics by leveraging the Spotify, YouTube and Genius APIs.
 Home-page: https://github.com/GiorgosNik/spotube-package
 License: Free for non-commercial use
 Author: GiorgosNik
 Author-email: giorgosnl17@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
```

