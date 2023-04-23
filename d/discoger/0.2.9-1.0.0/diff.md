# Comparing `tmp/discoger-0.2.9.tar.gz` & `tmp/discoger-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discoger-0.2.9.tar", last modified: Thu Nov  3 20:51:26 2022, max compression
+gzip compressed data, was "discoger-1.0.0.tar", last modified: Sun Apr 23 12:26:26 2023, max compression
```

## Comparing `discoger-0.2.9.tar` & `discoger-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 20:51:26.449648 discoger-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-11-03 20:51:10.000000 discoger-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1902 2022-11-03 20:51:26.449648 discoger-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      747 2022-11-03 20:51:10.000000 discoger-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 20:51:26.445648 discoger-0.2.9/discoger/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 20:51:10.000000 discoger-0.2.9/discoger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-11-03 20:51:10.000000 discoger-0.2.9/discoger/_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     8350 2022-11-03 20:51:10.000000 discoger-0.2.9/discoger/discoger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 20:51:26.449648 discoger-0.2.9/discoger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1902 2022-11-03 20:51:26.000000 discoger-0.2.9/discoger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-11-03 20:51:26.000000 discoger-0.2.9/discoger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-03 20:51:26.000000 discoger-0.2.9/discoger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-11-03 20:51:26.000000 discoger-0.2.9/discoger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-11-03 20:51:26.000000 discoger-0.2.9/discoger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-03 20:51:26.000000 discoger-0.2.9/discoger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-11-03 20:51:26.449648 discoger-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1823 2022-11-03 20:51:10.000000 discoger-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:26:26.448911 discoger-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 12:26:13.000000 discoger-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-23 12:26:26.448911 discoger-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-23 12:26:13.000000 discoger-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:26:26.448911 discoger-1.0.0/discoger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:26:13.000000 discoger-1.0.0/discoger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-23 12:26:13.000000 discoger-1.0.0/discoger/_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-04-23 12:26:13.000000 discoger-1.0.0/discoger/discoger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:26:26.448911 discoger-1.0.0/discoger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-23 12:26:26.000000 discoger-1.0.0/discoger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-23 12:26:26.000000 discoger-1.0.0/discoger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 12:26:26.000000 discoger-1.0.0/discoger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-23 12:26:26.000000 discoger-1.0.0/discoger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-23 12:26:26.000000 discoger-1.0.0/discoger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 12:26:26.000000 discoger-1.0.0/discoger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-23 12:26:26.448911 discoger-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-23 12:26:13.000000 discoger-1.0.0/setup.py
```

### Comparing `discoger-0.2.9/LICENSE` & `discoger-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `discoger-0.2.9/PKG-INFO` & `discoger-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: discoger
-Version: 0.2.9
+Version: 1.0.0
 Summary: Get notification from Discogs
 Home-page: https://github.com/beudbeud/discoger
 Author: Beudbeud
 Author-email: beudbeud@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/beudbeud/discoger/archive/0.2.9.tar.gz
+Download-URL: https://github.com/beudbeud/discoger/archive/1.0.0.tar.gz
 Description: # Discoger
         
         Telegram bot for checking if there are new sell in one specific list on Discogs
         
         ## How to use it
         
         ### Installation
@@ -40,17 +40,16 @@
         ```
         docker container run -v ./:/root/.config/discoger beudbeud/discoger
         ```
         
 Keywords: discogs,telegram,bot
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `discoger-0.2.9/README.md` & `discoger-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `discoger-0.2.9/discoger.egg-info/PKG-INFO` & `discoger-1.0.0/discoger.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: discoger
-Version: 0.2.9
+Version: 1.0.0
 Summary: Get notification from Discogs
 Home-page: https://github.com/beudbeud/discoger
 Author: Beudbeud
 Author-email: beudbeud@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/beudbeud/discoger/archive/0.2.9.tar.gz
+Download-URL: https://github.com/beudbeud/discoger/archive/1.0.0.tar.gz
 Description: # Discoger
         
         Telegram bot for checking if there are new sell in one specific list on Discogs
         
         ## How to use it
         
         ### Installation
@@ -40,17 +40,16 @@
         ```
         docker container run -v ./:/root/.config/discoger beudbeud/discoger
         ```
         
 Keywords: discogs,telegram,bot
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `discoger-0.2.9/setup.py` & `discoger-1.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,19 +20,18 @@
     url=f'https://github.com/{package_info.__github_username__}/{package_info.__title__}',  #
     download_url=f'https://github.com/{package_info.__github_username__}/{package_info.__title__}/archive/{package_info.__version__}.tar.gz',
     keywords=package_info.__keywords__,
     install_requires=requirements,
     entry_points={"console_scripts": ["discoger = discoger.discoger:main"]},
     classifiers=[
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
-        'Development Status :: 4 - Beta',
+        'Development Status :: 5 - Production/Stable',
         # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state
         'Programming Language :: Python :: 3',  # Specify which python versions that you want
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Topic :: Internet :: WWW/HTTP',
         'Operating System :: OS Independent'
     ],
-    python_requires='>=3.6'
+    python_requires='>=3.7'
 )
```

