# Comparing `tmp/ascii-yt-2.1.0.tar.gz` & `tmp/ascii-yt-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascii-yt-2.1.0.tar", last modified: Wed Mar 29 15:09:45 2023, max compression
+gzip compressed data, was "ascii-yt-2.1.1.tar", last modified: Sun Apr 23 21:47:52 2023, max compression
```

## Comparing `ascii-yt-2.1.0.tar` & `ascii-yt-2.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 15:09:45.169287 ascii-yt-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-29 15:09:30.000000 ascii-yt-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-03-29 15:09:45.169287 ascii-yt-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-03-29 15:09:30.000000 ascii-yt-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 15:09:45.165287 ascii-yt-2.1.0/ascii_youtube/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 15:09:30.000000 ascii-yt-2.1.0/ascii_youtube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-03-29 15:09:30.000000 ascii-yt-2.1.0/ascii_youtube/ascii_frames.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-29 15:09:30.000000 ascii-yt-2.1.0/ascii_youtube/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-03-29 15:09:30.000000 ascii-yt-2.1.0/ascii_youtube/play.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 15:09:45.169287 ascii-yt-2.1.0/ascii_yt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-03-29 15:09:45.000000 ascii-yt-2.1.0/ascii_yt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-03-29 15:09:45.000000 ascii-yt-2.1.0/ascii_yt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 15:09:45.000000 ascii-yt-2.1.0/ascii_yt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-29 15:09:45.000000 ascii-yt-2.1.0/ascii_yt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-29 15:09:45.000000 ascii-yt-2.1.0/ascii_yt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-29 15:09:45.000000 ascii-yt-2.1.0/ascii_yt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-03-29 15:09:45.169287 ascii-yt-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-29 15:09:30.000000 ascii-yt-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:47:52.191089 ascii-yt-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-23 21:47:41.000000 ascii-yt-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-23 21:47:52.191089 ascii-yt-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-23 21:47:41.000000 ascii-yt-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:47:52.191089 ascii-yt-2.1.1/ascii_youtube/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:47:41.000000 ascii-yt-2.1.1/ascii_youtube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-23 21:47:41.000000 ascii-yt-2.1.1/ascii_youtube/ascii_frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-23 21:47:41.000000 ascii-yt-2.1.1/ascii_youtube/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-23 21:47:41.000000 ascii-yt-2.1.1/ascii_youtube/play.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:47:52.191089 ascii-yt-2.1.1/ascii_yt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-23 21:47:52.000000 ascii-yt-2.1.1/ascii_yt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-23 21:47:52.000000 ascii-yt-2.1.1/ascii_yt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 21:47:52.000000 ascii-yt-2.1.1/ascii_yt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-23 21:47:52.000000 ascii-yt-2.1.1/ascii_yt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-23 21:47:52.000000 ascii-yt-2.1.1/ascii_yt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-23 21:47:52.000000 ascii-yt-2.1.1/ascii_yt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-23 21:47:52.191089 ascii-yt-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-23 21:47:41.000000 ascii-yt-2.1.1/setup.py
```

### Comparing `ascii-yt-2.1.0/LICENSE` & `ascii-yt-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ascii-yt-2.1.0/PKG-INFO` & `ascii-yt-2.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: ascii-yt
-Version: 2.1.0
+Version: 2.1.1
 Summary: play any youtube video ▶ with ASCII in the terminal.
-Home-page: https://github.com/malkiAbdoo/ascii-yt
-Author: Malki Abderrahman
-Author-email: abdo.malkiep@gmail.com
-Project-URL: Source, https://github.com/malkiAbdoo/ascii-yt
-Project-URL: Tracker, https://github.com/joelibaceta/ascii-yt/issues
+Home-page: https://github.com/malkiii/ascii-yt
+Author: Malki Abdurrahman
+Project-URL: Source, https://github.com/malkiii/ascii-yt
+Project-URL: Tracker, https://github.com/malkiii/ascii-yt/issues
 Keywords: ascii,art,video,youtube,linux,shell,python,terminal
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align=center>
 
 # ascii-yt
 
 play any youtube video ▶ with ASCII in the terminal.
 
-[![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/malkiAbdoo/ascii-yt?color=red)](./ascii_video_player)
-[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/malkiAbdoo/ascii-yt/publish.yml?color=2fbe50&logo=github)](https://github.com/malkiAbdoo/ascii-yt/actions)
+[![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/malkiii/ascii-yt?color=red)](./ascii_video_player)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/malkiii/ascii-yt/publish.yml?color=2fbe50&logo=github)](https://github.com/malkiii/ascii-yt/actions)
 [![PyPI](https://img.shields.io/pypi/v/ascii-yt?label=pypi%20version&logo=pypi)](https://pypi.org/project/ascii-yt/)
 [![Twitter URL](https://img.shields.io/twitter/url?label=@malkiAbdoo&url=https%3A%2F%2Ftwitter.com%2FmalkiAbdoo)](https://twitter.com/malkiAbdoo)
 
-![Screenshot](https://raw.githubusercontent.com/malkiAbdoo/ascii-yt/main/images/example.gif)
+![Screenshot](./images/example.gif)
 
 </div>
 
 ## Requirements
 
 - python 3.3 or above
 - Linux or MacOS
@@ -88,14 +87,16 @@
 2. Resize it to the terminal size (if there's not a custom size in the options)
 3. Convert the frame to a grayscale image (black & white)
 4. Mapping each pixel to a given character depending on the grayscale value from black to the white. the default value: `" .'~;icok0XN"`
 
 5. finaly display the frame.
 
 <details>
+
 <summary>Overview</summary><br>
-<img src="https://raw.githubusercontent.com/malkiAbdoo/ascii-yt/main/images/explain.jpg" alt="overview" />
+<img src="https://raw.githubusercontent.com/malkiii/ascii-yt/main/images/explain.jpg" alt="overview" />
+
 </details>
 
 ## License
 
-Distributed under the [MIT](https://github.com/malkiAbdoo/ascii-yt/blob/main/LICENSE) license.
+Distributed under the [MIT](https://github.com/malkiii/ascii-yt/blob/main/LICENSE) license.
```

### Comparing `ascii-yt-2.1.0/README.md` & `ascii-yt-2.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 <div align=center>
 
 # ascii-yt
 
 play any youtube video ▶ with ASCII in the terminal.
 
-[![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/malkiAbdoo/ascii-yt?color=red)](./ascii_video_player)
-[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/malkiAbdoo/ascii-yt/publish.yml?color=2fbe50&logo=github)](https://github.com/malkiAbdoo/ascii-yt/actions)
+[![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/malkiii/ascii-yt?color=red)](./ascii_video_player)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/malkiii/ascii-yt/publish.yml?color=2fbe50&logo=github)](https://github.com/malkiii/ascii-yt/actions)
 [![PyPI](https://img.shields.io/pypi/v/ascii-yt?label=pypi%20version&logo=pypi)](https://pypi.org/project/ascii-yt/)
 [![Twitter URL](https://img.shields.io/twitter/url?label=@malkiAbdoo&url=https%3A%2F%2Ftwitter.com%2FmalkiAbdoo)](https://twitter.com/malkiAbdoo)
 
-![Screenshot](https://raw.githubusercontent.com/malkiAbdoo/ascii-yt/main/images/example.gif)
+![Screenshot](./images/example.gif)
 
 </div>
 
 ## Requirements
 
 - python 3.3 or above
 - Linux or MacOS
@@ -70,14 +70,16 @@
 2. Resize it to the terminal size (if there's not a custom size in the options)
 3. Convert the frame to a grayscale image (black & white)
 4. Mapping each pixel to a given character depending on the grayscale value from black to the white. the default value: `" .'~;icok0XN"`
 
 5. finaly display the frame.
 
 <details>
+
 <summary>Overview</summary><br>
-<img src="https://raw.githubusercontent.com/malkiAbdoo/ascii-yt/main/images/explain.jpg" alt="overview" />
+<img src="https://raw.githubusercontent.com/malkiii/ascii-yt/main/images/explain.jpg" alt="overview" />
+
 </details>
 
 ## License
 
-Distributed under the [MIT](https://github.com/malkiAbdoo/ascii-yt/blob/main/LICENSE) license.
+Distributed under the [MIT](https://github.com/malkiii/ascii-yt/blob/main/LICENSE) license.
```

### Comparing `ascii-yt-2.1.0/ascii_youtube/ascii_frames.py` & `ascii-yt-2.1.1/ascii_youtube/ascii_frames.py`

 * *Files identical despite different names*

### Comparing `ascii-yt-2.1.0/ascii_youtube/cli.py` & `ascii-yt-2.1.1/ascii_youtube/cli.py`

 * *Files identical despite different names*

### Comparing `ascii-yt-2.1.0/ascii_youtube/play.py` & `ascii-yt-2.1.1/ascii_youtube/play.py`

 * *Files identical despite different names*

### Comparing `ascii-yt-2.1.0/ascii_yt.egg-info/PKG-INFO` & `ascii-yt-2.1.1/ascii_yt.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: ascii-yt
-Version: 2.1.0
+Version: 2.1.1
 Summary: play any youtube video ▶ with ASCII in the terminal.
-Home-page: https://github.com/malkiAbdoo/ascii-yt
-Author: Malki Abderrahman
-Author-email: abdo.malkiep@gmail.com
-Project-URL: Source, https://github.com/malkiAbdoo/ascii-yt
-Project-URL: Tracker, https://github.com/joelibaceta/ascii-yt/issues
+Home-page: https://github.com/malkiii/ascii-yt
+Author: Malki Abdurrahman
+Project-URL: Source, https://github.com/malkiii/ascii-yt
+Project-URL: Tracker, https://github.com/malkiii/ascii-yt/issues
 Keywords: ascii,art,video,youtube,linux,shell,python,terminal
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align=center>
 
 # ascii-yt
 
 play any youtube video ▶ with ASCII in the terminal.
 
-[![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/malkiAbdoo/ascii-yt?color=red)](./ascii_video_player)
-[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/malkiAbdoo/ascii-yt/publish.yml?color=2fbe50&logo=github)](https://github.com/malkiAbdoo/ascii-yt/actions)
+[![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/malkiii/ascii-yt?color=red)](./ascii_video_player)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/malkiii/ascii-yt/publish.yml?color=2fbe50&logo=github)](https://github.com/malkiii/ascii-yt/actions)
 [![PyPI](https://img.shields.io/pypi/v/ascii-yt?label=pypi%20version&logo=pypi)](https://pypi.org/project/ascii-yt/)
 [![Twitter URL](https://img.shields.io/twitter/url?label=@malkiAbdoo&url=https%3A%2F%2Ftwitter.com%2FmalkiAbdoo)](https://twitter.com/malkiAbdoo)
 
-![Screenshot](https://raw.githubusercontent.com/malkiAbdoo/ascii-yt/main/images/example.gif)
+![Screenshot](./images/example.gif)
 
 </div>
 
 ## Requirements
 
 - python 3.3 or above
 - Linux or MacOS
@@ -88,14 +87,16 @@
 2. Resize it to the terminal size (if there's not a custom size in the options)
 3. Convert the frame to a grayscale image (black & white)
 4. Mapping each pixel to a given character depending on the grayscale value from black to the white. the default value: `" .'~;icok0XN"`
 
 5. finaly display the frame.
 
 <details>
+
 <summary>Overview</summary><br>
-<img src="https://raw.githubusercontent.com/malkiAbdoo/ascii-yt/main/images/explain.jpg" alt="overview" />
+<img src="https://raw.githubusercontent.com/malkiii/ascii-yt/main/images/explain.jpg" alt="overview" />
+
 </details>
 
 ## License
 
-Distributed under the [MIT](https://github.com/malkiAbdoo/ascii-yt/blob/main/LICENSE) license.
+Distributed under the [MIT](https://github.com/malkiii/ascii-yt/blob/main/LICENSE) license.
```

### Comparing `ascii-yt-2.1.0/setup.cfg` & `ascii-yt-2.1.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [metadata]
 name = ascii-yt
-version = 2.1.0
-author = Malki Abderrahman
-author_email = abdo.malkiep@gmail.com
+version = 2.1.1
+author = Malki Abdurrahman
 description = play any youtube video ▶ with ASCII in the terminal.
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/malkiAbdoo/ascii-yt
+url = https://github.com/malkiii/ascii-yt
 project_urls = 
-	Source=https://github.com/malkiAbdoo/ascii-yt
-	Tracker=https://github.com/joelibaceta/ascii-yt/issues
+	Source=https://github.com/malkiii/ascii-yt
+	Tracker=https://github.com/malkiii/ascii-yt/issues
 classifiers = 
-	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.10
-	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
+	Intended Audience :: Developers
 	Operating System :: OS Independent
+	Programming Language :: Python :: 3
+	Programming Language :: Python :: 3.10
 keywords = ascii, art, video, youtube, linux, shell, python, terminal
 
 [options]
 packages = find:
 include_package_data = True
 setup_requires = 
 	setuptools>=50.3.2
```

