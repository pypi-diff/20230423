# Comparing `tmp/HackerGprat-0.3.4.tar.gz` & `tmp/HackerGprat-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HackerGprat-0.3.4.tar", last modified: Sun Apr  3 05:21:26 2022, max compression
+gzip compressed data, was "HackerGprat-0.3.5.tar", last modified: Sun Apr 23 13:05:26 2023, max compression
```

## Comparing `HackerGprat-0.3.4.tar` & `HackerGprat-0.3.5.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxrwx   0        0        0        0 2022-04-03 05:21:26.622051 HackerGprat-0.3.4/
--rw-rw-rw-   0        0        0      255 2022-01-30 10:19:44.000000 HackerGprat-0.3.4/LICENSE
--rw-rw-rw-   0        0        0     1792 2022-04-03 05:21:26.620044 HackerGprat-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0      986 2022-03-25 09:41:12.000000 HackerGprat-0.3.4/README.md
--rw-rw-rw-   0        0        0      110 2022-01-30 09:33:40.000000 HackerGprat-0.3.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-04-03 05:21:26.623047 HackerGprat-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0     2110 2022-04-03 05:20:58.000000 HackerGprat-0.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2022-04-03 05:21:26.264012 HackerGprat-0.3.4/src/
-drwxrwxrwx   0        0        0        0 2022-04-03 05:21:26.566046 HackerGprat-0.3.4/src/HackerGprat/
--rw-rw-rw-   0        0        0      208 2022-04-02 16:19:18.000000 HackerGprat-0.3.4/src/HackerGprat/__init__.py
--rw-rw-rw-   0        0        0     4318 2022-03-25 09:10:02.000000 HackerGprat-0.3.4/src/HackerGprat/basic.py
--rw-rw-rw-   0        0        0      629 2022-03-28 17:58:09.000000 HackerGprat-0.3.4/src/HackerGprat/converter.py
--rw-rw-rw-   0        0        0     1166 2022-04-01 16:34:34.000000 HackerGprat-0.3.4/src/HackerGprat/internet.py
--rw-rw-rw-   0        0        0      299 2022-04-02 16:49:28.000000 HackerGprat-0.3.4/src/HackerGprat/notification.py
--rw-rw-rw-   0        0        0      439 2022-04-02 14:37:03.000000 HackerGprat-0.3.4/src/HackerGprat/short_name.py
--rw-rw-rw-   0        0        0        0 2022-03-03 00:46:49.000000 HackerGprat-0.3.4/src/HackerGprat/test.py
--rw-rw-rw-   0        0        0      898 2022-04-01 16:54:44.000000 HackerGprat-0.3.4/src/HackerGprat/trading.py
--rw-rw-rw-   0        0        0      163 2022-03-25 08:56:37.000000 HackerGprat-0.3.4/src/HackerGprat/trading_indicator.py
--rw-rw-rw-   0        0        0     1252 2022-04-03 05:04:48.000000 HackerGprat-0.3.4/src/HackerGprat/yt.py
-drwxrwxrwx   0        0        0        0 2022-04-03 05:21:26.617055 HackerGprat-0.3.4/src/HackerGprat.egg-info/
--rw-rw-rw-   0        0        0     1792 2022-04-03 05:21:25.000000 HackerGprat-0.3.4/src/HackerGprat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      517 2022-04-03 05:21:26.000000 HackerGprat-0.3.4/src/HackerGprat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-03 05:21:25.000000 HackerGprat-0.3.4/src/HackerGprat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      133 2022-04-03 05:21:26.000000 HackerGprat-0.3.4/src/HackerGprat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-04-03 05:21:26.000000 HackerGprat-0.3.4/src/HackerGprat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 13:05:26.165809 HackerGprat-0.3.5/
+-rw-rw-rw-   0        0        0      255 2022-06-02 02:08:29.000000 HackerGprat-0.3.5/LICENSE
+-rw-rw-rw-   0        0        0     1751 2023-04-23 13:05:26.163807 HackerGprat-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0      986 2022-06-02 02:08:29.000000 HackerGprat-0.3.5/README.md
+-rw-rw-rw-   0        0        0      110 2022-06-02 02:08:29.000000 HackerGprat-0.3.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-23 13:05:26.165809 HackerGprat-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     2408 2023-04-23 13:04:39.000000 HackerGprat-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 13:05:25.907752 HackerGprat-0.3.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-23 13:05:26.105811 HackerGprat-0.3.5/src/HackerGprat/
+-rw-rw-rw-   0        0        0      208 2022-06-02 02:08:29.000000 HackerGprat-0.3.5/src/HackerGprat/__init__.py
+-rw-rw-rw-   0        0        0     4318 2022-06-02 02:08:29.000000 HackerGprat-0.3.5/src/HackerGprat/basic.py
+-rw-rw-rw-   0        0        0      629 2022-06-02 02:08:29.000000 HackerGprat-0.3.5/src/HackerGprat/converter.py
+-rw-rw-rw-   0        0        0     1166 2022-06-02 02:08:29.000000 HackerGprat-0.3.5/src/HackerGprat/internet.py
+-rw-rw-rw-   0        0        0      299 2022-06-02 02:08:29.000000 HackerGprat-0.3.5/src/HackerGprat/notification.py
+-rw-rw-rw-   0        0        0      439 2022-06-02 02:08:29.000000 HackerGprat-0.3.5/src/HackerGprat/short_name.py
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:08:29.000000 HackerGprat-0.3.5/src/HackerGprat/test.py
+-rw-rw-rw-   0        0        0      898 2022-06-02 02:08:29.000000 HackerGprat-0.3.5/src/HackerGprat/trading.py
+-rw-rw-rw-   0        0        0      163 2022-06-02 02:08:29.000000 HackerGprat-0.3.5/src/HackerGprat/trading_indicator.py
+-rw-rw-rw-   0        0        0     1252 2022-06-02 02:08:29.000000 HackerGprat-0.3.5/src/HackerGprat/yt.py
+drwxrwxrwx   0        0        0        0 2023-04-23 13:05:26.149812 HackerGprat-0.3.5/src/HackerGprat.egg-info/
+-rw-rw-rw-   0        0        0     1751 2023-04-23 13:05:25.000000 HackerGprat-0.3.5/src/HackerGprat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      531 2023-04-23 13:05:25.000000 HackerGprat-0.3.5/src/HackerGprat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 13:05:25.000000 HackerGprat-0.3.5/src/HackerGprat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      190 2023-04-23 13:05:25.000000 HackerGprat-0.3.5/src/HackerGprat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-23 13:05:25.000000 HackerGprat-0.3.5/src/HackerGprat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 13:05:26.161806 HackerGprat-0.3.5/tests/
+-rw-rw-rw-   0        0        0      133 2022-06-02 02:08:29.000000 HackerGprat-0.3.5/tests/test.py
```

### Comparing `HackerGprat-0.3.4/PKG-INFO` & `HackerGprat-0.3.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: HackerGprat
-Version: 0.3.4
+Version: 0.3.5
 Summary: Here You can find Userfull fucntion which you need in your every python packages.
 Home-page: https://github.com/HackerGprat/HackerGprat-PIP-Library/
 Author: HackerGprat
 Author-email: Sorry@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/HackerGprat/HackerGprat-PIP-Library/issues
 Project-URL: Website, https://hackergprat.github.io
 Project-URL: Instagram, https://instagram.com/HackerGprat
 Project-URL: YouTube, https://youtube.com/HackerGprat
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -74,9 +72,7 @@
 
 
 ----
 ## EXTRA LINKS
 - [PYPI LIBRARY](https://pypi.org/project/HackerGprat/)
 
 
-
-
```

### Comparing `HackerGprat-0.3.4/README.md` & `HackerGprat-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `HackerGprat-0.3.4/setup.py` & `HackerGprat-0.3.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,38 +3,47 @@
 with open( "README.md" , 'r', encoding="utf-8") as fh:
     long_description = fh.read()
 
     # print( long_description )
     
 setuptools.setup(
     name = "HackerGprat",
-    version = "0.3.4",
+    version = "0.3.5",
     author = "HackerGprat",
     author_email = "Sorry@gmail.com",   # "https://youtube.com/HackerGprat" # test it working or not
     description = "Here You can find Userfull fucntion which you need in your every python packages.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/HackerGprat/HackerGprat-PIP-Library/",
     
     install_requires =['numpy',
                        'pandas',
                        'matplotlib',
+                       'ipython',
                        'scipy',
-                       'binance',
-                       'python-binance',
+                       'scikit-learn',
+                       'seaborn',
                        'pillow',
-                       'setuptools',
                        'wheel',
                        'requests',
-                       'ipython',
-                       'scikit-learn',
-                       'sklearn',
-                       'seaborn',
                        'bs4',
-                       'plyer'
+                       'plyer',
+                       'binance',
+                       'python-binance',
+                       'setuptools',
+                       'jupyterlab',
+                       'jupyter',
+                       'nltk',
+                       'spacy',
+                       'textblob',
+                       'CoreNLP',
+                       'docx',
+                       'PyPDF2',
+                       'build'
+                       
                     #    '--upgrade pip' error while buidling dont use this
         ],
     
     project_urls={
         "Bug Tracker" : "https://github.com/HackerGprat/HackerGprat-PIP-Library/issues",
         "Website" : "https://hackergprat.github.io",
         "Instagram": "https://instagram.com/HackerGprat",
```

### Comparing `HackerGprat-0.3.4/src/HackerGprat/basic.py` & `HackerGprat-0.3.5/src/HackerGprat/basic.py`

 * *Files identical despite different names*

### Comparing `HackerGprat-0.3.4/src/HackerGprat/converter.py` & `HackerGprat-0.3.5/src/HackerGprat/converter.py`

 * *Files identical despite different names*

### Comparing `HackerGprat-0.3.4/src/HackerGprat/internet.py` & `HackerGprat-0.3.5/src/HackerGprat/internet.py`

 * *Files identical despite different names*

### Comparing `HackerGprat-0.3.4/src/HackerGprat/trading.py` & `HackerGprat-0.3.5/src/HackerGprat/trading.py`

 * *Files identical despite different names*

### Comparing `HackerGprat-0.3.4/src/HackerGprat/yt.py` & `HackerGprat-0.3.5/src/HackerGprat/yt.py`

 * *Files identical despite different names*

### Comparing `HackerGprat-0.3.4/src/HackerGprat.egg-info/PKG-INFO` & `HackerGprat-0.3.5/src/HackerGprat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: HackerGprat
-Version: 0.3.4
+Version: 0.3.5
 Summary: Here You can find Userfull fucntion which you need in your every python packages.
 Home-page: https://github.com/HackerGprat/HackerGprat-PIP-Library/
 Author: HackerGprat
 Author-email: Sorry@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/HackerGprat/HackerGprat-PIP-Library/issues
 Project-URL: Website, https://hackergprat.github.io
 Project-URL: Instagram, https://instagram.com/HackerGprat
 Project-URL: YouTube, https://youtube.com/HackerGprat
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -74,9 +72,7 @@
 
 
 ----
 ## EXTRA LINKS
 - [PYPI LIBRARY](https://pypi.org/project/HackerGprat/)
 
 
-
-
```

### Comparing `HackerGprat-0.3.4/src/HackerGprat.egg-info/SOURCES.txt` & `HackerGprat-0.3.5/src/HackerGprat.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,9 @@
 src/HackerGprat/trading.py
 src/HackerGprat/trading_indicator.py
 src/HackerGprat/yt.py
 src/HackerGprat.egg-info/PKG-INFO
 src/HackerGprat.egg-info/SOURCES.txt
 src/HackerGprat.egg-info/dependency_links.txt
 src/HackerGprat.egg-info/requires.txt
-src/HackerGprat.egg-info/top_level.txt
+src/HackerGprat.egg-info/top_level.txt
+tests/test.py
```

