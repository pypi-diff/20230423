# Comparing `tmp/audio_extract-0.3.0.tar.gz` & `tmp/audio_extract-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio_extract-0.3.0.tar", last modified: Sat Apr 22 22:01:30 2023, max compression
+gzip compressed data, was "audio_extract-0.3.1.tar", last modified: Sat Apr 22 22:25:02 2023, max compression
```

## Comparing `audio_extract-0.3.0.tar` & `audio_extract-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 22:01:30.844972 audio_extract-0.3.0/
--rw-rw-rw-   0        0        0     1090 2023-04-22 17:27:29.000000 audio_extract-0.3.0/LICENSE.md
--rw-rw-rw-   0        0        0     4308 2023-04-22 22:01:30.842971 audio_extract-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     3393 2023-04-22 22:01:19.000000 audio_extract-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 22:01:30.809971 audio_extract-0.3.0/audio_extract/
--rw-rw-rw-   0        0        0     1705 2023-04-22 21:37:32.000000 audio_extract-0.3.0/audio_extract/__init__.py
--rw-rw-rw-   0        0        0      142 2023-04-22 18:09:12.000000 audio_extract-0.3.0/audio_extract/exceptions.py
--rw-rw-rw-   0        0        0     1123 2023-04-22 21:31:51.000000 audio_extract-0.3.0/audio_extract/execute.py
--rw-rw-rw-   0        0        0     1798 2023-04-22 21:45:01.000000 audio_extract-0.3.0/audio_extract/ffmpeg_tools.py
--rw-rw-rw-   0        0        0     1245 2023-04-22 21:50:51.000000 audio_extract-0.3.0/audio_extract/utils.py
--rw-rw-rw-   0        0        0     2859 2023-04-22 19:49:07.000000 audio_extract-0.3.0/audio_extract/validators.py
-drwxrwxrwx   0        0        0        0 2023-04-22 22:01:30.840971 audio_extract-0.3.0/audio_extract.egg-info/
--rw-rw-rw-   0        0        0     4308 2023-04-22 22:01:30.000000 audio_extract-0.3.0/audio_extract.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2023-04-22 22:01:30.000000 audio_extract-0.3.0/audio_extract.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 22:01:30.000000 audio_extract-0.3.0/audio_extract.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-22 22:01:30.000000 audio_extract-0.3.0/audio_extract.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       70 2023-04-22 22:01:30.000000 audio_extract-0.3.0/audio_extract.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-22 22:01:30.000000 audio_extract-0.3.0/audio_extract.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 22:01:30.844972 audio_extract-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     2436 2023-04-22 22:00:52.000000 audio_extract-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 22:25:02.133358 audio_extract-0.3.1/
+-rw-rw-rw-   0        0        0     1090 2023-04-22 17:27:29.000000 audio_extract-0.3.1/LICENSE.md
+-rw-rw-rw-   0        0        0     4308 2023-04-22 22:25:02.132357 audio_extract-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3393 2023-04-22 22:01:19.000000 audio_extract-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 22:25:02.099357 audio_extract-0.3.1/audio_extract/
+-rw-rw-rw-   0        0        0     1723 2023-04-22 22:19:55.000000 audio_extract-0.3.1/audio_extract/__init__.py
+-rw-rw-rw-   0        0        0      142 2023-04-22 18:09:12.000000 audio_extract-0.3.1/audio_extract/exceptions.py
+-rw-rw-rw-   0        0        0     1123 2023-04-22 21:31:51.000000 audio_extract-0.3.1/audio_extract/execute.py
+-rw-rw-rw-   0        0        0     1798 2023-04-22 21:45:01.000000 audio_extract-0.3.1/audio_extract/ffmpeg_tools.py
+-rw-rw-rw-   0        0        0     1314 2023-04-22 22:19:05.000000 audio_extract-0.3.1/audio_extract/utils.py
+-rw-rw-rw-   0        0        0     2859 2023-04-22 19:49:07.000000 audio_extract-0.3.1/audio_extract/validators.py
+drwxrwxrwx   0        0        0        0 2023-04-22 22:25:02.129357 audio_extract-0.3.1/audio_extract.egg-info/
+-rw-rw-rw-   0        0        0     4308 2023-04-22 22:25:01.000000 audio_extract-0.3.1/audio_extract.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2023-04-22 22:25:02.000000 audio_extract-0.3.1/audio_extract.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 22:25:01.000000 audio_extract-0.3.1/audio_extract.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-22 22:25:01.000000 audio_extract-0.3.1/audio_extract.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       86 2023-04-22 22:25:01.000000 audio_extract-0.3.1/audio_extract.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-22 22:25:01.000000 audio_extract-0.3.1/audio_extract.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 22:25:02.133358 audio_extract-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     2460 2023-04-22 22:24:32.000000 audio_extract-0.3.1/setup.py
```

### Comparing `audio_extract-0.3.0/LICENSE.md` & `audio_extract-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `audio_extract-0.3.0/PKG-INFO` & `audio_extract-0.3.1/audio_extract.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: audio_extract
-Version: 0.3.0
+Name: audio-extract
+Version: 0.3.1
 Summary: Extract and trim audio from videos or trim audios.
 Home-page: https://github.com/riad-azz/audio-extract
 Author: riad-azz
 Author-email: riadh.azzoun@hotmail.com
 License: MIT License
 Project-URL: Source, https://github.com/riad-azz/audio-extract
 Keywords: convert video,audio,ffmpeg,video to mp3
```

### Comparing `audio_extract-0.3.0/README.md` & `audio_extract-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `audio_extract-0.3.0/audio_extract/__init__.py` & `audio_extract-0.3.1/audio_extract/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 def run(input_path: str, output_path: str = "./audio.mp3", start_time: str = "00:00", duration: str | None = None):
     input_path = os.path.abspath(input_path)
     output_path = os.path.abspath(output_path)
 
     if not os.path.exists(input_path):
-        utils.print_error(f"{input_path} does not exist")
+        utils.print_error(f"Failed : {input_path} does not exist")
         return False
 
     print(f"Processing audio for {input_path} please wait...")
 
     if not output_path.endswith(".mp3"):
         output_path += ".mp3"
 
@@ -40,9 +40,9 @@
             return extract_full_audio(input_path, output_path, start_time)
         else:
             return extract_sub_audio(input_path, output_path, start_time, duration)
     except Exception as e:
         if isinstance(e, AudioExtractException):
             utils.print_error(e.message)
         else:
-            utils.print_error(f"Something went wrong, {e}")
+            utils.print_error(f"Failed : Something went wrong, {e}")
         return False
```

### Comparing `audio_extract-0.3.0/audio_extract/execute.py` & `audio_extract-0.3.1/audio_extract/execute.py`

 * *Files identical despite different names*

### Comparing `audio_extract-0.3.0/audio_extract/ffmpeg_tools.py` & `audio_extract-0.3.1/audio_extract/ffmpeg_tools.py`

 * *Files identical despite different names*

### Comparing `audio_extract-0.3.0/audio_extract/utils.py` & `audio_extract-0.3.1/audio_extract/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+import os
 import mutagen
+from colorama import Fore, Style
+
+os.system("color")
 
 
 def print_success(text: str):
-    print("\033[32m" + "✅  " + f"{text}" + "\033[0m")
+    print(f"{Fore.LIGHTGREEN_EX}{text}{Style.RESET_ALL}")
 
 
 def print_error(text: str):
-    print("\033[31m" + "❌  " + f"{text}" + "\033[0m")
+    print(f"{Fore.LIGHTRED_EX}{text}{Style.RESET_ALL}")
 
 
 def media_duration(path: str):
     file = mutagen.File(path)
     duration = file.info.length
     return duration
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `audio_extract-0.3.0/audio_extract/validators.py` & `audio_extract-0.3.1/audio_extract/validators.py`

 * *Files identical despite different names*

### Comparing `audio_extract-0.3.0/audio_extract.egg-info/PKG-INFO` & `audio_extract-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: audio-extract
-Version: 0.3.0
+Name: audio_extract
+Version: 0.3.1
 Summary: Extract and trim audio from videos or trim audios.
 Home-page: https://github.com/riad-azz/audio-extract
 Author: riad-azz
 Author-email: riadh.azzoun@hotmail.com
 License: MIT License
 Project-URL: Source, https://github.com/riad-azz/audio-extract
 Keywords: convert video,audio,ffmpeg,video to mp3
```

### Comparing `audio_extract-0.3.0/setup.py` & `audio_extract-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,26 +29,27 @@
 
         package_dir = Path(__file__).resolve().parent
         if str(package_dir) not in sys.path:
             sys.path.insert(0, str(package_dir))
 
 
 requires = [
+    "colorama>=0.4.6",
     "ffmpeg>=1.4",
     "imageio-ffmpeg>=0.4.8",
     "mutagen>=1.46.0",
     "py-file-type>=0.1.0",
 ]
 
 long_description = open('README.md').read()
 long_description_content_type = 'text/markdown'
 
 setup(
     name='audio_extract',
-    version='0.3.0',
+    version='0.3.1',
     author='riad-azz',
     author_email='riadh.azzoun@hotmail.com',
     description='Extract and trim audio from videos or trim audios.',
     long_description=long_description,
     long_description_content_type=long_description_content_type,
     url='https://github.com/riad-azz/audio-extract',
     project_urls={
```

