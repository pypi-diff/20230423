# Comparing `tmp/elevenlabs-0.2.4.tar.gz` & `tmp/elevenlabs-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabs-0.2.4.tar", last modified: Wed Apr 19 16:18:16 2023, max compression
+gzip compressed data, was "elevenlabs-0.2.5.tar", last modified: Sun Apr 23 18:36:14 2023, max compression
```

## Comparing `elevenlabs-0.2.4.tar` & `elevenlabs-0.2.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:18:16.736959 elevenlabs-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-19 16:18:16.736959 elevenlabs-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-04-19 16:18:05.000000 elevenlabs-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:18:16.736959 elevenlabs-0.2.4/elevenlabs/
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-19 16:18:05.000000 elevenlabs-0.2.4/elevenlabs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:18:16.736959 elevenlabs-0.2.4/elevenlabs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-19 16:18:05.000000 elevenlabs-0.2.4/elevenlabs/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-19 16:18:05.000000 elevenlabs-0.2.4/elevenlabs/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-19 16:18:05.000000 elevenlabs-0.2.4/elevenlabs/api/history.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-19 16:18:05.000000 elevenlabs-0.2.4/elevenlabs/api/tts.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-19 16:18:05.000000 elevenlabs-0.2.4/elevenlabs/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-19 16:18:05.000000 elevenlabs-0.2.4/elevenlabs/api/voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-19 16:18:05.000000 elevenlabs-0.2.4/elevenlabs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:18:16.736959 elevenlabs-0.2.4/elevenlabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-19 16:18:16.000000 elevenlabs-0.2.4/elevenlabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-19 16:18:16.000000 elevenlabs-0.2.4/elevenlabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 16:18:16.000000 elevenlabs-0.2.4/elevenlabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-19 16:18:16.000000 elevenlabs-0.2.4/elevenlabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-19 16:18:16.000000 elevenlabs-0.2.4/elevenlabs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 16:18:16.736959 elevenlabs-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-19 16:18:05.000000 elevenlabs-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:36:14.323181 elevenlabs-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-23 18:36:14.323181 elevenlabs-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-04-23 18:35:56.000000 elevenlabs-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:36:14.323181 elevenlabs-0.2.5/elevenlabs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-23 18:35:56.000000 elevenlabs-0.2.5/elevenlabs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:36:14.323181 elevenlabs-0.2.5/elevenlabs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-23 18:35:56.000000 elevenlabs-0.2.5/elevenlabs/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-23 18:35:56.000000 elevenlabs-0.2.5/elevenlabs/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-23 18:35:56.000000 elevenlabs-0.2.5/elevenlabs/api/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-23 18:35:56.000000 elevenlabs-0.2.5/elevenlabs/api/tts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-23 18:35:56.000000 elevenlabs-0.2.5/elevenlabs/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-23 18:35:56.000000 elevenlabs-0.2.5/elevenlabs/api/voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-23 18:35:56.000000 elevenlabs-0.2.5/elevenlabs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:36:14.323181 elevenlabs-0.2.5/elevenlabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-23 18:36:14.000000 elevenlabs-0.2.5/elevenlabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-23 18:36:14.000000 elevenlabs-0.2.5/elevenlabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:36:14.000000 elevenlabs-0.2.5/elevenlabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-23 18:36:14.000000 elevenlabs-0.2.5/elevenlabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 18:36:14.000000 elevenlabs-0.2.5/elevenlabs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 18:36:14.323181 elevenlabs-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-23 18:35:56.000000 elevenlabs-0.2.5/setup.py
```

### Comparing `elevenlabs-0.2.4/PKG-INFO` & `elevenlabs-0.2.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabs
-Version: 0.2.4
+Version: 0.2.5
 Summary: The official elevenlabs python package.
 Home-page: https://github.com/elevenlabs/elevenlabs-python
 Author: Elevenlabs
 Keywords: artificial intelligence,deep learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `elevenlabs-0.2.4/README.md` & `elevenlabs-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.4/elevenlabs/__init__.py` & `elevenlabs-0.2.5/elevenlabs/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import re
 import wave
 from collections.abc import Iterator
 from typing import List, Optional, Union
 
 from .api import TTS, Voice, VoiceClone, Voices, VoiceSettings
 from .utils import *  # noqa F403
 
@@ -12,15 +13,15 @@
 
 
 def get_api_key() -> Optional[str]:
     return os.environ.get("ELEVEN_API_KEY")
 
 
 # Save default voices to avoid querying the API for unathorized users
-DEFAULT_VOICES = [
+VOICES_CACHE = [
     Voice(
         voice_id="21m00Tcm4TlvDq8ikWAM",
         name="Rachel",
         category="premade",
         settings=VoiceSettings(stability=0.75, similarity_boost=0.75),
     ),
     Voice(
@@ -75,35 +76,49 @@
 
 
 def voices(api_key: Optional[str] = None) -> List[Voice]:
     """Lists all voices in the API, if authenticated for the current user"""
     if api_key:
         set_api_key(api_key)
     api_key = get_api_key()
-    return Voices.from_api() if api_key else DEFAULT_VOICES
+    global VOICES_CACHE
+    VOICES_CACHE = Voices.from_api() if api_key else VOICES_CACHE
+    return VOICES_CACHE
 
 
 def clone(**kwargs) -> Voice:
     return Voice.from_clone(VoiceClone(**kwargs))
 
 
+def is_voice_id(val: str) -> bool:
+    return bool(re.match(r"^[a-zA-Z0-9]{20}$", val))
+
+
 def generate(
     text: str,
     api_key: Optional[str] = None,
-    voice: Union[str, Voice] = DEFAULT_VOICES[2],  # Bella
+    voice: Union[str, Voice] = VOICES_CACHE[2],  # Bella
     stream: bool = False,
     stream_chunk_size: int = 2048,
 ) -> Union[bytes, Iterator[bytes]]:
     if api_key:
         set_api_key(api_key)
 
-    # Find first voice with matching name or id if string provided
     if isinstance(voice, str):
         voice_str = voice
-        voice = next((v for v in voices() if v.name == voice or v.voice_id == voice), None)  # type: ignore # noqa E501
+        # If voice is valid voice_id, use it
+        if is_voice_id(voice):
+            voice = Voice(voice_id=voice)
+        # Otherwise, search voice by name
+        else:
+            # Check if voice is in cache
+            voice = next((v for v in VOICES_CACHE if v.name == voice), None)  # type: ignore # noqa E501
+            # If not, query API
+            voice = next((v for v in voices() if v.name == voice), None) if not voice else voice  # type: ignore # noqa E501
+        # Raise error if voice not found
         if not voice:
             raise ValueError(f"Voice '{voice_str}' not found.")
 
     assert isinstance(voice, Voice)
 
     if stream:
         return TTS.generate_stream(text, voice, stream_chunk_size)
```

### Comparing `elevenlabs-0.2.4/elevenlabs/api/base.py` & `elevenlabs-0.2.5/elevenlabs/api/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,23 +21,24 @@
         if method == "get":
             response = requests.get(url, headers=headers, **kwargs)
         elif method == "post":
             response = requests.post(url, headers=headers, **kwargs)
         else:
             raise ValueError(f"Invalid request method {method}")
 
-        # print(response.status_code, response.reason, response.text)
-
         if response.status_code == 401:
             raise SystemExit(
                 "Your quota is exceeded or your API key is invalid, please set a"
                 " valid key: ELEVEN_API_KEY"
             )
 
-        response.raise_for_status()
+        try:
+            response.raise_for_status()
+        except Exception as e:
+            raise type(e)(response.reason, response.text)
         return response
 
     @staticmethod
     def get(url: str, *args, **kwargs):
         return API.request(url, method="get", *args, **kwargs)  # type: ignore
 
     @staticmethod
```

### Comparing `elevenlabs-0.2.4/elevenlabs/api/history.py` & `elevenlabs-0.2.5/elevenlabs/api/history.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.4/elevenlabs/api/tts.py` & `elevenlabs-0.2.5/elevenlabs/api/tts.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,21 +6,25 @@
 from .voice import Voice
 
 
 class TTS(API):
     @staticmethod
     def generate(text: str, voice: Voice) -> bytes:
         url = f"{api_base_url_v1}/text-to-speech/{voice.voice_id}"
-        data = dict(text=text, voice_settings=voice.settings.dict())  # type: ignore
+        data = dict(
+            text=text, voice_settings=voice.settings.dict() if voice.settings else None
+        )  # type: ignore
         response = API.post(url, json=data)
         return response.content
 
     @staticmethod
     def generate_stream(
         text: str, voice: Voice, stream_chunk_size: int = 2048
     ) -> Iterator[bytes]:
         url = f"{api_base_url_v1}/text-to-speech/{voice.voice_id}/stream"
-        data = dict(text=text, voice_settings=voice.settings.dict())  # type: ignore
+        data = dict(
+            text=text, voice_settings=voice.settings.dict() if voice.settings else None
+        )  # type: ignore
         response = API.post(url, json=data, stream=True)
         for chunk in response.iter_content(chunk_size=stream_chunk_size):
             if chunk:
                 yield chunk
```

### Comparing `elevenlabs-0.2.4/elevenlabs/api/voice.py` & `elevenlabs-0.2.5/elevenlabs/api/voice.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.4/elevenlabs/utils.py` & `elevenlabs-0.2.5/elevenlabs/utils.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.4/elevenlabs.egg-info/PKG-INFO` & `elevenlabs-0.2.5/elevenlabs.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabs
-Version: 0.2.4
+Version: 0.2.5
 Summary: The official elevenlabs python package.
 Home-page: https://github.com/elevenlabs/elevenlabs-python
 Author: Elevenlabs
 Keywords: artificial intelligence,deep learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `elevenlabs-0.2.4/setup.py` & `elevenlabs-0.2.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import find_packages, setup
 
 setup(
     name="elevenlabs",
     packages=find_packages(exclude=[]),
-    version="0.2.4",
+    version="0.2.5",
     description="The official elevenlabs python package.",
     long_description_content_type="text/markdown",
     author="Elevenlabs",
     url="https://github.com/elevenlabs/elevenlabs-python",
     keywords=["artificial intelligence", "deep learning"],
-    install_requires=["pydantic>=1.10", "ipython>=8.0"],
+    install_requires=["pydantic>=1.10", "ipython>=7.0"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.6",
     ],
```

