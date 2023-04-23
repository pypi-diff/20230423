# Comparing `tmp/syncedlyrics-0.4.0.tar.gz` & `tmp/syncedlyrics-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncedlyrics-0.4.0.tar", max compression
+gzip compressed data, was "syncedlyrics-0.5.0.tar", max compression
```

## Comparing `syncedlyrics-0.4.0.tar` & `syncedlyrics-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,23 @@
--rw-r--r--   0        0        0     1081 2022-11-26 15:55:28.589240 syncedlyrics-0.4.0/LICENSE
--rw-r--r--   0        0        0      891 2023-01-29 17:51:59.652528 syncedlyrics-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1279 2023-01-29 17:23:04.973870 syncedlyrics-0.4.0/README.md
--rw-r--r--   0        0        0     1895 2023-01-29 17:11:26.288145 syncedlyrics-0.4.0/syncedlyrics/__init__.py
--rw-r--r--   0        0        0       91 2022-11-27 19:01:53.954957 syncedlyrics-0.4.0/syncedlyrics/__main__.py
--rw-r--r--   0        0        0     1080 2023-01-29 15:17:45.434783 syncedlyrics-0.4.0/syncedlyrics/cli.py
--rw-r--r--   0        0        0      165 2023-01-29 16:42:25.280838 syncedlyrics-0.4.0/syncedlyrics/providers/__init__.py
--rw-r--r--   0        0        0     1072 2023-01-29 15:48:04.679364 syncedlyrics-0.4.0/syncedlyrics/providers/base.py
--rw-r--r--   0        0        0     1836 2023-01-21 13:44:04.510093 syncedlyrics-0.4.0/syncedlyrics/providers/deezer.py
--rw-r--r--   0        0        0     1617 2023-01-29 17:22:23.265068 syncedlyrics-0.4.0/syncedlyrics/providers/lyricsify.py
--rw-r--r--   0        0        0     1325 2023-01-29 17:22:14.380292 syncedlyrics-0.4.0/syncedlyrics/providers/megalobiz.py
--rw-r--r--   0        0        0     3432 2023-01-29 17:22:03.333621 syncedlyrics-0.4.0/syncedlyrics/providers/netease.py
--rw-r--r--   0        0        0      796 2022-11-27 20:02:30.397213 syncedlyrics-0.4.0/syncedlyrics/providers/spotify.py
--rw-r--r--   0        0        0      978 2023-01-29 16:26:47.552975 syncedlyrics-0.4.0/syncedlyrics/utils.py
--rw-r--r--   0        0        0     2163 1970-01-01 00:00:00.000000 syncedlyrics-0.4.0/setup.py
--rw-r--r--   0        0        0     2307 1970-01-01 00:00:00.000000 syncedlyrics-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-04-12 14:05:47.000000 syncedlyrics-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1150 2023-04-12 15:28:36.000000 syncedlyrics-0.5.0/README.md
+-rw-r--r--   0        0        0      876 2023-04-23 15:28:24.000000 syncedlyrics-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1805 2023-04-23 15:25:45.000000 syncedlyrics-0.5.0/syncedlyrics/__init__.py
+-rw-r--r--   0        0        0       87 2023-04-12 14:05:47.000000 syncedlyrics-0.5.0/syncedlyrics/__main__.py
+-rw-r--r--   0        0        0     1032 2023-04-12 14:05:47.000000 syncedlyrics-0.5.0/syncedlyrics/cli.py
+-rw-r--r--   0        0        0      194 2023-04-12 14:49:44.000000 syncedlyrics-0.5.0/syncedlyrics/providers/__init__.py
+-rw-r--r--   0        0        0      423 2023-04-12 14:51:11.000000 syncedlyrics-0.5.0/syncedlyrics/providers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1563 2023-04-12 14:52:47.000000 syncedlyrics-0.5.0/syncedlyrics/providers/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0     1940 2023-04-12 14:52:47.000000 syncedlyrics-0.5.0/syncedlyrics/providers/__pycache__/deezer.cpython-39.pyc
+-rw-r--r--   0        0        0     2099 2023-04-12 14:52:47.000000 syncedlyrics-0.5.0/syncedlyrics/providers/__pycache__/lyricsify.cpython-39.pyc
+-rw-r--r--   0        0        0     1402 2023-04-12 14:53:36.000000 syncedlyrics-0.5.0/syncedlyrics/providers/__pycache__/megalobiz.cpython-39.pyc
+-rw-r--r--   0        0        0     1662 2023-04-16 10:26:21.000000 syncedlyrics-0.5.0/syncedlyrics/providers/__pycache__/musixmatch.cpython-39.pyc
+-rw-r--r--   0        0        0     3578 2023-04-12 14:51:11.000000 syncedlyrics-0.5.0/syncedlyrics/providers/__pycache__/netease.cpython-39.pyc
+-rw-r--r--   0        0        0     1040 2023-04-12 14:05:47.000000 syncedlyrics-0.5.0/syncedlyrics/providers/base.py
+-rw-r--r--   0        0        0     1788 2023-04-12 14:05:47.000000 syncedlyrics-0.5.0/syncedlyrics/providers/deezer.py
+-rw-r--r--   0        0        0     1589 2023-04-23 15:25:09.000000 syncedlyrics-0.5.0/syncedlyrics/providers/lyricsify.py
+-rw-r--r--   0        0        0     1269 2023-04-12 14:05:47.000000 syncedlyrics-0.5.0/syncedlyrics/providers/megalobiz.py
+-rw-r--r--   0        0        0     1352 2023-04-23 15:27:17.000000 syncedlyrics-0.5.0/syncedlyrics/providers/musixmatch.py
+-rw-r--r--   0        0        0     3371 2023-04-12 14:05:47.000000 syncedlyrics-0.5.0/syncedlyrics/providers/netease.py
+-rw-r--r--   0        0        0      771 2023-04-12 14:05:47.000000 syncedlyrics-0.5.0/syncedlyrics/providers/spotify.py
+-rw-r--r--   0        0        0      946 2023-04-12 14:05:47.000000 syncedlyrics-0.5.0/syncedlyrics/utils.py
+-rw-r--r--   0        0        0     2222 1970-01-01 00:00:00.000000 syncedlyrics-0.5.0/PKG-INFO
```

### Comparing `syncedlyrics-0.4.0/LICENSE` & `syncedlyrics-0.5.0/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Momo
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2022 Momo
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `syncedlyrics-0.4.0/pyproject.toml` & `syncedlyrics-0.5.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-[tool.poetry]
-name = "syncedlyrics"
-version = "0.4.0"
-description = "Get an LRC format (synchronized) lyrics for your music"
-repository = "https://github.com/rtcq/syncedlyrics"
-urls = { "Bug Tracker" = "https://github.com/rtcq/syncedlyrics/issues" }
-authors = ["Momo <lo3me@proton.me>"]
-license = "MIT"
-readme = "README.md"
-classifiers = [
-    "Topic :: Multimedia :: Sound/Audio",
-    "Topic :: Multimedia :: Sound/Audio :: Players",
-    "Topic :: Multimedia :: Sound/Audio :: Speech",
-]
-
-[tool.poetry.dependencies]
-python = "^3.7"
-requests = "^2.28.1"
-rapidfuzz = "^2.13.2"
-beautifulsoup4 = "^4.11.1"
-
-[tool.poetry.dev-dependencies]
-black = "*"
-
-[tool.poetry.scripts]
-syncedlyrics = "syncedlyrics.cli:cli_handler"
-
-[tool.poetry.group.dev.dependencies]
-black = "^22.12.0"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "syncedlyrics"
+version = "0.5.0"
+description = "Get an LRC format (synchronized) lyrics for your music"
+repository = "https://github.com/rtcq/syncedlyrics"
+urls = { "Bug Tracker" = "https://github.com/rtcq/syncedlyrics/issues" }
+authors = ["Momo <lo3me@proton.me>"]
+license = "MIT"
+readme = "README.md"
+classifiers = [
+    "Topic :: Multimedia :: Sound/Audio",
+    "Topic :: Multimedia :: Sound/Audio :: Players",
+    "Topic :: Multimedia :: Sound/Audio :: Speech",
+]
+
+[tool.poetry.dependencies]
+python = "^3.7"
+requests = "^2.28.1"
+rapidfuzz = "^2.13.2"
+beautifulsoup4 = "^4.11.1"
+
+[tool.poetry.dev-dependencies]
+black = "*"
+
+[tool.poetry.scripts]
+syncedlyrics = "syncedlyrics.cli:cli_handler"
+
+[tool.poetry.group.dev.dependencies]
+black = "^22.12.0"
+pytest = "^7.3.0"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `syncedlyrics-0.4.0/README.md` & `syncedlyrics-0.5.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,42 @@
-# syncedlyrics
- Get an LRC format (synchronized) lyrics for your music.
- 
- [![Downloads](https://static.pepy.tech/badge/syncedlyrics/month)](https://pepy.tech/project/syncedlyrics)
-
-## Installation
-```
-pip install syncedlyrics
-```
-## Usage
-### CLI
-```
-syncedlyrics "SEARCH_TERM"
-```
-#### Available Options
-| Flag | Description |
-| --- | --- |
-| `-o` | Path to save `.lrc` lyrics, default="{search_term}.lrc" |
-| `-v` | Use this flag to show the logs |
-| `--allow-plain` | Return a plain text (not synced) lyrics if not LRC was found |
-
-### Python
-```py
-import syncedlyrics
-lrc = syncedlyrics.search("[TRACK_NAME] [ARTIST_NAME]")
-```
-Or with options:
-```py
-syncedlyrics.search("...", allow_plain_format=True, save_path="{search_term}_1234.lrc", providers=["NetEase"])
-```
-
-## Providers
-- [NetEase](https://music.163.com/)
-- [Lyricsify](https://www.lyricsify.com/)
-- [Megalobiz](https://www.megalobiz.com/)
-- ~~[Deezer](https://deezer.com/)~~ (Currently broken, PR is appreciated)
-
-Feel free to suggest more providers please.
-
-## License
-[MIT](https://github.com/rtcq/syncedlyrics/blob/master/LICENSE)
-
-## Notes
-I also found a [repo](https://github.com/fashni/MxLRC) for Musixmatch API, but it has annoying API rate limits at the moment
+# syncedlyrics
+ Get an LRC format (synchronized) lyrics for your music.
+ 
+ [![Downloads](https://static.pepy.tech/badge/syncedlyrics/month)](https://pepy.tech/project/syncedlyrics)
+
+## Installation
+```
+pip install syncedlyrics
+```
+## Usage
+### CLI
+```
+syncedlyrics "SEARCH_TERM"
+```
+#### Available Options
+| Flag | Description |
+| --- | --- |
+| `-o` | Path to save `.lrc` lyrics, default="{search_term}.lrc" |
+| `-v` | Use this flag to show the logs |
+| `--allow-plain` | Return a plain text (not synced) lyrics if no LRC format was found |
+
+### Python
+```py
+import syncedlyrics
+lrc = syncedlyrics.search("[TRACK_NAME] [ARTIST_NAME]")
+```
+Or with options:
+```py
+syncedlyrics.search("...", allow_plain_format=True, save_path="{search_term}_1234.lrc", providers=["NetEase"])
+```
+
+## Providers
+- [Musixmatch](https://www.musixmatch.com/)
+- [Lyricsify](https://www.lyricsify.com/)
+- [NetEase](https://music.163.com/)
+- [Megalobiz](https://www.megalobiz.com/)
+- ~~[Deezer](https://deezer.com/)~~ (Currently broken, PR is appreciated)
+
+Feel free to suggest more providers please.
+
+## License
+[MIT](https://github.com/rtcq/syncedlyrics/blob/master/LICENSE)
```

### Comparing `syncedlyrics-0.4.0/syncedlyrics/__init__.py` & `syncedlyrics-0.5.0/syncedlyrics/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,51 @@
-"""
-Search for an LRC format (synchronized lyrics) of a music.
-
-```py
-import syncedlyrics
-lrc_text = syncedlyrics.search("[TRACK_NAME] [ARTIST_NAME]")
-```
-"""
-
-from typing import Optional, List
-import logging
-from .providers import NetEase, Lyricsify, Megalobiz
-from .utils import is_lrc_valid, save_lrc_file
-
-logger = logging.getLogger(__name__)
-
-
-def search(
-    search_term: str,
-    allow_plain_format: bool = False,
-    save_path: str = None,
-    providers: List[str] = None,
-) -> Optional[str]:
-    """
-    Returns the synced lyrics of the song in [LRC](https://en.wikipedia.org/wiki/LRC_(file_format)) format if found.
-    ### Arguments
-    - `search_term`: The search term to find the track.
-    - `allow_normal_format`: Return a plain text (not synced) lyrics if not LRC was found.
-    - `save_path`: Path to save `.lrc` lyrics. No saving if `None`.
-    - `providers`: A list of provider names to include in searching; loops over all the providers as soon as an LRC is found. Supported providers: `Lyricsify`, `NetEase`
-    `Megalobiz`
-    """
-    _providers = [Lyricsify(), NetEase(), Megalobiz()]
-    if providers:
-        # Filtering the providers
-        _providers = [p for p in _providers if p.__class__.__name__ in providers]
-    lrc = None
-    for provider in _providers:
-        logger.debug(f"Looking for an LRC on {provider.__class__.__name__}")
-        lrc = provider.get_lrc(search_term)
-        if is_lrc_valid(lrc, allow_plain_format):
-            logger.info(
-                f'synced-lyrics found for "{search_term}" on {provider.__class__.__name__}'
-            )
-            break
-    if not lrc:
-        logger.info(f'No synced-lyrics found for "{search_term}" :(')
-        return
-    if save_path:
-        save_path = save_path.format(search_term=search_term)
-        save_lrc_file(save_path, lrc)
-    return lrc
+"""
+Search for an LRC format (synchronized lyrics) of a music.
+
+```py
+import syncedlyrics
+lrc_text = syncedlyrics.search("[TRACK_NAME] [ARTIST_NAME]")
+```
+"""
+
+from typing import Optional, List
+import logging
+from .providers import NetEase, Lyricsify, Megalobiz, Musixmatch
+from .utils import is_lrc_valid, save_lrc_file
+
+logger = logging.getLogger(__name__)
+
+
+def search(
+    search_term: str,
+    allow_plain_format: bool = False,
+    save_path: str = None,
+    providers: List[str] = None,
+) -> Optional[str]:
+    """
+    Returns the synced lyrics of the song in [LRC](https://en.wikipedia.org/wiki/LRC_(file_format)) format if found.
+    ### Arguments
+    - `search_term`: The search term to find the track
+    - `allow_normal_format`: Return a plain text (not synced) lyrics if not LRC was found
+    - `save_path`: Path to save `.lrc` lyrics. No saving if `None`
+    - `providers`: A list of provider names to include in searching; loops over all the providers as soon as an LRC is found
+    """
+    _providers = [Lyricsify(), Musixmatch(), NetEase(), Megalobiz()]
+    if providers:
+        # Filtering the providers
+        _providers = [p for p in _providers if p.__class__.__name__ in providers]
+    lrc = None
+    for provider in _providers:
+        logger.debug(f"Looking for an LRC on {provider.__class__.__name__}")
+        lrc = provider.get_lrc(search_term)
+        if is_lrc_valid(lrc, allow_plain_format):
+            logger.info(
+                f'synced-lyrics found for "{search_term}" on {provider.__class__.__name__}'
+            )
+            break
+    if not lrc:
+        logger.info(f'No synced-lyrics found for "{search_term}" :(')
+        return
+    if save_path:
+        save_path = save_path.format(search_term=search_term)
+        save_lrc_file(save_path, lrc)
+    return lrc
```

### Comparing `syncedlyrics-0.4.0/syncedlyrics/providers/base.py` & `syncedlyrics-0.5.0/syncedlyrics/providers/base.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-import requests
-from typing import Optional
-
-
-class LRCProvider:
-    """
-    Base class for all of the synced (LRC format) lyrics providers.
-    """
-
-    session = requests.Session()
-
-    def __init__(self) -> None:
-        self.session.headers.update(
-            {
-                "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36"
-            }
-        )
-
-    def get_lrc_by_id(self, track_id: str) -> Optional[str]:
-        """
-        Returns the synced lyrics of the song in [LRC](https://en.wikipedia.org/wiki/LRC_(file_format)) format if found.
-
-        ### Arguments
-        - track_id: The ID of the track defined in the provider database. e.g. Spotify/Deezer track ID
-        """
-        raise NotImplementedError
-
-    def get_lrc(self, search_term: str) -> Optional[str]:
-        """
-        Returns the synced lyrics of the song in [LRC](https://en.wikipedia.org/wiki/LRC_(file_format)) format if found.
-        """
-        raise NotImplementedError
+import requests
+from typing import Optional
+
+
+class LRCProvider:
+    """
+    Base class for all of the synced (LRC format) lyrics providers.
+    """
+
+    session = requests.Session()
+
+    def __init__(self) -> None:
+        self.session.headers.update(
+            {
+                "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36"
+            }
+        )
+
+    def get_lrc_by_id(self, track_id: str) -> Optional[str]:
+        """
+        Returns the synced lyrics of the song in [LRC](https://en.wikipedia.org/wiki/LRC_(file_format)) format if found.
+
+        ### Arguments
+        - track_id: The ID of the track defined in the provider database. e.g. Spotify/Deezer track ID
+        """
+        raise NotImplementedError
+
+    def get_lrc(self, search_term: str) -> Optional[str]:
+        """
+        Returns the synced lyrics of the song in [LRC](https://en.wikipedia.org/wiki/LRC_(file_format)) format if found.
+        """
+        raise NotImplementedError
```

### Comparing `syncedlyrics-0.4.0/syncedlyrics/providers/deezer.py` & `syncedlyrics-0.5.0/syncedlyrics/providers/deezer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,50 @@
-"""Deezer LRC provider (API powered by LyricFind)"""
-
-from typing import Optional
-from .base import LRCProvider
-
-# Currently broken
-# TODO: Fix invalid CSRF token
-
-# Mostly based on https://gist.github.com/akashrchandran/95915c2081815397c454bd8aa4a118b5
-
-class Deezer(LRCProvider):
-    """Deezer provider class"""
-
-    SEARCH_ENDPOINT = "https://api.deezer.com/search?q="
-    API_ENDPOINT = "http://www.deezer.com/ajax/gw-light.php"
-    token = "null"
-
-    def __init__(self) -> None:
-        super().__init__()
-        self.token = self._api_call("deezer.getUserData")["results"]["checkForm"]
-
-    def _api_call(self, method: str, json=None) -> dict:
-        params = {
-            "api_version": "1.0",
-            "api_token": self.token,
-            "input": "3",
-            "method": method,
-        }
-        response = self.session.post(self.API_ENDPOINT, params=params, json=json)
-        return response.json()
-
-    def get_lrc_by_id(self, track_id: str) -> Optional[str]:
-        lrc_response = self._api_call("song.getLyrics", json={"sng_id": track_id})
-        lrc_json_objs = lrc_response["results"].get("LYRICS_SYNC_JSON")
-        if not lrc_json_objs:
-            # Returning the plain text lyrics
-            return lrc_response["results"].get("LYRICS_TEXT")
-        lrc = ""
-        for chunk in lrc_json_objs:
-            if chunk.get("lrc_timestamp") and chunk.get("line"):
-                lrc += f"{chunk['lrc_timestamp']} {chunk['line']}\n"
-        return lrc or None
-
-    def get_lrc(self, search_term: str) -> Optional[str]:
-        search_results = self.session.get(self.SEARCH_ENDPOINT + search_term).json()
-        if not search_results.get("data"):
-            return
-        song = search_results.get("data")[0]
-        return self.get_lrc_by_id(song["id"])
+"""Deezer LRC provider (API powered by LyricFind)"""
+
+from typing import Optional
+from .base import LRCProvider
+
+# Currently broken
+# TODO: Fix invalid CSRF token
+
+# Mostly based on https://gist.github.com/akashrchandran/95915c2081815397c454bd8aa4a118b5
+
+
+class Deezer(LRCProvider):
+    """Deezer provider class"""
+
+    SEARCH_ENDPOINT = "https://api.deezer.com/search?q="
+    API_ENDPOINT = "http://www.deezer.com/ajax/gw-light.php"
+    token = "null"
+
+    def __init__(self) -> None:
+        super().__init__()
+        self.token = self._api_call("deezer.getUserData")["results"]["checkForm"]
+
+    def _api_call(self, method: str, json=None) -> dict:
+        params = {
+            "api_version": "1.0",
+            "api_token": self.token,
+            "input": "3",
+            "method": method,
+        }
+        response = self.session.post(self.API_ENDPOINT, params=params, json=json)
+        return response.json()
+
+    def get_lrc_by_id(self, track_id: str) -> Optional[str]:
+        lrc_response = self._api_call("song.getLyrics", json={"sng_id": track_id})
+        lrc_json_objs = lrc_response["results"].get("LYRICS_SYNC_JSON")
+        if not lrc_json_objs:
+            # Returning the plain text lyrics
+            return lrc_response["results"].get("LYRICS_TEXT")
+        lrc = ""
+        for chunk in lrc_json_objs:
+            if chunk.get("lrc_timestamp") and chunk.get("line"):
+                lrc += f"{chunk['lrc_timestamp']} {chunk['line']}\n"
+        return lrc or None
+
+    def get_lrc(self, search_term: str) -> Optional[str]:
+        search_results = self.session.get(self.SEARCH_ENDPOINT + search_term).json()
+        if not search_results.get("data"):
+            return
+        song = search_results.get("data")[0]
+        return self.get_lrc_by_id(song["id"])
```

### Comparing `syncedlyrics-0.4.0/syncedlyrics/providers/lyricsify.py` & `syncedlyrics-0.5.0/syncedlyrics/providers/lyricsify.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-"""Lyricsify (lyricsify.com) LRC provider"""
-
-from typing import Optional
-from bs4 import SoupStrainer
-import rapidfuzz
-from .base import LRCProvider
-from ..utils import generate_bs4_soup
-
-
-class Lyricsify(LRCProvider):
-    """Lyricsify LRC provider class"""
-
-    ROOT_URL = "https://www.lyricsify.com"
-    SEARCH_ENDPOINT = ROOT_URL + "/search?q="
-
-    def __init__(self) -> None:
-        super().__init__()
-        self.parser = "html.parser"
-
-    def get_lrc(self, search_term: str) -> Optional[str]:
-        url = self.SEARCH_ENDPOINT + search_term.replace(" ", "+")
-
-        # Just processing the `a` tags whose `href` attribute starts with /lyric/
-        # and whose text is similar to the query too. https://github.com/maxbachmann/RapidFuzz#scorers
-        _t = lambda s: s.lower().replace("-", "")
-        text_match = lambda t: rapidfuzz.fuzz.token_sort_ratio(_t(search_term), _t(t))
-        href_match = lambda h: h.startswith("/lyric/")
-        a_tags_boud = SoupStrainer("a", href=href_match)
-        soup = generate_bs4_soup(self.session, url, parse_only=a_tags_boud)
-        a_tag = soup.find_all("a", string=lambda t: text_match(t) > 80, limit=4)
-        if not a_tag:
-            return None
-
-        # The one with the highest similarity score
-        a_tag = sorted(a_tag, key=lambda tag: text_match(tag.string))[-1]
-
-        # Scraping from the LRC page
-        lrc_id = a_tag["href"].split(".")[-1]
-        soup = generate_bs4_soup(self.session, self.ROOT_URL + a_tag["href"])
-        return soup.find("div", {"id": f"lyrics_{lrc_id}_details"}).get_text()
+"""Lyricsify (lyricsify.com) LRC provider"""
+
+from typing import Optional
+from bs4 import SoupStrainer
+import rapidfuzz
+from .base import LRCProvider
+from ..utils import generate_bs4_soup
+
+
+class Lyricsify(LRCProvider):
+    """Lyricsify LRC provider class"""
+
+    ROOT_URL = "https://www.lyricsify.com"
+    SEARCH_ENDPOINT = ROOT_URL + "/search?q="
+
+    def __init__(self) -> None:
+        super().__init__()
+        self.parser = "html.parser"
+
+    def get_lrc(self, search_term: str) -> Optional[str]:
+        url = self.SEARCH_ENDPOINT + search_term.replace(" ", "+")
+
+        # Just processing the `a` tags whose `href` attribute starts with /lyric/
+        # and whose text is similar to the query too. https://github.com/maxbachmann/RapidFuzz#scorers
+        _t = lambda s: s.lower().replace("-", "") if s else s
+        text_match = lambda t: rapidfuzz.fuzz.token_sort_ratio(_t(search_term), _t(t))
+        href_match = lambda h: h.startswith("/lyric/")
+        a_tags_boud = SoupStrainer("a", href=href_match)
+        soup = generate_bs4_soup(self.session, url, parse_only=a_tags_boud)
+        a_tag = soup.find_all("a", string=lambda t: text_match(t) > 80, limit=4)
+        if not a_tag:
+            return None
+
+        # The one with the highest similarity score
+        a_tag = sorted(a_tag, key=lambda tag: text_match(tag.string))[-1]
+
+        # Scraping from the LRC page
+        lrc_id = a_tag["href"].split(".")[-1]
+        soup = generate_bs4_soup(self.session, self.ROOT_URL + a_tag["href"])
+        return soup.find("div", {"id": f"lyrics_{lrc_id}_details"}).get_text()
```

### Comparing `syncedlyrics-0.4.0/syncedlyrics/providers/netease.py` & `syncedlyrics-0.5.0/syncedlyrics/providers/netease.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-"""NetEase (music.163.com) china-based provider"""
-
-from typing import Optional
-from rapidfuzz.fuzz import partial_ratio
-from .base import LRCProvider
-
-headers = {
-    "accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9",
-    "accept-language": "en-US,en;q=0.9,fa;q=0.8",
-    "cache-control": "max-age=0",
-    "sec-ch-ua": '".Not/A)Brand";v="99", "Google Chrome";v="103", "Chromium";v="103"',
-    "sec-ch-ua-mobile": "?0",
-    "sec-ch-ua-platform": '"Windows"',
-    "sec-fetch-dest": "document",
-    "sec-fetch-mode": "navigate",
-    "sec-fetch-site": "none",
-    "sec-fetch-user": "?1",
-    "upgrade-insecure-requests": "1",
-    "cookie": "NMTID=00OAVK3xqDG726ITU6jopU6jF2yMk0AAAGCO8l1BA; JSESSIONID-WYYY=8KQo11YK2GZP45RMlz8Kn80vHZ9%2FGvwzRKQXXy0iQoFKycWdBlQjbfT0MJrFa6hwRfmpfBYKeHliUPH287JC3hNW99WQjrh9b9RmKT%2Fg1Exc2VwHZcsqi7ITxQgfEiee50po28x5xTTZXKoP%2FRMctN2jpDeg57kdZrXz%2FD%2FWghb%5C4DuZ%3A1659124633932; _iuqxldmzr_=32; _ntes_nnid=0db6667097883aa9596ecfe7f188c3ec,1659122833973; _ntes_nuid=0db6667097883aa9596ecfe7f188c3ec; WNMCID=xygast.1659122837568.01.0; WEVNSM=1.0.0; WM_NI=CwbjWAFbcIzPX3dsLP%2F52VB%2Bxr572gmqAYwvN9KU5X5f1nRzBYl0SNf%2BV9FTmmYZy%2FoJLADaZS0Q8TrKfNSBNOt0HLB8rRJh9DsvMOT7%2BCGCQLbvlWAcJBJeXb1P8yZ3RHA%3D; WM_NIKE=9ca17ae2e6ffcda170e2e6ee90c65b85ae87b9aa5483ef8ab3d14a939e9a83c459959caeadce47e991fbaee82af0fea7c3b92a81a9ae8bd64b86beadaaf95c9cedac94cf5cedebfeb7c121bcaefbd8b16dafaf8fbaf67e8ee785b6b854f7baff8fd1728287a4d1d246a6f59adac560afb397bbfc25ad9684a2c76b9a8d00b2bb60b295aaafd24a8e91bcd1cb4882e8beb3c964fb9cbd97d04598e9e5a4c6499394ae97ef5d83bd86a3c96f9cbeffb1bb739aed9ea9c437e2a3; WM_TID=AAkRFnl03RdABEBEQFOBWHCPOeMra4IL; playerid=94262567",
-}
-
-
-class NetEase(LRCProvider):
-    """NetEase provider class"""
-
-    API_ENDPOINT_METADATA = "https://music.163.com/api/search/pc"
-    API_ENDPOINT_LYRICS = "https://music.163.com/api/song/lyric"
-
-    def __init__(self) -> None:
-        super().__init__()
-        self.session.headers.update(headers)
-
-    def search_track(self, search_term: str) -> Optional[dict]:
-        """Returns a `dict` containing some metadata for the found track."""
-        params = {"limit": 10, "type": 1, "offset": 0, "s": search_term}
-        response = self.session.get(self.API_ENDPOINT_METADATA, params=params)
-        results = response.json().get("result", {}).get("songs")
-        if not results:
-            return
-        track = results[0]
-        track_name = f"{track.get('name')} {track.get('artists')[0].get('name')}"
-        if partial_ratio(search_term, track_name) < 70:
-            return
-        # Update the session cookies from the new sent cookies for the next request.
-        self.session.cookies.update(response.cookies)
-        self.session.headers.update({"referer": response.url})
-        return track
-
-    def get_lrc_by_id(self, track_id: str) -> Optional[str]:
-        params = {"id": track_id, "lv": 1}
-        response = self.session.get(self.API_ENDPOINT_LYRICS, params=params)
-        lrc = response.json().get("lrc", {}).get("lyric")
-        if not lrc:
-            return
-        return lrc
-
-    def get_lrc(self, search_term: str) -> Optional[str]:
-        track = self.search_track(search_term)
-        if not track:
-            return
-        return self.get_lrc_by_id(track["id"])
+"""NetEase (music.163.com) china-based provider"""
+
+from typing import Optional
+from rapidfuzz.fuzz import partial_ratio
+from .base import LRCProvider
+
+headers = {
+    "accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9",
+    "accept-language": "en-US,en;q=0.9,fa;q=0.8",
+    "cache-control": "max-age=0",
+    "sec-ch-ua": '".Not/A)Brand";v="99", "Google Chrome";v="103", "Chromium";v="103"',
+    "sec-ch-ua-mobile": "?0",
+    "sec-ch-ua-platform": '"Windows"',
+    "sec-fetch-dest": "document",
+    "sec-fetch-mode": "navigate",
+    "sec-fetch-site": "none",
+    "sec-fetch-user": "?1",
+    "upgrade-insecure-requests": "1",
+    "cookie": "NMTID=00OAVK3xqDG726ITU6jopU6jF2yMk0AAAGCO8l1BA; JSESSIONID-WYYY=8KQo11YK2GZP45RMlz8Kn80vHZ9%2FGvwzRKQXXy0iQoFKycWdBlQjbfT0MJrFa6hwRfmpfBYKeHliUPH287JC3hNW99WQjrh9b9RmKT%2Fg1Exc2VwHZcsqi7ITxQgfEiee50po28x5xTTZXKoP%2FRMctN2jpDeg57kdZrXz%2FD%2FWghb%5C4DuZ%3A1659124633932; _iuqxldmzr_=32; _ntes_nnid=0db6667097883aa9596ecfe7f188c3ec,1659122833973; _ntes_nuid=0db6667097883aa9596ecfe7f188c3ec; WNMCID=xygast.1659122837568.01.0; WEVNSM=1.0.0; WM_NI=CwbjWAFbcIzPX3dsLP%2F52VB%2Bxr572gmqAYwvN9KU5X5f1nRzBYl0SNf%2BV9FTmmYZy%2FoJLADaZS0Q8TrKfNSBNOt0HLB8rRJh9DsvMOT7%2BCGCQLbvlWAcJBJeXb1P8yZ3RHA%3D; WM_NIKE=9ca17ae2e6ffcda170e2e6ee90c65b85ae87b9aa5483ef8ab3d14a939e9a83c459959caeadce47e991fbaee82af0fea7c3b92a81a9ae8bd64b86beadaaf95c9cedac94cf5cedebfeb7c121bcaefbd8b16dafaf8fbaf67e8ee785b6b854f7baff8fd1728287a4d1d246a6f59adac560afb397bbfc25ad9684a2c76b9a8d00b2bb60b295aaafd24a8e91bcd1cb4882e8beb3c964fb9cbd97d04598e9e5a4c6499394ae97ef5d83bd86a3c96f9cbeffb1bb739aed9ea9c437e2a3; WM_TID=AAkRFnl03RdABEBEQFOBWHCPOeMra4IL; playerid=94262567",
+}
+
+
+class NetEase(LRCProvider):
+    """NetEase provider class"""
+
+    API_ENDPOINT_METADATA = "https://music.163.com/api/search/pc"
+    API_ENDPOINT_LYRICS = "https://music.163.com/api/song/lyric"
+
+    def __init__(self) -> None:
+        super().__init__()
+        self.session.headers.update(headers)
+
+    def search_track(self, search_term: str) -> Optional[dict]:
+        """Returns a `dict` containing some metadata for the found track."""
+        params = {"limit": 10, "type": 1, "offset": 0, "s": search_term}
+        response = self.session.get(self.API_ENDPOINT_METADATA, params=params)
+        results = response.json().get("result", {}).get("songs")
+        if not results:
+            return
+        track = results[0]
+        track_name = f"{track.get('name')} {track.get('artists')[0].get('name')}"
+        if partial_ratio(search_term, track_name) < 70:
+            return
+        # Update the session cookies from the new sent cookies for the next request.
+        self.session.cookies.update(response.cookies)
+        self.session.headers.update({"referer": response.url})
+        return track
+
+    def get_lrc_by_id(self, track_id: str) -> Optional[str]:
+        params = {"id": track_id, "lv": 1}
+        response = self.session.get(self.API_ENDPOINT_LYRICS, params=params)
+        lrc = response.json().get("lrc", {}).get("lyric")
+        if not lrc:
+            return
+        return lrc
+
+    def get_lrc(self, search_term: str) -> Optional[str]:
+        track = self.search_track(search_term)
+        if not track:
+            return
+        return self.get_lrc_by_id(track["id"])
```

### Comparing `syncedlyrics-0.4.0/PKG-INFO` & `syncedlyrics-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncedlyrics
-Version: 0.4.0
+Version: 0.5.0
 Summary: Get an LRC format (synchronized) lyrics for your music
 Home-page: https://github.com/rtcq/syncedlyrics
 License: MIT
 Author: Momo
 Author-email: lo3me@proton.me
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -39,33 +39,31 @@
 syncedlyrics "SEARCH_TERM"
 ```
 #### Available Options
 | Flag | Description |
 | --- | --- |
 | `-o` | Path to save `.lrc` lyrics, default="{search_term}.lrc" |
 | `-v` | Use this flag to show the logs |
-| `--allow-plain` | Return a plain text (not synced) lyrics if not LRC was found |
+| `--allow-plain` | Return a plain text (not synced) lyrics if no LRC format was found |
 
 ### Python
 ```py
 import syncedlyrics
 lrc = syncedlyrics.search("[TRACK_NAME] [ARTIST_NAME]")
 ```
 Or with options:
 ```py
 syncedlyrics.search("...", allow_plain_format=True, save_path="{search_term}_1234.lrc", providers=["NetEase"])
 ```
 
 ## Providers
-- [NetEase](https://music.163.com/)
+- [Musixmatch](https://www.musixmatch.com/)
 - [Lyricsify](https://www.lyricsify.com/)
+- [NetEase](https://music.163.com/)
 - [Megalobiz](https://www.megalobiz.com/)
 - ~~[Deezer](https://deezer.com/)~~ (Currently broken, PR is appreciated)
 
 Feel free to suggest more providers please.
 
 ## License
 [MIT](https://github.com/rtcq/syncedlyrics/blob/master/LICENSE)
 
-## Notes
-I also found a [repo](https://github.com/fashni/MxLRC) for Musixmatch API, but it has annoying API rate limits at the moment
-
```

