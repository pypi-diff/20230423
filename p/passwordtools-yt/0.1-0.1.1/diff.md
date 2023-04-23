# Comparing `tmp/passwordtools-yt-0.1.tar.gz` & `tmp/passwordtools-yt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passwordtools-yt-0.1.tar", last modified: Sun Apr 23 16:20:50 2023, max compression
+gzip compressed data, was "passwordtools-yt-0.1.1.tar", last modified: Sun Apr 23 16:54:22 2023, max compression
```

## Comparing `passwordtools-yt-0.1.tar` & `passwordtools-yt-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 16:20:50.073531 passwordtools-yt-0.1/
--rw-rw-rw-   0        0        0     1084 2023-04-19 17:45:55.000000 passwordtools-yt-0.1/LICENCE
--rw-rw-rw-   0        0        0      448 2023-04-23 16:20:50.068527 passwordtools-yt-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1407 2023-04-23 14:10:48.000000 passwordtools-yt-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 16:20:50.040449 passwordtools-yt-0.1/passwordtools/
--rw-rw-rw-   0        0        0      219 2023-04-21 15:19:11.000000 passwordtools-yt-0.1/passwordtools/__init__.py
--rw-rw-rw-   0        0        0     2126 2023-04-21 15:03:13.000000 passwordtools-yt-0.1/passwordtools/main.py
-drwxrwxrwx   0        0        0        0 2023-04-23 16:20:50.063505 passwordtools-yt-0.1/passwordtools_yt.egg-info/
--rw-rw-rw-   0        0        0      448 2023-04-23 16:20:49.000000 passwordtools-yt-0.1/passwordtools_yt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-04-23 16:20:49.000000 passwordtools-yt-0.1/passwordtools_yt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 16:20:49.000000 passwordtools-yt-0.1/passwordtools_yt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-23 16:20:49.000000 passwordtools-yt-0.1/passwordtools_yt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 16:20:50.074527 passwordtools-yt-0.1/setup.cfg
--rw-rw-rw-   0        0        0      539 2023-04-23 16:13:08.000000 passwordtools-yt-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 16:54:22.130847 passwordtools-yt-0.1.1/
+-rw-rw-rw-   0        0        0     1084 2023-04-19 17:45:55.000000 passwordtools-yt-0.1.1/LICENCE
+-rw-rw-rw-   0        0        0     1915 2023-04-23 16:54:22.124870 passwordtools-yt-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1397 2023-04-23 16:51:17.000000 passwordtools-yt-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 16:54:22.098843 passwordtools-yt-0.1.1/passwordtools/
+-rw-rw-rw-   0        0        0      219 2023-04-21 15:19:11.000000 passwordtools-yt-0.1.1/passwordtools/__init__.py
+-rw-rw-rw-   0        0        0     2126 2023-04-21 15:03:13.000000 passwordtools-yt-0.1.1/passwordtools/main.py
+drwxrwxrwx   0        0        0        0 2023-04-23 16:54:22.120842 passwordtools-yt-0.1.1/passwordtools_yt.egg-info/
+-rw-rw-rw-   0        0        0     1915 2023-04-23 16:54:22.000000 passwordtools-yt-0.1.1/passwordtools_yt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-04-23 16:54:22.000000 passwordtools-yt-0.1.1/passwordtools_yt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 16:54:22.000000 passwordtools-yt-0.1.1/passwordtools_yt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-23 16:54:22.000000 passwordtools-yt-0.1.1/passwordtools_yt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 16:54:22.130847 passwordtools-yt-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      706 2023-04-23 16:53:47.000000 passwordtools-yt-0.1.1/setup.py
```

### Comparing `passwordtools-yt-0.1/LICENCE` & `passwordtools-yt-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `passwordtools-yt-0.1/README.md` & `passwordtools-yt-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,15 @@
     pip install passwordtool-yt
 
 
 For more info, go to documentation.
 ## Documentation.
 
 For more information on how to use PasswordGenerator, please refer to the documentation website:
-
-https://passwordgenerator.readthedocs.io/en/latest/
+https://yair-t.github.io/passwordtools-docs
 
 
 ### License
 passwordtools is licensed under the MIT License.
```

### Comparing `passwordtools-yt-0.1/passwordtools/main.py` & `passwordtools-yt-0.1.1/passwordtools/main.py`

 * *Files identical despite different names*

### Comparing `passwordtools-yt-0.1/setup.py` & `passwordtools-yt-0.1.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 from setuptools import setup
+import os
 
 setup(
     name="passwordtools-yt",
-    version="0.1",
+    version="0.1.1",
+    readme="README.md",
     description="A package for creating passwords and testing password strength",
+    long_description=open('README.md').read(),
+    long_description_content_type="text/markdown",
+    python_requires='>=3.11',
     author="Yair-T",
     url="https://github.com/Yair-T",
     packages=['passwordtools'],
     license='MIT LICENSE',
     project_urls={
         'Documentation': 'https://yair-t.github.io/passwordtools-docs/',
         'Bug Tracker': 'https://github.com/Yair-T/passwordtools/issues',
         'Source Code': 'https://github.com/Yair-T/passwordtools'
     },
-)
+)
```

