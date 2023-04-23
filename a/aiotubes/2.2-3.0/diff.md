# Comparing `tmp/aiotubes-2.2.tar.gz` & `tmp/aiotubes-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotubes-2.2.tar", last modified: Thu Mar 16 19:11:14 2023, max compression
+gzip compressed data, was "aiotubes-3.0.tar", last modified: Sun Apr 23 14:58:05 2023, max compression
```

## Comparing `aiotubes-2.2.tar` & `aiotubes-3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-03-16 19:11:14.874007 aiotubes-2.2/
--rw-rw-rw-   0        0        0     1084 2022-10-11 08:30:57.000000 aiotubes-2.2/LICENSE
--rw-rw-rw-   0        0        0      697 2023-03-16 19:11:14.873008 aiotubes-2.2/PKG-INFO
--rw-rw-rw-   0        0        0      362 2023-02-26 12:48:23.000000 aiotubes-2.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-16 19:11:14.845082 aiotubes-2.2/aiotubes/
--rw-rw-rw-   0        0        0       56 2023-03-16 19:10:05.000000 aiotubes-2.2/aiotubes/__init__.py
--rw-rw-rw-   0        0        0      994 2023-02-24 10:13:03.000000 aiotubes-2.2/aiotubes/constants.py
--rw-rw-rw-   0        0        0     3220 2023-03-16 19:10:05.000000 aiotubes-2.2/aiotubes/exceptions.py
--rw-rw-rw-   0        0        0     6213 2023-03-16 19:10:05.000000 aiotubes-2.2/aiotubes/extractors.py
--rw-rw-rw-   0        0        0     1487 2023-02-24 20:59:01.000000 aiotubes-2.2/aiotubes/helpers.py
--rw-rw-rw-   0        0        0     4427 2023-02-24 13:57:51.000000 aiotubes-2.2/aiotubes/itags.py
--rw-rw-rw-   0        0        0     2142 2023-03-16 19:10:05.000000 aiotubes-2.2/aiotubes/playlist.py
--rw-rw-rw-   0        0        0     1155 2023-03-16 19:10:05.000000 aiotubes-2.2/aiotubes/request.py
--rw-rw-rw-   0        0        0     8022 2023-03-16 19:10:05.000000 aiotubes-2.2/aiotubes/streams.py
--rw-rw-rw-   0        0        0     5199 2023-03-16 19:10:25.000000 aiotubes-2.2/aiotubes/video.py
-drwxrwxrwx   0        0        0        0 2023-03-16 19:11:14.872010 aiotubes-2.2/aiotubes.egg-info/
--rw-rw-rw-   0        0        0      697 2023-03-16 19:11:14.000000 aiotubes-2.2/aiotubes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-03-16 19:11:14.000000 aiotubes-2.2/aiotubes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-16 19:11:14.000000 aiotubes-2.2/aiotubes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-03-16 19:11:14.000000 aiotubes-2.2/aiotubes.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-16 19:11:14.000000 aiotubes-2.2/aiotubes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-16 19:11:14.874007 aiotubes-2.2/setup.cfg
--rw-rw-rw-   0        0        0      659 2023-03-16 19:11:08.000000 aiotubes-2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 14:58:05.477006 aiotubes-3.0/
+-rw-rw-rw-   0        0        0     1084 2022-10-11 08:30:57.000000 aiotubes-3.0/LICENSE
+-rw-rw-rw-   0        0        0      697 2023-04-23 14:58:05.476009 aiotubes-3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2023-04-23 14:57:43.000000 aiotubes-3.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-23 14:58:05.450077 aiotubes-3.0/aiotube/
+-rw-rw-rw-   0        0        0       58 2023-04-23 14:53:51.000000 aiotubes-3.0/aiotube/__init__.py
+-rw-rw-rw-   0        0        0     1762 2023-04-23 14:53:51.000000 aiotubes-3.0/aiotube/client.py
+-rw-rw-rw-   0        0        0      994 2023-04-23 12:02:05.000000 aiotubes-3.0/aiotube/constants.py
+-rw-rw-rw-   0        0        0     2511 2023-04-23 14:53:45.000000 aiotubes-3.0/aiotube/exceptions.py
+-rw-rw-rw-   0        0        0     5405 2023-04-23 14:53:51.000000 aiotubes-3.0/aiotube/extractors.py
+-rw-rw-rw-   0        0        0     1487 2023-02-24 20:59:01.000000 aiotubes-3.0/aiotube/helpers.py
+-rw-rw-rw-   0        0        0     4427 2023-02-24 13:57:51.000000 aiotubes-3.0/aiotube/itags.py
+-rw-rw-rw-   0        0        0     2226 2023-04-23 14:53:51.000000 aiotubes-3.0/aiotube/playlist.py
+-rw-rw-rw-   0        0        0     8021 2023-04-23 14:53:51.000000 aiotubes-3.0/aiotube/streams.py
+-rw-rw-rw-   0        0        0     5029 2023-04-23 14:53:51.000000 aiotubes-3.0/aiotube/video.py
+drwxrwxrwx   0        0        0        0 2023-04-23 14:58:05.475035 aiotubes-3.0/aiotubes.egg-info/
+-rw-rw-rw-   0        0        0      697 2023-04-23 14:58:05.000000 aiotubes-3.0/aiotubes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-04-23 14:58:05.000000 aiotubes-3.0/aiotubes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 14:58:05.000000 aiotubes-3.0/aiotubes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-23 14:58:05.000000 aiotubes-3.0/aiotubes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-23 14:58:05.000000 aiotubes-3.0/aiotubes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 14:58:05.477006 aiotubes-3.0/setup.cfg
+-rw-rw-rw-   0        0        0      666 2023-04-23 14:51:17.000000 aiotubes-3.0/setup.py
```

### Comparing `aiotubes-2.2/LICENSE` & `aiotubes-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotubes-2.2/PKG-INFO` & `aiotubes-3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aiotubes
-Version: 2.2
+Version: 3.0
 Summary: Asynchronous Youtube API
 Home-page: https://github.com/sheldygg/aiotube
 Author: sheldy
 License: MIT
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AIOTUBE
 
-**aiotube** Asynchronous Youtube API
+**aiotube** Asynchronous YouTube API
 
 
 ### Example
 
 ```python
 import asyncio
 
-from aiotubes import Video
+from aiotube import Video
 
 async def main():
     client = Video("https://www.youtube.com/watch?v=MZ-cvXEvYI8")
     stream = (await client.streams()).get_audio_only()
     await stream.download_filepath(filename="yeat.mp3")
     
 asyncio.run(main())
```

### Comparing `aiotubes-2.2/aiotubes/constants.py` & `aiotubes-3.0/aiotube/constants.py`

 * *Files identical despite different names*

### Comparing `aiotubes-2.2/aiotubes/exceptions.py` & `aiotubes-3.0/aiotube/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from typing import Pattern, Union
+from re import Pattern
 
 
-class AiotubeError(Exception):
-    "Base Exception"
+class AiotubeError(BaseException):
+    """Base Exception"""
 
 
 class HTMLParseError(AiotubeError):
     pass
 
 
 class RegexMatchError(AiotubeError):
     """Regex pattern did not return any matches."""
 
-    def __init__(self, caller: str, pattern: Union[str, Pattern]):
+    def __init__(self, caller: str, pattern: str | Pattern):
         """
         :param str caller:
             Calling function
         :param str pattern:
             Pattern that failed to match
         """
         super().__init__(f"{caller}: could not find match for {pattern}")
@@ -37,21 +37,14 @@
 
     @property
     def error_string(self):
         return f"{self.video_id} is unavailable"
 
 
 class MembersOnly(VideoUnavailable):
-    """Video is members-only.
-
-    YouTube has special videos that are only viewable to users who have
-    subscribed to a content creator.
-    ref: https://support.google.com/youtube/answer/7544492?hl=en
-    """
-
     def __init__(self, video_id: str):
         """
         :param str video_id:
             A YouTube video identifier.
         """
         self.video_id = video_id
         super().__init__(self.video_id)
@@ -99,23 +92,7 @@
         """
         self.video_id = video_id
         super().__init__(self.video_id)
 
     @property
     def error_string(self):
         return f"{self.video_id} is a private video"
-
-
-class AgeRestrictedError(VideoUnavailable):
-    """Video is age restricted, and cannot be accessed without OAuth."""
-
-    def __init__(self, video_id: str):
-        """
-        :param str video_id:
-            A YouTube video identifier.
-        """
-        self.video_id = video_id
-        super().__init__(self.video_id)
-
-    @property
-    def error_string(self):
-        return f"{self.video_id} is age restricted, and can't be accessed without logging in."
```

### Comparing `aiotubes-2.2/aiotubes/extractors.py` & `aiotubes-3.0/aiotube/extractors.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,117 +1,27 @@
 import ast
 import json
 import re
-from typing import Dict, List, Tuple, Union
 from urllib.parse import parse_qs, urlparse
 
-from .exceptions import HTMLParseError, RegexMatchError
+from aiotube.exceptions import HTMLParseError, RegexMatchError
 
 
-def playability_status(watch_html: str):
-    """Return the playability status and status explanation of a video.
-
-    For example, a video may have a status of LOGIN_REQUIRED, and an explanation
-    of "This is a private video. Please sign in to verify that you may see it."
-
-    This explanation is what gets incorporated into the media player overlay.
-
-    :param str watch_html:
-        The html contents of the watch page.
-    :rtype: bool
-    :returns:
-        Playability status and reason of the video.
-    """
-    player_response = initial_player_response(watch_html)
-    status_dict = player_response.get("playabilityStatus", {})
-    if "liveStreamability" in status_dict:
-        return "LIVE_STREAM", "Video is a live stream."
-    if "status" in status_dict:
-        if "reason" in status_dict:
-            return status_dict["status"], [status_dict["reason"]]
-        if "messages" in status_dict:
-            return status_dict["status"], status_dict["messages"]
-    return None, [None]
-
-
-def initial_player_response(watch_html: str) -> str:
-    """Extract the ytInitialPlayerResponse json from the watch_html page.
-
-    This mostly contains metadata necessary for rendering the page on-load,
-    such as video information, copyright notices, etc.
-
-    @param watch_html: Html of the watch page
-    @return:
-    """
-    patterns = [
-        r"window\[['\"]ytInitialPlayerResponse['\"]]\s*=\s*",
-        r"ytInitialPlayerResponse\s*=\s*",
-    ]
-    for pattern in patterns:
-        try:
-            return parse_for_object(watch_html, pattern)
-        except HTMLParseError:
-            pass
-
-    raise RegexMatchError(
-        caller="initial_player_response", pattern="initial_player_response_pattern"
-    )
-
-
-def extract_video_id(url: str) -> str:
+def extract_video_id(url: str):
     pattern = r"(?:v=|\/)([0-9A-Za-z_-]{11}).*"
     result = re.search(pattern=pattern, string=url)
     return result.group(1)
 
 
-def extract_playlist_id(url: str) -> str:
-    parsed = urlparse(url)
-    return parse_qs(parsed.query)["list"][0]
-
-
-def extract_playlist_info(watch_html: str) -> str:
-    patterns = [r"window\[['\"]ytInitialData['\"]]\s*=\s*", r"ytInitialData\s*=\s*"]
-    for pattern in patterns:
-        try:
-            return parse_for_object(watch_html, pattern)
-        except HTMLParseError:
-            pass
-
-    raise RegexMatchError(
-        caller="extract_playlist_info", pattern="extract_playlist_info_pattern"
-    )
-
-
-def parse_for_object(html, preceding_regex):
-    regex = re.compile(preceding_regex)
-    result = regex.search(html)
-    if not result:
-        raise HTMLParseError(f"No matches for regex {preceding_regex}")
-
-    start_index = result.end()
-    return parse_for_object_from_startpoint(html, start_index)
-
-
-def parse_for_object_from_startpoint(html, start_point):
-    full_obj = find_object_from_startpoint(html, start_point)
-    try:
-        return json.loads(full_obj)
-    except json.decoder.JSONDecodeError:
-        try:
-            return ast.literal_eval(full_obj)
-        except (ValueError, SyntaxError):
-            raise HTMLParseError("Could not parse object.")
-
-
 def find_object_from_startpoint(html, start_point):
     html = html[start_point:]
     if html[0] not in ["{", "["]:
         raise HTMLParseError(f"Invalid start point. Start of HTML:\n{html[:20]}")
 
-    # First letter MUST be a open brace, so we put that in the stack,
+    # First letter MUST be an open brace, so we put that in the stack,
     # and skip the first character.
     stack = [html[0]]
     i = 1
 
     context_closers = {"{": "}", "[": "]", '"': '"'}
 
     while i < len(html):
@@ -140,15 +50,73 @@
 
         i += 1
 
     full_obj = html[:i]
     return full_obj  # noqa: R504
 
 
-def apply_descrambler(stream_data: Dict) -> Union[List, None]:
+def parse_for_object_from_startpoint(html, start_point):
+    full_obj = find_object_from_startpoint(html, start_point)
+    try:
+        return json.loads(full_obj)
+    except json.decoder.JSONDecodeError:
+        try:
+            return ast.literal_eval(full_obj)
+        except (ValueError, SyntaxError):
+            raise HTMLParseError("Could not parse object.")
+
+
+def parse_for_object(html, preceding_regex):
+    regex = re.compile(preceding_regex)
+    result = regex.search(html)
+    if not result:
+        raise HTMLParseError(f"No matches for regex {preceding_regex}")
+
+    start_index = result.end()
+    return parse_for_object_from_startpoint(html, start_index)
+
+
+def initial_player_response(watch_html: str) -> str | dict:
+    patterns = [
+        r"window\[['\"]ytInitialPlayerResponse['\"]]\s*=\s*",
+        r"ytInitialPlayerResponse\s*=\s*",
+    ]
+    for pattern in patterns:
+        try:
+            return parse_for_object(watch_html, pattern)
+        except HTMLParseError:
+            pass
+
+    raise RegexMatchError(
+        caller="initial_player_response", pattern="initial_player_response_pattern"
+    )
+
+
+def playability_status(watch_html: str):
+    player_response = initial_player_response(watch_html)
+    status_dict = player_response.get("playabilityStatus", {})
+    if "liveStreamability" in status_dict:
+        return "LIVE_STREAM", "Video is a live stream."
+    if "status" in status_dict:
+        if "reason" in status_dict:
+            return status_dict["status"], [status_dict["reason"]]
+        if "messages" in status_dict:
+            return status_dict["status"], status_dict["messages"]
+    return None, [None]
+
+
+def mime_type_codec(mime_type_codec: str) -> tuple[str, list[str]]:
+    pattern = r"(\w+\/\w+)\;\scodecs=\"([a-zA-Z-0-9.,\s]*)\""
+    regex = re.compile(pattern)
+    results = regex.search(mime_type_codec)
+    mime_type, codecs = results.groups()
+    return mime_type, [c.strip() for c in codecs.split(",")]
+
+
+def apply_descrambler(stream_data: dict) -> list | None:
     if "url" in stream_data:
         return None
     formats = []
     if "formats" in stream_data.keys():
         formats.extend(stream_data["formats"])
     if "adaptiveFormats" in stream_data.keys():
         formats.extend(stream_data["adaptiveFormats"])
@@ -159,25 +127,35 @@
                 data["url"] = cipher_url["url"][0]
                 data["s"] = cipher_url["s"][0]
         data["is_otf"] = data.get("type") == "FORMAT_STREAM_TYPE_OTF"
 
     return formats
 
 
+def extract_playlist_id(url: str) -> str:
+    parsed = urlparse(url)
+    return parse_qs(parsed.query)["list"][0]
+
+
+def extract_playlist_info(watch_html: str) -> str | dict:
+    patterns = [r"window\[['\"]ytInitialData['\"]]\s*=\s*", r"ytInitialData\s*=\s*"]
+    for pattern in patterns:
+        try:
+            return parse_for_object(watch_html, pattern)
+        except HTMLParseError:
+            pass
+
+    raise RegexMatchError(
+        caller="extract_playlist_info", pattern="extract_playlist_info_pattern"
+    )
+
+
 def extract_video_id_from_playlist(playlist_info: dict):
     section_contents = playlist_info["contents"]["twoColumnBrowseResultsRenderer"][
         "tabs"
     ][0]["tabRenderer"]["content"]["sectionListRenderer"]["contents"]
     important_content = section_contents[0]["itemSectionRenderer"]["contents"][0][
         "playlistVideoListRenderer"
     ]
     videos = important_content["contents"]
     video_ids = list(map(lambda x: x["playlistVideoRenderer"]["videoId"], videos))
     return video_ids
-
-
-def mime_type_codec(mime_type_codec: str) -> Tuple[str, List[str]]:
-    pattern = r"(\w+\/\w+)\;\scodecs=\"([a-zA-Z-0-9.,\s]*)\""
-    regex = re.compile(pattern)
-    results = regex.search(mime_type_codec)
-    mime_type, codecs = results.groups()
-    return mime_type, [c.strip() for c in codecs.split(",")]
```

### Comparing `aiotubes-2.2/aiotubes/helpers.py` & `aiotubes-3.0/aiotube/helpers.py`

 * *Files identical despite different names*

### Comparing `aiotubes-2.2/aiotubes/itags.py` & `aiotubes-3.0/aiotube/itags.py`

 * *Files identical despite different names*

### Comparing `aiotubes-2.2/aiotubes/playlist.py` & `aiotubes-3.0/aiotube/playlist.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from typing import AsyncGenerator, List
 
+from .client import HttpMethod, RequestClient
 from .extractors import (extract_playlist_id, extract_playlist_info,
                          extract_video_id_from_playlist)
-from .request import RequestClient
 from .video import Video
 
 
-class Playlist(RequestClient):
+class Playlist:
     def __init__(self, url: str) -> None:
+        self.client = RequestClient("ANDROID")
         self._input_url = url
         self._playlist_id = None
         self._html = None
         self._playlist_info = None
         self._sidebar_info = None
 
     @property
@@ -24,15 +25,17 @@
     @property
     def playlist_url(self) -> str:
         return f"https://www.youtube.com/playlist?list={self.playlist_id}"
 
     async def playlist_html(self) -> str:
         if self._html:
             return self._html
-        request = await self.request(method="GET", url=self.playlist_url)
+        request = await self.client.request(
+            method=HttpMethod.GET, url=self.playlist_url
+        )
         self._html = request.get("response").decode("utf-8")
         return self._html
 
     async def playlist_info(self) -> dict:
         if self._playlist_info:
             return self._playlist_info
         info = extract_playlist_info(await self.playlist_html())
```

### Comparing `aiotubes-2.2/aiotubes/streams.py` & `aiotubes-3.0/aiotube/streams.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 from datetime import datetime
 from io import BytesIO
 from typing import AsyncGenerator, Callable, List, Optional
 
 from pydantic import BaseModel, HttpUrl
 
+from .client import RequestClient
 from .extractors import mime_type_codec
 from .helpers import safe_filename, target_directory
 from .itags import get_format_profile
-from .request import RequestClient
 
 
 class Stream(BaseModel, RequestClient):
     title: str
     author: str
     url: HttpUrl
     itag: int
```

### Comparing `aiotubes-2.2/aiotubes/video.py` & `aiotubes-3.0/aiotube/video.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,108 +1,107 @@
-from typing import Dict, List, Optional
+from aiotube.client import HttpMethod, RequestClient
+from aiotube.exceptions import (LiveStreamError, MembersOnly,
+                                RecordingUnavailable, VideoPrivate,
+                                VideoUnavailable)
+from aiotube.extractors import (apply_descrambler, extract_video_id,
+                                playability_status)
+from aiotube.streams import Stream, StreamQuery
 
-from .constants import default_clients
-from .exceptions import (AgeRestrictedError, LiveStreamError, MembersOnly,
-                         RecordingUnavailable, VideoPrivate, VideoUnavailable)
-from .extractors import apply_descrambler, extract_video_id, playability_status
-from .request import RequestClient
-from .streams import Stream, StreamQuery
 
-
-class Video(RequestClient):
-    def __init__(self, url: str, client: str = "ANDROID") -> None:
+class Video:
+    def __init__(self, url: str):
         self.video_id = extract_video_id(url)
-        self.api_key = default_clients[client]["api_key"]
-        self.context = default_clients[client]["context"]
         self.base_url = "https://www.youtube.com/youtubei/v1"
         self.watch_url = f"https://youtube.com/watch?v={self.video_id}"
-        self._video_info: Optional[Dict] = None
-        self._fmt_streams: Optional[List[Stream]] = None
+        self.client = RequestClient("ANDROID")
         self._html = None
+        self._video_info = None
+        self._fmt_streams = None
 
-    @property
-    def base_params(self) -> Dict:
-        return {"key": self.api_key, "contentCheckOk": True, "racyCheckOk": True}
-
-    @property
-    def base_data(self) -> Dict:
-        return {"context": self.context}
+    def __repr__(self):
+        return f"<aiotube.video.Video object: videoId={self.video_id}>"
 
     async def html(self):
-        if self._html:
-            return self._html
-        return (await self.request(method="GET", url=self.watch_url)).get("response")
-
-    async def video_info(self) -> Dict:
-        if self._video_info:
-            return self._video_info
-        endpoint = f"{self.base_url}/player"
-        query = {
-            "videoId": self.video_id,
-        }
-        query.update(self.base_params)
-        headers = {"Content-Type": "application/json"}
-        result = await self.request(
-            method="POST",
-            url=endpoint,
-            params=query,
-            headers=headers,
-            data=self.base_data,
-        )
-        self._video_info = result.get("response")
+        if self._html is None:
+            self._html = (
+                await self.client.request(method=HttpMethod.GET, url=self.watch_url)
+            ).get("response")
+        return self._html
+
+    async def video_info(self):
+        if self._video_info is None:
+            endpoint = f"{self.base_url}/player"
+            query = {"videoId": self.video_id}
+            query.update(self.client.base_params)
+            headers = {"Content-Type": "application/json"}
+            response = await self.client.request(
+                method=HttpMethod.POST,
+                url=endpoint,
+                params=query,
+                headers=headers,
+                data=self.client.base_data,
+            )
+            self._video_info = response.get("response")
         return self._video_info
 
-    async def streaming_data(self) -> Dict:
+    async def streaming_data(self):
         await self.check_availability()
         data = await self.video_info()
         if "streamingData" in data:
             return data["streamingData"]
-        else:
-            return await self.bypass_age_gate()
+        await self.bypass_age_gate()
+        return self._video_info
 
-    async def fmt_streams(self) -> List[Stream]:
+    async def fmt_streams(self):
         await self.check_availability()
         if self._fmt_streams:
             return self._fmt_streams
         self._fmt_streams = []
         stream_manifest = apply_descrambler(await self.streaming_data())
         video_title = await self.title()
         video_author = await self.author()
         for stream in stream_manifest:
             video = Stream(title=video_title, author=video_author, **stream)
             self._fmt_streams.append(video)
         return self._fmt_streams
 
-    async def streams(self) -> StreamQuery:
+    async def streams(self):
         return StreamQuery(await self.fmt_streams())
 
-    async def length(self) -> int:
-        """Get the video length in seconds."""
-        return int(
-            (await self.video_info()).get("videoDetails", {}).get("lengthSeconds")
+    async def bypass_age_gate(self):
+        client = RequestClient("ANDROID_EMBED")
+        endpoint = f"{self.base_url}/player"
+        query = {"videoId": self.video_id}
+        query.update(self.client.base_params)
+        headers = {"Content-Type": "application/json"}
+        response = await client.request(
+            method=HttpMethod.POST,
+            url=endpoint,
+            params=query,
+            headers=headers,
+            data=self.client.base_data,
         )
+        self._video_info = response.get("response")
 
-    async def title(self) -> int:
+    async def title(self) -> str:
         """Get the video title."""
         await self.check_availability()
         return (await self.video_info()).get("videoDetails", {}).get("title")
 
-    async def author(self) -> int:
+    async def author(self) -> str:
         """Get the video author."""
         return (
             (await self.video_info()).get("videoDetails", {}).get("author", "unknown")
         )
 
-    async def bypass_age_gate(self):
-        self.api_key = default_clients["ANDROID_EMBED"]["api_key"]
-        self.context = default_clients["ANDROID_EMBED"]["context"]
-        data = await self.video_info()
-        playability_status = data["playabilityStatus"].get("status", None)
-        if playability_status == "UNPLAYABLE":
-            raise AgeRestrictedError(self.video_id)
+    async def length(self) -> int:
+        """Get the video length in seconds."""
+        return int(
+            (await self.video_info()).get("videoDetails", {}).get("lengthSeconds")
+        )
 
     async def check_availability(self):
         html = (await self.html()).decode()
         status, messages = playability_status(html)
         for reason in messages:
             if status == "UNPLAYABLE":
                 if reason == (
@@ -121,10 +120,7 @@
                 ):
                     raise VideoPrivate(video_id=self.video_id)
             elif status == "ERROR":
                 if reason == "Video unavailable":
                     raise VideoUnavailable(video_id=self.video_id)
             elif status == "LIVE_STREAM":
                 raise LiveStreamError(video_id=self.video_id)
-
-    def __repr__(self):
-        return f"<aiotubes.video.Video object: videoId={self.video_id}>"
```

### Comparing `aiotubes-2.2/aiotubes.egg-info/PKG-INFO` & `aiotubes-3.0/aiotubes.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aiotubes
-Version: 2.2
+Version: 3.0
 Summary: Asynchronous Youtube API
 Home-page: https://github.com/sheldygg/aiotube
 Author: sheldy
 License: MIT
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AIOTUBE
 
-**aiotube** Asynchronous Youtube API
+**aiotube** Asynchronous YouTube API
 
 
 ### Example
 
 ```python
 import asyncio
 
-from aiotubes import Video
+from aiotube import Video
 
 async def main():
     client = Video("https://www.youtube.com/watch?v=MZ-cvXEvYI8")
     stream = (await client.streams()).get_audio_only()
     await stream.download_filepath(filename="yeat.mp3")
     
 asyncio.run(main())
```

