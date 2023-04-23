# Comparing `tmp/spotdl-4.1.7.tar.gz` & `tmp/spotdl-4.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotdl-4.1.7.tar", max compression
+gzip compressed data, was "spotdl-4.1.8.tar", max compression
```

## Comparing `spotdl-4.1.7.tar` & `spotdl-4.1.8.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     1074 2023-04-22 18:24:04.582924 spotdl-4.1.7/LICENSE
--rw-r--r--   0        0        0     5977 2023-04-22 18:24:04.582924 spotdl-4.1.7/README.md
--rw-r--r--   0        0        0     2746 2023-04-22 18:24:04.586924 spotdl-4.1.7/pyproject.toml
--rw-r--r--   0        0        0     4668 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/__init__.py
--rw-r--r--   0        0        0      209 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/__main__.py
--rw-r--r--   0        0        0       58 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/_version.py
--rw-r--r--   0        0        0      186 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/console/__init__.py
--rw-r--r--   0        0        0      598 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/console/download.py
--rw-r--r--   0        0        0     4120 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/console/entry_point.py
--rw-r--r--   0        0        0     5995 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/console/meta.py
--rw-r--r--   0        0        0     2759 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/console/save.py
--rw-r--r--   0        0        0     5067 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/console/sync.py
--rw-r--r--   0        0        0     1702 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/console/url.py
--rw-r--r--   0        0        0     3041 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/console/web.py
--rw-r--r--   0        0        0       80 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/download/__init__.py
--rw-r--r--   0        0        0    27039 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/download/downloader.py
--rw-r--r--   0        0        0    13137 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/download/progress_handler.py
--rw-r--r--   0        0        0       54 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/providers/__init__.py
--rw-r--r--   0        0        0      465 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/providers/audio/__init__.py
--rw-r--r--   0        0        0    11137 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/providers/audio/base.py
--rw-r--r--   0        0        0     2665 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/providers/audio/sliderkz.py
--rw-r--r--   0        0        0     1840 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/providers/audio/youtube.py
--rw-r--r--   0        0        0     2789 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/providers/audio/ytmusic.py
--rw-r--r--   0        0        0      382 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/providers/lyrics/__init__.py
--rw-r--r--   0        0        0     3304 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/providers/lyrics/azlyrics.py
--rw-r--r--   0        0        0     3529 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/providers/lyrics/base.py
--rw-r--r--   0        0        0     3091 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/providers/lyrics/genius.py
--rw-r--r--   0        0        0     2765 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/providers/lyrics/musixmatch.py
--rw-r--r--   0        0        0     1689 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/providers/lyrics/synced.py
--rw-r--r--   0        0        0       38 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/types/__init__.py
--rw-r--r--   0        0        0     3451 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/types/album.py
--rw-r--r--   0        0        0     3101 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/types/artist.py
--rw-r--r--   0        0        0     3871 2023-04-22 18:24:04.586924 spotdl-4.1.7/spotdl/types/options.py
--rw-r--r--   0        0        0     4199 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/types/playlist.py
--rw-r--r--   0        0        0     2186 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/types/result.py
--rw-r--r--   0        0        0     3230 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/types/saved.py
--rw-r--r--   0        0        0     9758 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/types/song.py
--rw-r--r--   0        0        0      103 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/__init__.py
--rw-r--r--   0        0        0     1001 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/archive.py
--rw-r--r--   0        0        0    19690 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/arguments.py
--rw-r--r--   0        0        0     6994 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/config.py
--rw-r--r--   0        0        0     3109 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/console.py
--rw-r--r--   0        0        0      571 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/downloader.py
--rw-r--r--   0        0        0    11688 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/ffmpeg.py
--rw-r--r--   0        0        0    14355 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/formatter.py
--rw-r--r--   0        0        0     7018 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/github.py
--rw-r--r--   0        0        0     5364 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/logging.py
--rw-r--r--   0        0        0      940 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/lrc.py
--rw-r--r--   0        0        0     4144 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/m3u.py
--rw-r--r--   0        0        0    23312 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/matching.py
--rw-r--r--   0        0        0    15525 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/metadata.py
--rw-r--r--   0        0        0    15152 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/search.py
--rw-r--r--   0        0        0     6870 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/spotify.py
--rw-r--r--   0        0        0    28221 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/static.py
--rw-r--r--   0        0        0    15281 2023-04-22 18:24:04.590924 spotdl-4.1.7/spotdl/utils/web.py
--rw-r--r--   0        0        0     8199 1970-01-01 00:00:00.000000 spotdl-4.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-23 15:56:46.642111 spotdl-4.1.8/LICENSE
+-rw-r--r--   0        0        0     5977 2023-04-23 15:56:46.642111 spotdl-4.1.8/README.md
+-rw-r--r--   0        0        0     2747 2023-04-23 15:56:46.646111 spotdl-4.1.8/pyproject.toml
+-rw-r--r--   0        0        0     4668 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/__init__.py
+-rw-r--r--   0        0        0      209 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/__main__.py
+-rw-r--r--   0        0        0       58 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/_version.py
+-rw-r--r--   0        0        0      186 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/console/__init__.py
+-rw-r--r--   0        0        0      598 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/console/download.py
+-rw-r--r--   0        0        0     4120 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/console/entry_point.py
+-rw-r--r--   0        0        0     5995 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/console/meta.py
+-rw-r--r--   0        0        0     2759 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/console/save.py
+-rw-r--r--   0        0        0     5067 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/console/sync.py
+-rw-r--r--   0        0        0     1702 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/console/url.py
+-rw-r--r--   0        0        0     3041 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/console/web.py
+-rw-r--r--   0        0        0       80 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/download/__init__.py
+-rw-r--r--   0        0        0    27263 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/download/downloader.py
+-rw-r--r--   0        0        0    13137 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/download/progress_handler.py
+-rw-r--r--   0        0        0       54 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/providers/__init__.py
+-rw-r--r--   0        0        0      465 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/providers/audio/__init__.py
+-rw-r--r--   0        0        0    11137 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/providers/audio/base.py
+-rw-r--r--   0        0        0     2665 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/providers/audio/sliderkz.py
+-rw-r--r--   0        0        0     1840 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/providers/audio/youtube.py
+-rw-r--r--   0        0        0     2789 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/providers/audio/ytmusic.py
+-rw-r--r--   0        0        0      382 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/providers/lyrics/__init__.py
+-rw-r--r--   0        0        0     3304 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/providers/lyrics/azlyrics.py
+-rw-r--r--   0        0        0     3529 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/providers/lyrics/base.py
+-rw-r--r--   0        0        0     3091 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/providers/lyrics/genius.py
+-rw-r--r--   0        0        0     2765 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/providers/lyrics/musixmatch.py
+-rw-r--r--   0        0        0     1689 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/providers/lyrics/synced.py
+-rw-r--r--   0        0        0       38 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/types/__init__.py
+-rw-r--r--   0        0        0     3451 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/types/album.py
+-rw-r--r--   0        0        0     3101 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/types/artist.py
+-rw-r--r--   0        0        0     3871 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/types/options.py
+-rw-r--r--   0        0        0     4199 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/types/playlist.py
+-rw-r--r--   0        0        0     2186 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/types/result.py
+-rw-r--r--   0        0        0     3230 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/types/saved.py
+-rw-r--r--   0        0        0     9758 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/types/song.py
+-rw-r--r--   0        0        0      103 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/utils/__init__.py
+-rw-r--r--   0        0        0     1001 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/utils/archive.py
+-rw-r--r--   0        0        0    19690 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/utils/arguments.py
+-rw-r--r--   0        0        0     6994 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/utils/config.py
+-rw-r--r--   0        0        0     3109 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/utils/console.py
+-rw-r--r--   0        0        0      571 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/utils/downloader.py
+-rw-r--r--   0        0        0    11688 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/utils/ffmpeg.py
+-rw-r--r--   0        0        0    14271 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/utils/formatter.py
+-rw-r--r--   0        0        0     7018 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/utils/github.py
+-rw-r--r--   0        0        0     5364 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/utils/logging.py
+-rw-r--r--   0        0        0      940 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/utils/lrc.py
+-rw-r--r--   0        0        0     4144 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/utils/m3u.py
+-rw-r--r--   0        0        0    23312 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/utils/matching.py
+-rw-r--r--   0        0        0    15621 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/utils/metadata.py
+-rw-r--r--   0        0        0    15347 2023-04-23 15:56:46.650111 spotdl-4.1.8/spotdl/utils/search.py
+-rw-r--r--   0        0        0     6870 2023-04-23 15:56:46.650111 spotdl-4.1.8/spotdl/utils/spotify.py
+-rw-r--r--   0        0        0    28221 2023-04-23 15:56:46.650111 spotdl-4.1.8/spotdl/utils/static.py
+-rw-r--r--   0        0        0    15281 2023-04-23 15:56:46.650111 spotdl-4.1.8/spotdl/utils/web.py
+-rw-r--r--   0        0        0     8206 1970-01-01 00:00:00.000000 spotdl-4.1.8/PKG-INFO
```

### Comparing `spotdl-4.1.7/LICENSE` & `spotdl-4.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/README.md` & `spotdl-4.1.8/README.md`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/pyproject.toml` & `spotdl-4.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spotdl"
-version = "4.1.7"
+version = "4.1.8"
 description = "Download your Spotify playlists and songs along with album art and metadata"
 license = "MIT"
 authors = ["spotDL Team <spotdladmins@googlegroups.com>"]
 maintainers = ["xnetcat <xnetcat.dev@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/spotDL/spotify-downloader.git"
 homepage = "https://github.com/spotDL/spotify-downloader/"
@@ -42,15 +42,15 @@
 rapidfuzz = "==2.15.1"
 python-slugify = {extras = ["unidecode"], version = "^8.0.1"}
 uvicorn = "^0.21.1"
 pydantic = "^1.10.7"
 fastapi = "^0.95.1"
 platformdirs = "^3.2.0"
 pykakasi = "^2.2.1"
-syncedlyrics = "0.4.0"
+syncedlyrics = "^0.5.0"
 typing-extensions = "^4.5.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 pytest-mock = "^3.10.0"
 pytest-vcr = "^1.0.2"
 pyfakefs = "^5.2.2"
@@ -60,15 +60,15 @@
 mypy = "^1.2.0"
 pylint = "^2.17.2"
 black = "^23.3.0"
 mdformat-gfm = "^0.3.5"
 types-orjson = "^3.6.2"
 types-python-slugify = "^8.0.0.2"
 types-requests = "^2.28.11.17"
-types-setuptools = "^67.6.0.8"
+types-setuptools = "^67.7.0.0"
 types-toml = "^0.10.8.6"
 types-ujson = "^5.7.0.3"
 pyinstaller = "^5.10.1"
 mkdocs = "^1.4.2"
 isort = [
     {version = "^5.11.4", python = "<3.8"},
     {version = "^5.12.0", python = ">=3.8"},
```

### Comparing `spotdl-4.1.7/spotdl/__init__.py` & `spotdl-4.1.8/spotdl/__init__.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/console/download.py` & `spotdl-4.1.8/spotdl/console/download.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/console/entry_point.py` & `spotdl-4.1.8/spotdl/console/entry_point.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/console/meta.py` & `spotdl-4.1.8/spotdl/console/meta.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/console/save.py` & `spotdl-4.1.8/spotdl/console/save.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/console/sync.py` & `spotdl-4.1.8/spotdl/console/sync.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/console/url.py` & `spotdl-4.1.8/spotdl/console/url.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/console/web.py` & `spotdl-4.1.8/spotdl/console/web.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/download/downloader.py` & `spotdl-4.1.8/spotdl/download/downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -488,23 +488,28 @@
                         logger.debug(
                             "Could not remove duplicate file: %s, error: %s",
                             dup_song_path,
                             exc,
                         )
 
             # Find song lyrics and add them to the song object
-            lyrics = self.search_lyrics(song)
-            if lyrics is None:
-                logger.debug(
-                    "No lyrics found for %s, lyrics providers: %s",
-                    song.display_name,
-                    ", ".join([lprovider.name for lprovider in self.lyrics_providers]),
-                )
-            else:
-                song.lyrics = lyrics
+            try:
+                lyrics = self.search_lyrics(song)
+                if lyrics is None:
+                    logger.debug(
+                        "No lyrics found for %s, lyrics providers: %s",
+                        song.display_name,
+                        ", ".join(
+                            [lprovider.name for lprovider in self.lyrics_providers]
+                        ),
+                    )
+                else:
+                    song.lyrics = lyrics
+            except Exception as exc:
+                logger.debug("Could not search for lyrics: %s", exc)
 
             # If the file already exists and we want to overwrite the metadata,
             # we can skip the download
             if file_exists and self.settings["overwrite"] == "metadata":
                 most_recent_duplicate: Optional[Path] = None
                 if dup_song_paths:
                     # Get the most recent duplicate song path and remove the rest
@@ -691,15 +696,15 @@
                         "Removing %s sponsor segments for %s",
                         len(chapters),
                         song.display_name,
                     )
 
                     # Initialize the modify chapters post processor
                     modify_chapters = ModifyChaptersPP(
-                        audio_downloader.audio_handler,
+                        downloader=audio_downloader.audio_handler,
                         remove_sponsor_segments=SPONSOR_BLOCK_CATEGORIES,
                     )
 
                     # Run the post processor to remove the sponsor segments
                     # this returns a list of files to delete
                     files_to_delete, download_info = modify_chapters.run(download_info)
```

### Comparing `spotdl-4.1.7/spotdl/download/progress_handler.py` & `spotdl-4.1.8/spotdl/download/progress_handler.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/providers/audio/base.py` & `spotdl-4.1.8/spotdl/providers/audio/base.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/providers/audio/sliderkz.py` & `spotdl-4.1.8/spotdl/providers/audio/sliderkz.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/providers/audio/youtube.py` & `spotdl-4.1.8/spotdl/providers/audio/youtube.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/providers/audio/ytmusic.py` & `spotdl-4.1.8/spotdl/providers/audio/ytmusic.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/providers/lyrics/azlyrics.py` & `spotdl-4.1.8/spotdl/providers/lyrics/azlyrics.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/providers/lyrics/base.py` & `spotdl-4.1.8/spotdl/providers/lyrics/base.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/providers/lyrics/genius.py` & `spotdl-4.1.8/spotdl/providers/lyrics/genius.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/providers/lyrics/musixmatch.py` & `spotdl-4.1.8/spotdl/providers/lyrics/musixmatch.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/providers/lyrics/synced.py` & `spotdl-4.1.8/spotdl/providers/lyrics/synced.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/types/album.py` & `spotdl-4.1.8/spotdl/types/album.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/types/artist.py` & `spotdl-4.1.8/spotdl/types/artist.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/types/options.py` & `spotdl-4.1.8/spotdl/types/options.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/types/playlist.py` & `spotdl-4.1.8/spotdl/types/playlist.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/types/result.py` & `spotdl-4.1.8/spotdl/types/result.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/types/saved.py` & `spotdl-4.1.8/spotdl/types/saved.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/types/song.py` & `spotdl-4.1.8/spotdl/types/song.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/utils/archive.py` & `spotdl-4.1.8/spotdl/utils/archive.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/utils/arguments.py` & `spotdl-4.1.8/spotdl/utils/arguments.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/utils/config.py` & `spotdl-4.1.8/spotdl/utils/config.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/utils/console.py` & `spotdl-4.1.8/spotdl/utils/console.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/utils/downloader.py` & `spotdl-4.1.8/spotdl/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/utils/ffmpeg.py` & `spotdl-4.1.8/spotdl/utils/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/utils/formatter.py` & `spotdl-4.1.8/spotdl/utils/formatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Module for formatting songs into strings.
 Contains functions to create search queries and song titles
 and file names.
 """
 
+import copy
 import logging
 import re
 from functools import lru_cache
 from pathlib import Path
 from typing import List, Optional
 
 import pykakasi
@@ -299,14 +300,16 @@
     - short: whether to use the short version of the template
     - file_name_length: the maximum length of the file name
 
     ### Returns
     - the formatted string as a Path object
     """
 
+    temp_song = copy.deepcopy(song)
+
     # If template does not contain any of the keys,
     # append {artists} - {title}.{output-ext} to it
     if not any(key in template for key in VARS) and template != "":
         template += "/{artists} - {title}.{output-ext}"
 
     if template == "":
         template = "{artists} - {title}.{output-ext}"
@@ -348,71 +351,76 @@
     if len(file.name) < length_limit:
         # Restrict the filename if needed
         if restrict:
             return restrict_filename(file)
 
         return file
 
-    # If the file name length is greater than ,
-    # and we are already using the short version of the template,
-    # fallback to default template
-    if short is True:
-        # Path template is already short, but we still can't create a file
-        # so we reduce it even further
-        if template == "{artist} - {title}.{output-ext}":
-            if len(song.name) > (length_limit * 0.80):
-                logger.warning(
-                    "%s: File name is too long. Using only part of the song title.",
-                    song.display_name,
-                )
-
-                name_parts = song.name.split(" ")
-                new_name = ""
-                for part in name_parts:
-                    if len(new_name) + len(part) < (length_limit * 0.80):
-                        new_name += part + " "
-                    else:
-                        break
-
-                song.name = new_name.strip()
-            else:
-                logger.warning(
-                    "%s: File name is too long. Using only song title.",
-                    song.display_name,
-                )
-
-            return create_file_name(
-                song=song,
-                template="{title}.{output-ext}",
-                file_extension=file_extension,
-                restrict=restrict,
-                short=short,
-            )
+    if short is False:
+        return create_file_name(
+            song,
+            template,
+            file_extension,
+            restrict=restrict,
+            short=True,
+            file_name_length=length_limit,
+        )
 
-        # This will probably never occur, but just in case
-        if template == "{title}.{output-ext}":
-            raise RecursionError(
-                f'"{song.display_name} is too long to be shortened. File a bug report on GitHub'
-            )
+    # Path template is already short, but we still can't create a file
+    # so we reduce it even further
+    long_artist = len(song.artist) > (length_limit * 0.50)
+    long_title = len(song.name) > (length_limit * 0.50)
+
+    path_separator = "/" if "/" in template else "\\"
+    name_template = template.rsplit(path_separator, 1)[1]
 
+    if long_artist:
         logger.warning(
-            "%s: File name is too long. Using the default template.",
-            song.display_name,
+            "%s: File name is too long. Using only part of song artist.",
+            temp_song.display_name,
         )
 
-        return create_file_name(
-            song=song,
-            template="{artist} - {title}.{output-ext}",
-            file_extension=file_extension,
-            restrict=restrict,
-            short=short,
+        short_artist = temp_song.artist.split(",")[0]
+        temp_song.artist = short_artist
+        if len(temp_song.artist) > (length_limit * 0.50):
+            temp_song.artist = temp_song.artist.split(" ")[0]
+
+    if long_title:
+        logger.warning(
+            "%s: File name is too long. Using only part of the song title.",
+            temp_song.display_name,
         )
 
+        name_parts = temp_song.name.split(" ")
+
+        old_name = temp_song.name
+        temp_song.name = ""
+        for part in name_parts:
+            old_name = temp_song.name
+            temp_song.name += part + " "
+
+            formatted_name = format_query(
+                song=temp_song,
+                template=name_template,
+                santitize=True,
+                file_extension=file_extension,
+                short=True,
+            )
+
+            if len(formatted_name.strip()) > length_limit:
+                temp_song.name = old_name.strip()
+                break
+
     return create_file_name(
-        song, template, file_extension, restrict=restrict, short=True
+        song=temp_song,
+        template=template,
+        file_extension=file_extension,
+        restrict=restrict,
+        short=short,
+        file_name_length=length_limit,
     )
 
 
 def parse_duration(duration: Optional[str]) -> float:
     """
     Convert string value of time (duration: "25:36:59") to a float value of seconds (92219.0)
```

### Comparing `spotdl-4.1.7/spotdl/utils/github.py` & `spotdl-4.1.8/spotdl/utils/github.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/utils/logging.py` & `spotdl-4.1.8/spotdl/utils/logging.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/utils/lrc.py` & `spotdl-4.1.8/spotdl/utils/lrc.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/utils/m3u.py` & `spotdl-4.1.8/spotdl/utils/m3u.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/utils/matching.py` & `spotdl-4.1.8/spotdl/utils/matching.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/utils/metadata.py` & `spotdl-4.1.8/spotdl/utils/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,15 +314,17 @@
                 time_tag = line.split("]", 1)[0] + "]"
                 text = line.replace(time_tag, "")
 
                 time_tag = time_tag.replace("[", "")
                 time_tag = time_tag.replace("]", "")
                 time_tag = time_tag.replace(".", ":")
                 time_tag_vals = time_tag.split(":")
-                if len(time_tag_vals) != 3:
+                if len(time_tag_vals) != 3 or any(
+                    not isinstance(tag, int) for tag in time_tag_vals
+                ):
                     continue
 
                 minute, sec, millisecond = time_tag_vals
                 time = to_ms(min=minute, sec=sec, ms=millisecond)
                 lrc_data.append((text, time))
 
             audio_file.add(USLT(encoding=3, text=song.lyrics))
```

### Comparing `spotdl-4.1.7/spotdl/utils/search.py` & `spotdl-4.1.8/spotdl/utils/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import concurrent.futures
 import json
 import logging
 from pathlib import Path
 from typing import Dict, List, Optional
 
+import requests
 from ytmusicapi import YTMusic
 
 from spotdl.types.album import Album
 from spotdl.types.artist import Artist
 from spotdl.types.playlist import Playlist
 from spotdl.types.saved import Saved
 from spotdl.types.song import Song, SongList
@@ -193,14 +194,17 @@
                 else:
                     for index, song in enumerate(spot_list.songs):
                         song.download_url = ytm_list.songs[index].download_url
 
                     lists.append(spot_list)
         elif "open.spotify.com" in request and "track" in request:
             songs.append(Song.from_url(url=request))
+        elif "https://spotify.link/" in request:
+            resp = requests.head(request, allow_redirects=True, timeout=10)
+            songs.append(Song.from_url(url=resp.url))
         elif "open.spotify.com" in request and "playlist" in request:
             lists.append(Playlist.from_url(request, fetch_songs=False))
         elif "open.spotify.com" in request and "album" in request:
             lists.append(Album.from_url(request, fetch_songs=False))
         elif "open.spotify.com" in request and "artist" in request:
             lists.append(Artist.from_url(request, fetch_songs=False))
         elif "album:" in request:
```

### Comparing `spotdl-4.1.7/spotdl/utils/spotify.py` & `spotdl-4.1.8/spotdl/utils/spotify.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/utils/static.py` & `spotdl-4.1.8/spotdl/utils/static.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/spotdl/utils/web.py` & `spotdl-4.1.8/spotdl/utils/web.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.7/PKG-INFO` & `spotdl-4.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotdl
-Version: 4.1.7
+Version: 4.1.8
 Summary: Download your Spotify playlists and songs along with album art and metadata
 Home-page: https://github.com/spotDL/spotify-downloader/
 License: MIT
 Keywords: spotify,downloader,spotdl,music
 Author: spotDL Team
 Author-email: spotdladmins@googlegroups.com
 Maintainer: xnetcat
@@ -35,15 +35,15 @@
 Requires-Dist: pykakasi (>=2.2.1,<3.0.0)
 Requires-Dist: python-slugify[unidecode] (>=8.0.1,<9.0.0)
 Requires-Dist: pytube (>=12.1.3,<13.0.0)
 Requires-Dist: rapidfuzz (==2.15.1)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: rich (>=13.3.4,<14.0.0)
 Requires-Dist: spotipy (>=2.23.0,<3.0.0)
-Requires-Dist: syncedlyrics (==0.4.0)
+Requires-Dist: syncedlyrics (>=0.5.0,<0.6.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Requires-Dist: uvicorn (>=0.21.1,<0.22.0)
 Requires-Dist: yt-dlp (>=2023.3.4,<2024.0.0)
 Requires-Dist: ytmusicapi (>=0.22.0,<0.23.0) ; python_version < "3.8"
 Requires-Dist: ytmusicapi (>=0.24.0,<0.25.0) ; python_version >= "3.8"
 Project-URL: Documentation, https://spotdl.rtfd.io/en/latest/
 Project-URL: Repository, https://github.com/spotDL/spotify-downloader.git
```

