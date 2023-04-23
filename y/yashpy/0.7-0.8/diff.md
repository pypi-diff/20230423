# Comparing `tmp/yashpy-0.7.tar.gz` & `tmp/yashpy-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yashpy-0.7.tar", last modified: Sun Apr 23 07:57:03 2023, max compression
+gzip compressed data, was "yashpy-0.8.tar", last modified: Sun Apr 23 08:01:45 2023, max compression
```

## Comparing `yashpy-0.7.tar` & `yashpy-0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 07:57:03.102169 yashpy-0.7/
--rw-rw-rw-   0        0        0      175 2023-04-23 07:57:03.101194 yashpy-0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1091 2023-04-22 07:53:52.000000 yashpy-0.7/licence.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 07:57:03.102169 yashpy-0.7/setup.cfg
--rw-rw-rw-   0        0        0      245 2023-04-23 07:56:48.000000 yashpy-0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:57:03.087529 yashpy-0.7/yashpy/
--rw-rw-rw-   0        0        0     2141 2023-04-23 07:56:57.000000 yashpy-0.7/yashpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:57:03.100218 yashpy-0.7/yashpy.egg-info/
--rw-rw-rw-   0        0        0      175 2023-04-23 07:57:02.000000 yashpy-0.7/yashpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      159 2023-04-23 07:57:02.000000 yashpy-0.7/yashpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 07:57:02.000000 yashpy-0.7/yashpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-23 07:57:02.000000 yashpy-0.7/yashpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 08:01:45.358585 yashpy-0.8/
+-rw-rw-rw-   0        0        0      175 2023-04-23 08:01:45.358585 yashpy-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1091 2023-04-22 07:53:52.000000 yashpy-0.8/licence.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 08:01:45.358585 yashpy-0.8/setup.cfg
+-rw-rw-rw-   0        0        0      245 2023-04-23 08:01:28.000000 yashpy-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 08:01:45.341993 yashpy-0.8/yashpy/
+-rw-rw-rw-   0        0        0     2139 2023-04-23 08:01:36.000000 yashpy-0.8/yashpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 08:01:45.356636 yashpy-0.8/yashpy.egg-info/
+-rw-rw-rw-   0        0        0      175 2023-04-23 08:01:45.000000 yashpy-0.8/yashpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      159 2023-04-23 08:01:45.000000 yashpy-0.8/yashpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 08:01:45.000000 yashpy-0.8/yashpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-23 08:01:45.000000 yashpy-0.8/yashpy.egg-info/top_level.txt
```

### Comparing `yashpy-0.7/licence.txt` & `yashpy-0.8/licence.txt`

 * *Files identical despite different names*

### Comparing `yashpy-0.7/yashpy/__init__.py` & `yashpy-0.8/yashpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,8 +111,8 @@
 #point2=(12,2)
 def distance(point1, point2):
     differences = [point1[x] - point2[x] for x in range(len(point1))]
     differences_squared = [difference ** 2 for difference in differences]
     sum_of_squares = sum(differences_squared)
     return sum_of_squares ** 0.5
 
-print(distance(point_1, point_2))
+print(distance(point1, point2))
```

