# Comparing `tmp/image_frequency_analysis-0.1.tar.gz` & `tmp/image_frequency_analysis-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_frequency_analysis-0.1.tar", last modified: Sun Apr 23 12:27:12 2023, max compression
+gzip compressed data, was "image_frequency_analysis-0.2.0.tar", last modified: Sun Apr 23 13:24:25 2023, max compression
```

## Comparing `image_frequency_analysis-0.1.tar` & `image_frequency_analysis-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 12:27:12.639533 image_frequency_analysis-0.1/
--rw-rw-rw-   0        0        0     1086 2023-04-15 11:42:59.000000 image_frequency_analysis-0.1/LICENSE
--rw-rw-rw-   0        0        0      136 2023-04-23 12:27:12.637533 image_frequency_analysis-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      129 2023-04-15 11:42:59.000000 image_frequency_analysis-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 12:27:12.629532 image_frequency_analysis-0.1/image_frequency_analysis/
--rw-rw-rw-   0        0        0     1648 2023-04-16 07:20:17.000000 image_frequency_analysis-0.1/image_frequency_analysis/__init__.py
--rw-rw-rw-   0        0        0     4870 2023-04-16 07:04:45.000000 image_frequency_analysis-0.1/image_frequency_analysis/frequency_analysis.py
-drwxrwxrwx   0        0        0        0 2023-04-23 12:27:12.635533 image_frequency_analysis-0.1/image_frequency_analysis.egg-info/
--rw-rw-rw-   0        0        0      136 2023-04-23 12:27:12.000000 image_frequency_analysis-0.1/image_frequency_analysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2023-04-23 12:27:12.000000 image_frequency_analysis-0.1/image_frequency_analysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 12:27:12.000000 image_frequency_analysis-0.1/image_frequency_analysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-04-23 12:27:12.000000 image_frequency_analysis-0.1/image_frequency_analysis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-04-23 12:27:12.000000 image_frequency_analysis-0.1/image_frequency_analysis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 12:27:12.639533 image_frequency_analysis-0.1/setup.cfg
--rw-rw-rw-   0        0        0      277 2023-04-15 12:14:26.000000 image_frequency_analysis-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 13:24:24.920250 image_frequency_analysis-0.2.0/
+-rw-rw-rw-   0        0        0     1086 2023-04-15 11:42:59.000000 image_frequency_analysis-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      229 2023-04-23 13:24:24.918209 image_frequency_analysis-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      129 2023-04-15 11:42:59.000000 image_frequency_analysis-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 13:24:24.900193 image_frequency_analysis-0.2.0/image_frequency_analysis/
+-rw-rw-rw-   0        0        0     1648 2023-04-16 07:20:17.000000 image_frequency_analysis-0.2.0/image_frequency_analysis/__init__.py
+-rw-rw-rw-   0        0        0     4870 2023-04-16 07:04:45.000000 image_frequency_analysis-0.2.0/image_frequency_analysis/frequency_analysis.py
+drwxrwxrwx   0        0        0        0 2023-04-23 13:24:24.914207 image_frequency_analysis-0.2.0/image_frequency_analysis.egg-info/
+-rw-rw-rw-   0        0        0      229 2023-04-23 13:24:24.000000 image_frequency_analysis-0.2.0/image_frequency_analysis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2023-04-23 13:24:24.000000 image_frequency_analysis-0.2.0/image_frequency_analysis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 13:24:24.000000 image_frequency_analysis-0.2.0/image_frequency_analysis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-04-23 13:24:24.000000 image_frequency_analysis-0.2.0/image_frequency_analysis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-04-23 13:24:24.000000 image_frequency_analysis-0.2.0/image_frequency_analysis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 13:24:24.921229 image_frequency_analysis-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      572 2023-04-23 13:24:20.000000 image_frequency_analysis-0.2.0/setup.py
```

### Comparing `image_frequency_analysis-0.1/LICENSE` & `image_frequency_analysis-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `image_frequency_analysis-0.1/image_frequency_analysis/__init__.py` & `image_frequency_analysis-0.2.0/image_frequency_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `image_frequency_analysis-0.1/image_frequency_analysis/frequency_analysis.py` & `image_frequency_analysis-0.2.0/image_frequency_analysis/frequency_analysis.py`

 * *Files identical despite different names*

