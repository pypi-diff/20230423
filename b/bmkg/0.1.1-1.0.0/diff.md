# Comparing `tmp/bmkg-0.1.1.tar.gz` & `tmp/bmkg-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmkg-0.1.1.tar", last modified: Wed Jul 13 15:31:48 2022, max compression
+gzip compressed data, was "bmkg-1.0.0.tar", last modified: Sun Apr 23 16:28:37 2023, max compression
```

## Comparing `bmkg-0.1.1.tar` & `bmkg-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxrwx   0        0        0        0 2022-07-13 15:31:48.245713 bmkg-0.1.1/
--rw-rw-rw-   0        0        0     1082 2022-07-13 10:53:05.000000 bmkg-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1604 2022-07-13 15:31:48.279715 bmkg-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      797 2022-07-13 15:08:19.000000 bmkg-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2022-07-13 15:31:47.404714 bmkg-0.1.1/bmkg/
--rw-rw-rw-   0        0        0      222 2022-07-13 12:36:01.000000 bmkg-0.1.1/bmkg/__init__.py
--rw-rw-rw-   0        0        0     6705 2022-07-13 13:52:00.000000 bmkg-0.1.1/bmkg/area.py
--rw-rw-rw-   0        0        0     3784 2022-07-13 14:21:57.000000 bmkg-0.1.1/bmkg/bmkg.py
--rw-rw-rw-   0        0        0     3318 2022-07-13 14:57:45.000000 bmkg-0.1.1/bmkg/earthquake.py
--rw-rw-rw-   0        0        0     1166 2022-07-13 12:36:01.000000 bmkg-0.1.1/bmkg/province.py
--rw-rw-rw-   0        0        0       97 2022-07-13 13:50:59.000000 bmkg-0.1.1/bmkg/settings.py
--rw-rw-rw-   0        0        0     1087 2022-07-13 13:51:51.000000 bmkg-0.1.1/bmkg/weather.py
-drwxrwxrwx   0        0        0        0 2022-07-13 15:31:48.243713 bmkg-0.1.1/bmkg.egg-info/
--rw-rw-rw-   0        0        0     1604 2022-07-13 15:31:42.000000 bmkg-0.1.1/bmkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2022-07-13 15:31:42.000000 bmkg-0.1.1/bmkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-13 15:31:42.000000 bmkg-0.1.1/bmkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2022-07-13 15:31:42.000000 bmkg-0.1.1/bmkg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2022-07-13 15:31:42.000000 bmkg-0.1.1/bmkg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2022-07-13 15:31:48.321711 bmkg-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      951 2022-07-13 15:25:51.000000 bmkg-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 16:28:37.392893 bmkg-1.0.0/
+-rw-rw-rw-   0        0        0     1087 2023-03-20 02:31:47.000000 bmkg-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0      135 2023-03-20 02:35:35.000000 bmkg-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3637 2023-04-23 16:28:37.392893 bmkg-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2127 2023-04-23 14:00:34.000000 bmkg-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 16:28:37.316238 bmkg-1.0.0/bmkg/
+-rw-rw-rw-   0        0        0     1414 2023-04-23 16:21:05.000000 bmkg-1.0.0/bmkg/__init__.py
+-rw-rw-rw-   0        0        0     2115 2023-04-23 13:54:53.000000 bmkg-1.0.0/bmkg/base.py
+-rw-rw-rw-   0        0        0     9314 2023-04-23 13:54:53.000000 bmkg-1.0.0/bmkg/client.py
+-rw-rw-rw-   0        0        0     1461 2023-04-23 13:54:53.000000 bmkg-1.0.0/bmkg/constants.py
+-rw-rw-rw-   0        0        0     4027 2023-04-23 16:18:21.000000 bmkg-1.0.0/bmkg/earthquake.py
+-rw-rw-rw-   0        0        0     5067 2023-04-23 13:54:53.000000 bmkg-1.0.0/bmkg/enums.py
+-rw-rw-rw-   0        0        0     1271 2023-04-23 16:18:33.000000 bmkg-1.0.0/bmkg/errors.py
+-rw-rw-rw-   0        0        0     8501 2023-04-23 13:54:54.000000 bmkg-1.0.0/bmkg/forecast.py
+drwxrwxrwx   0        0        0        0 2023-04-23 16:28:37.391113 bmkg-1.0.0/bmkg.egg-info/
+-rw-rw-rw-   0        0        0     3637 2023-04-23 16:28:36.000000 bmkg-1.0.0/bmkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-04-23 16:28:37.000000 bmkg-1.0.0/bmkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 16:28:36.000000 bmkg-1.0.0/bmkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-23 16:28:36.000000 bmkg-1.0.0/bmkg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-23 16:28:36.000000 bmkg-1.0.0/bmkg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1454 2023-04-23 16:21:41.000000 bmkg-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-23 16:28:37.392893 bmkg-1.0.0/setup.cfg
```

### Comparing `bmkg-0.1.1/LICENSE` & `bmkg-1.0.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 null
+Copyright (c) 2021-2023 null
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

