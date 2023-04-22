# Comparing `tmp/audio_extract-0.2.0.tar.gz` & `tmp/audio_extract-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio_extract-0.2.0.tar", last modified: Sat Apr 22 21:57:41 2023, max compression
+gzip compressed data, was "audio_extract-0.3.0.tar", last modified: Sat Apr 22 22:01:30 2023, max compression
```

## Comparing `audio_extract-0.2.0.tar` & `audio_extract-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 21:57:41.771234 audio_extract-0.2.0/
--rw-rw-rw-   0        0        0     1090 2023-04-22 17:27:29.000000 audio_extract-0.2.0/LICENSE.md
--rw-rw-rw-   0        0        0     4314 2023-04-22 21:57:41.770233 audio_extract-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3393 2023-04-22 21:57:09.000000 audio_extract-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 21:57:41.745235 audio_extract-0.2.0/audio_extract/
--rw-rw-rw-   0        0        0     1705 2023-04-22 21:37:32.000000 audio_extract-0.2.0/audio_extract/__init__.py
--rw-rw-rw-   0        0        0      142 2023-04-22 18:09:12.000000 audio_extract-0.2.0/audio_extract/exceptions.py
--rw-rw-rw-   0        0        0     1123 2023-04-22 21:31:51.000000 audio_extract-0.2.0/audio_extract/execute.py
--rw-rw-rw-   0        0        0     1798 2023-04-22 21:45:01.000000 audio_extract-0.2.0/audio_extract/ffmpeg_tools.py
--rw-rw-rw-   0        0        0     1245 2023-04-22 21:50:51.000000 audio_extract-0.2.0/audio_extract/utils.py
--rw-rw-rw-   0        0        0     2859 2023-04-22 19:49:07.000000 audio_extract-0.2.0/audio_extract/validators.py
-drwxrwxrwx   0        0        0        0 2023-04-22 21:57:41.768233 audio_extract-0.2.0/audio_extract.egg-info/
--rw-rw-rw-   0        0        0     4314 2023-04-22 21:57:41.000000 audio_extract-0.2.0/audio_extract.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2023-04-22 21:57:41.000000 audio_extract-0.2.0/audio_extract.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 21:57:41.000000 audio_extract-0.2.0/audio_extract.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-22 21:57:41.000000 audio_extract-0.2.0/audio_extract.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       70 2023-04-22 21:57:41.000000 audio_extract-0.2.0/audio_extract.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-22 21:57:41.000000 audio_extract-0.2.0/audio_extract.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 21:57:41.771234 audio_extract-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     2442 2023-04-22 21:51:50.000000 audio_extract-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 22:01:30.844972 audio_extract-0.3.0/
+-rw-rw-rw-   0        0        0     1090 2023-04-22 17:27:29.000000 audio_extract-0.3.0/LICENSE.md
+-rw-rw-rw-   0        0        0     4308 2023-04-22 22:01:30.842971 audio_extract-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3393 2023-04-22 22:01:19.000000 audio_extract-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 22:01:30.809971 audio_extract-0.3.0/audio_extract/
+-rw-rw-rw-   0        0        0     1705 2023-04-22 21:37:32.000000 audio_extract-0.3.0/audio_extract/__init__.py
+-rw-rw-rw-   0        0        0      142 2023-04-22 18:09:12.000000 audio_extract-0.3.0/audio_extract/exceptions.py
+-rw-rw-rw-   0        0        0     1123 2023-04-22 21:31:51.000000 audio_extract-0.3.0/audio_extract/execute.py
+-rw-rw-rw-   0        0        0     1798 2023-04-22 21:45:01.000000 audio_extract-0.3.0/audio_extract/ffmpeg_tools.py
+-rw-rw-rw-   0        0        0     1245 2023-04-22 21:50:51.000000 audio_extract-0.3.0/audio_extract/utils.py
+-rw-rw-rw-   0        0        0     2859 2023-04-22 19:49:07.000000 audio_extract-0.3.0/audio_extract/validators.py
+drwxrwxrwx   0        0        0        0 2023-04-22 22:01:30.840971 audio_extract-0.3.0/audio_extract.egg-info/
+-rw-rw-rw-   0        0        0     4308 2023-04-22 22:01:30.000000 audio_extract-0.3.0/audio_extract.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2023-04-22 22:01:30.000000 audio_extract-0.3.0/audio_extract.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 22:01:30.000000 audio_extract-0.3.0/audio_extract.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-22 22:01:30.000000 audio_extract-0.3.0/audio_extract.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       70 2023-04-22 22:01:30.000000 audio_extract-0.3.0/audio_extract.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-22 22:01:30.000000 audio_extract-0.3.0/audio_extract.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 22:01:30.844972 audio_extract-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     2436 2023-04-22 22:00:52.000000 audio_extract-0.3.0/setup.py
```

### Comparing `audio_extract-0.2.0/LICENSE.md` & `audio_extract-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `audio_extract-0.2.0/PKG-INFO` & `audio_extract-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: audio_extract
-Version: 0.2.0
+Version: 0.3.0
 Summary: Extract and trim audio from videos or trim audios.
-Home-page: https://github.com/riad-azz/py-audio-extract
+Home-page: https://github.com/riad-azz/audio-extract
 Author: riad-azz
 Author-email: riadh.azzoun@hotmail.com
 License: MIT License
-Project-URL: Source, https://github.com/riad-azz/py-audio-extract
+Project-URL: Source, https://github.com/riad-azz/audio-extract
 Keywords: convert video,audio,ffmpeg,video to mp3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -103,40 +103,40 @@
 * **`--duration`** or **`-d`**
 
 The duration of the output in `HH:MM:SS` or `MM:SS` format.
 
 ### Extract full audio
 
 ```bash
-extract-audio --input video.mp4 --output audio.mp3
+audio-extract --input video.mp4 --output audio.mp3
 ```
 
 This command will create a mp3 file called `audio.mp3` that contains the full audio of the video file `video.mp4`.
 
 #### Extract sub clip audio
 
 ```bash
-extract-audio --input video.mp4 --output audio.mp3 --start 00:00:30
+audio-extract --input video.mp4 --output audio.mp3 --start 00:00:30
 ```
 
 This would create a mp3 file called `audio.mp3` that starts after the first 30 seconds of the video file `video.mp4`.
 
 #### Extract sub clip audio with custom duration
 
 ```bash
-extract-audio --input video.mp4 --output audio.mp3 --start '00:25' --duration '01:15'
+audio-extract --input video.mp4 --output audio.mp3 --start '00:25' --duration '01:15'
 ```
 
 This command will convert video file `video.mp4` to a mp3 file starting from `00:25` to `01:15`
 called `audio.mp3` that will have a duration of `00:50`.
 
 #### Trim audio
 
 ```bash
-extract-audio --input audio.mp3 --output new_audio.mp3 --start '00:05' --duration '01:15'
+audio-extract --input audio.mp3 --output new_audio.mp3 --start '00:05' --duration '01:15'
 ```
 
 This command trim the audio starting from `00:05` to `01:15` of the file `audio.mp3` to a mp3 file
 called `new_audio.mp3` that will have a duration of `01:10`.
 
 
 ## Authors
```

### Comparing `audio_extract-0.2.0/README.md` & `audio_extract-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -80,40 +80,40 @@
 * **`--duration`** or **`-d`**
 
 The duration of the output in `HH:MM:SS` or `MM:SS` format.
 
 ### Extract full audio
 
 ```bash
-extract-audio --input video.mp4 --output audio.mp3
+audio-extract --input video.mp4 --output audio.mp3
 ```
 
 This command will create a mp3 file called `audio.mp3` that contains the full audio of the video file `video.mp4`.
 
 #### Extract sub clip audio
 
 ```bash
-extract-audio --input video.mp4 --output audio.mp3 --start 00:00:30
+audio-extract --input video.mp4 --output audio.mp3 --start 00:00:30
 ```
 
 This would create a mp3 file called `audio.mp3` that starts after the first 30 seconds of the video file `video.mp4`.
 
 #### Extract sub clip audio with custom duration
 
 ```bash
-extract-audio --input video.mp4 --output audio.mp3 --start '00:25' --duration '01:15'
+audio-extract --input video.mp4 --output audio.mp3 --start '00:25' --duration '01:15'
 ```
 
 This command will convert video file `video.mp4` to a mp3 file starting from `00:25` to `01:15`
 called `audio.mp3` that will have a duration of `00:50`.
 
 #### Trim audio
 
 ```bash
-extract-audio --input audio.mp3 --output new_audio.mp3 --start '00:05' --duration '01:15'
+audio-extract --input audio.mp3 --output new_audio.mp3 --start '00:05' --duration '01:15'
 ```
 
 This command trim the audio starting from `00:05` to `01:15` of the file `audio.mp3` to a mp3 file
 called `new_audio.mp3` that will have a duration of `01:10`.
 
 
 ## Authors
```

### Comparing `audio_extract-0.2.0/audio_extract/__init__.py` & `audio_extract-0.3.0/audio_extract/__init__.py`

 * *Files identical despite different names*

### Comparing `audio_extract-0.2.0/audio_extract/execute.py` & `audio_extract-0.3.0/audio_extract/execute.py`

 * *Files identical despite different names*

### Comparing `audio_extract-0.2.0/audio_extract/ffmpeg_tools.py` & `audio_extract-0.3.0/audio_extract/ffmpeg_tools.py`

 * *Files identical despite different names*

### Comparing `audio_extract-0.2.0/audio_extract/utils.py` & `audio_extract-0.3.0/audio_extract/utils.py`

 * *Files identical despite different names*

### Comparing `audio_extract-0.2.0/audio_extract/validators.py` & `audio_extract-0.3.0/audio_extract/validators.py`

 * *Files identical despite different names*

### Comparing `audio_extract-0.2.0/audio_extract.egg-info/PKG-INFO` & `audio_extract-0.3.0/audio_extract.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: audio-extract
-Version: 0.2.0
+Version: 0.3.0
 Summary: Extract and trim audio from videos or trim audios.
-Home-page: https://github.com/riad-azz/py-audio-extract
+Home-page: https://github.com/riad-azz/audio-extract
 Author: riad-azz
 Author-email: riadh.azzoun@hotmail.com
 License: MIT License
-Project-URL: Source, https://github.com/riad-azz/py-audio-extract
+Project-URL: Source, https://github.com/riad-azz/audio-extract
 Keywords: convert video,audio,ffmpeg,video to mp3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -103,40 +103,40 @@
 * **`--duration`** or **`-d`**
 
 The duration of the output in `HH:MM:SS` or `MM:SS` format.
 
 ### Extract full audio
 
 ```bash
-extract-audio --input video.mp4 --output audio.mp3
+audio-extract --input video.mp4 --output audio.mp3
 ```
 
 This command will create a mp3 file called `audio.mp3` that contains the full audio of the video file `video.mp4`.
 
 #### Extract sub clip audio
 
 ```bash
-extract-audio --input video.mp4 --output audio.mp3 --start 00:00:30
+audio-extract --input video.mp4 --output audio.mp3 --start 00:00:30
 ```
 
 This would create a mp3 file called `audio.mp3` that starts after the first 30 seconds of the video file `video.mp4`.
 
 #### Extract sub clip audio with custom duration
 
 ```bash
-extract-audio --input video.mp4 --output audio.mp3 --start '00:25' --duration '01:15'
+audio-extract --input video.mp4 --output audio.mp3 --start '00:25' --duration '01:15'
 ```
 
 This command will convert video file `video.mp4` to a mp3 file starting from `00:25` to `01:15`
 called `audio.mp3` that will have a duration of `00:50`.
 
 #### Trim audio
 
 ```bash
-extract-audio --input audio.mp3 --output new_audio.mp3 --start '00:05' --duration '01:15'
+audio-extract --input audio.mp3 --output new_audio.mp3 --start '00:05' --duration '01:15'
 ```
 
 This command trim the audio starting from `00:05` to `01:15` of the file `audio.mp3` to a mp3 file
 called `new_audio.mp3` that will have a duration of `01:10`.
 
 
 ## Authors
```

### Comparing `audio_extract-0.2.0/setup.py` & `audio_extract-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,31 +40,31 @@
 ]
 
 long_description = open('README.md').read()
 long_description_content_type = 'text/markdown'
 
 setup(
     name='audio_extract',
-    version='0.2.0',
+    version='0.3.0',
     author='riad-azz',
     author_email='riadh.azzoun@hotmail.com',
     description='Extract and trim audio from videos or trim audios.',
     long_description=long_description,
     long_description_content_type=long_description_content_type,
-    url='https://github.com/riad-azz/py-audio-extract',
+    url='https://github.com/riad-azz/audio-extract',
     project_urls={
-        "Source": "https://github.com/riad-azz/py-audio-extract",
+        "Source": "https://github.com/riad-azz/audio-extract",
     },
     packages=find_packages(exclude=["docs", "tests"]),
     install_requires=requires,
     license="MIT License",
     keywords=["convert video", "audio", "ffmpeg", "video to mp3"],
     entry_points={
         'console_scripts': [
-            'extract-audio=audio_extract.execute:main',
+            'audio-extract=audio_extract.execute:main',
         ],
     },
     cmdclass={
         'add_to_path': AddToPathCommand,
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

