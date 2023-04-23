# Comparing `tmp/gym-trading-env-0.1.8.tar.gz` & `tmp/gym-trading-env-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym-trading-env-0.1.8.tar", last modified: Thu Apr 13 12:54:04 2023, max compression
+gzip compressed data, was "gym-trading-env-0.1.9.tar", last modified: Thu Apr 13 13:25:37 2023, max compression
```

## Comparing `gym-trading-env-0.1.8.tar` & `gym-trading-env-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 12:54:04.435812 gym-trading-env-0.1.8/
--rw-rw-rw-   0        0        0     1088 2023-03-29 17:01:42.000000 gym-trading-env-0.1.8/LICENSE.txt
--rw-rw-rw-   0        0        0    14258 2023-04-13 12:54:04.434810 gym-trading-env-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0    12396 2023-04-13 12:39:12.000000 gym-trading-env-0.1.8/README.md
--rw-rw-rw-   0        0        0      870 2023-04-13 12:52:15.000000 gym-trading-env-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 12:54:04.436807 gym-trading-env-0.1.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-13 12:54:04.345824 gym-trading-env-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2023-04-13 12:54:04.367811 gym-trading-env-0.1.8/src/gym_trading_env/
--rw-rw-rw-   0        0        0      267 2023-04-13 10:54:15.000000 gym-trading-env-0.1.8/src/gym_trading_env/__init__.py
--rw-rw-rw-   0        0        0     4164 2023-04-13 12:39:12.000000 gym-trading-env-0.1.8/src/gym_trading_env/downloader.py
--rw-rw-rw-   0        0        0     8871 2023-04-13 11:58:15.000000 gym-trading-env-0.1.8/src/gym_trading_env/environments.py
--rw-rw-rw-   0        0        0     2502 2023-04-10 08:13:00.000000 gym-trading-env-0.1.8/src/gym_trading_env/renderer.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:54:04.431806 gym-trading-env-0.1.8/src/gym_trading_env/utils/
--rw-rw-rw-   0        0        0        0 2023-04-10 08:13:00.000000 gym-trading-env-0.1.8/src/gym_trading_env/utils/__init__.py
--rw-rw-rw-   0        0        0    14334 2023-04-10 08:13:00.000000 gym-trading-env-0.1.8/src/gym_trading_env/utils/charts.py
--rw-rw-rw-   0        0        0     3333 2023-04-13 09:31:51.000000 gym-trading-env-0.1.8/src/gym_trading_env/utils/history.py
--rw-rw-rw-   0        0        0     3036 2023-04-10 08:13:00.000000 gym-trading-env-0.1.8/src/gym_trading_env/utils/portfolio.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:54:04.420809 gym-trading-env-0.1.8/src/gym_trading_env.egg-info/
--rw-rw-rw-   0        0        0    14258 2023-04-13 12:54:04.000000 gym-trading-env-0.1.8/src/gym_trading_env.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      534 2023-04-13 12:54:04.000000 gym-trading-env-0.1.8/src/gym_trading_env.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 12:54:04.000000 gym-trading-env-0.1.8/src/gym_trading_env.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2023-04-13 12:54:04.000000 gym-trading-env-0.1.8/src/gym_trading_env.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-13 12:54:04.000000 gym-trading-env-0.1.8/src/gym_trading_env.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 13:25:37.237704 gym-trading-env-0.1.9/
+-rw-rw-rw-   0        0        0     1088 2023-03-29 17:01:42.000000 gym-trading-env-0.1.9/LICENSE.txt
+-rw-rw-rw-   0        0        0    14258 2023-04-13 13:25:37.235704 gym-trading-env-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    12396 2023-04-13 12:39:12.000000 gym-trading-env-0.1.9/README.md
+-rw-rw-rw-   0        0        0      870 2023-04-13 13:24:57.000000 gym-trading-env-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 13:25:37.237704 gym-trading-env-0.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 13:25:37.153704 gym-trading-env-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2023-04-13 13:25:37.176704 gym-trading-env-0.1.9/src/gym_trading_env/
+-rw-rw-rw-   0        0        0      333 2023-04-13 13:15:17.000000 gym-trading-env-0.1.9/src/gym_trading_env/__init__.py
+-rw-rw-rw-   0        0        0     4164 2023-04-13 12:39:12.000000 gym-trading-env-0.1.9/src/gym_trading_env/downloader.py
+-rw-rw-rw-   0        0        0     8871 2023-04-13 11:58:15.000000 gym-trading-env-0.1.9/src/gym_trading_env/environments.py
+-rw-rw-rw-   0        0        0     2502 2023-04-10 08:13:00.000000 gym-trading-env-0.1.9/src/gym_trading_env/renderer.py
+drwxrwxrwx   0        0        0        0 2023-04-13 13:25:37.231705 gym-trading-env-0.1.9/src/gym_trading_env/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-10 08:13:00.000000 gym-trading-env-0.1.9/src/gym_trading_env/utils/__init__.py
+-rw-rw-rw-   0        0        0    14334 2023-04-10 08:13:00.000000 gym-trading-env-0.1.9/src/gym_trading_env/utils/charts.py
+-rw-rw-rw-   0        0        0     3333 2023-04-13 09:31:51.000000 gym-trading-env-0.1.9/src/gym_trading_env/utils/history.py
+-rw-rw-rw-   0        0        0     3036 2023-04-10 08:13:00.000000 gym-trading-env-0.1.9/src/gym_trading_env/utils/portfolio.py
+drwxrwxrwx   0        0        0        0 2023-04-13 13:25:37.219705 gym-trading-env-0.1.9/src/gym_trading_env.egg-info/
+-rw-rw-rw-   0        0        0    14258 2023-04-13 13:25:37.000000 gym-trading-env-0.1.9/src/gym_trading_env.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      534 2023-04-13 13:25:37.000000 gym-trading-env-0.1.9/src/gym_trading_env.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 13:25:37.000000 gym-trading-env-0.1.9/src/gym_trading_env.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-04-13 13:25:37.000000 gym-trading-env-0.1.9/src/gym_trading_env.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-13 13:25:37.000000 gym-trading-env-0.1.9/src/gym_trading_env.egg-info/top_level.txt
```

### Comparing `gym-trading-env-0.1.8/LICENSE.txt` & `gym-trading-env-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.8/PKG-INFO` & `gym-trading-env-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-trading-env
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple, easy, customizable Open IA Gym environments for trading.
 Author-email: Clement Perroud <clement.perroud.pro@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `gym-trading-env-0.1.8/README.md` & `gym-trading-env-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.8/pyproject.toml` & `gym-trading-env-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gym-trading-env"
-version = "0.1.8"
+version = "0.1.9"
 license = {file = "LICENSE.txt"}
 authors = [
   { name="Clement Perroud", email="clement.perroud.pro@gmail.com" },
 ]
 description = "A simple, easy, customizable Open IA Gym environments for trading."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `gym-trading-env-0.1.8/src/gym_trading_env/downloader.py` & `gym-trading-env-0.1.9/src/gym_trading_env/downloader.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.8/src/gym_trading_env/environments.py` & `gym-trading-env-0.1.9/src/gym_trading_env/environments.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.8/src/gym_trading_env/renderer.py` & `gym-trading-env-0.1.9/src/gym_trading_env/renderer.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.8/src/gym_trading_env/utils/charts.py` & `gym-trading-env-0.1.9/src/gym_trading_env/utils/charts.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.8/src/gym_trading_env/utils/history.py` & `gym-trading-env-0.1.9/src/gym_trading_env/utils/history.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.8/src/gym_trading_env/utils/portfolio.py` & `gym-trading-env-0.1.9/src/gym_trading_env/utils/portfolio.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.8/src/gym_trading_env.egg-info/PKG-INFO` & `gym-trading-env-0.1.9/src/gym_trading_env.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-trading-env
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple, easy, customizable Open IA Gym environments for trading.
 Author-email: Clement Perroud <clement.perroud.pro@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `gym-trading-env-0.1.8/src/gym_trading_env.egg-info/SOURCES.txt` & `gym-trading-env-0.1.9/src/gym_trading_env.egg-info/SOURCES.txt`

 * *Files identical despite different names*

