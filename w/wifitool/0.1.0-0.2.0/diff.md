# Comparing `tmp/wifitool-0.1.0.tar.gz` & `tmp/wifitool-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wifitool-0.1.0.tar", last modified: Sun Apr 23 21:26:11 2023, max compression
+gzip compressed data, was "wifitool-0.2.0.tar", last modified: Sun Apr 23 21:46:38 2023, max compression
```

## Comparing `wifitool-0.1.0.tar` & `wifitool-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 21:26:11.954540 wifitool-0.1.0/
--rw-rw-rw-   0        0        0      694 2023-04-23 21:26:11.953543 wifitool-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        4 2023-04-08 22:06:19.000000 wifitool-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-23 21:26:11.954540 wifitool-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     8884 2023-04-23 21:21:53.000000 wifitool-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-23 21:26:11.942541 wifitool-0.1.0/wifitool/
--rw-rw-rw-   0        0        0     7202 2023-04-23 21:24:28.000000 wifitool-0.1.0/wifitool/__init__.py
--rw-rw-rw-   0        0        0      261 2023-04-23 21:23:19.000000 wifitool-0.1.0/wifitool/multiplication.py
-drwxrwxrwx   0        0        0        0 2023-04-23 21:26:11.951543 wifitool-0.1.0/wifitool.egg-info/
--rw-rw-rw-   0        0        0      694 2023-04-23 21:26:11.000000 wifitool-0.1.0/wifitool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-04-23 21:26:11.000000 wifitool-0.1.0/wifitool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 21:26:11.000000 wifitool-0.1.0/wifitool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-23 21:26:11.000000 wifitool-0.1.0/wifitool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-23 21:26:11.000000 wifitool-0.1.0/wifitool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 21:46:38.526901 wifitool-0.2.0/
+-rw-rw-rw-   0        0        0      694 2023-04-23 21:46:38.525901 wifitool-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0        4 2023-04-08 22:06:19.000000 wifitool-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-23 21:46:38.527900 wifitool-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1380 2023-04-23 21:46:36.000000 wifitool-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 21:46:38.487901 wifitool-0.2.0/wifitool/
+-rw-rw-rw-   0        0        0     7202 2023-04-23 21:24:28.000000 wifitool-0.2.0/wifitool/__init__.py
+-rw-rw-rw-   0        0        0      261 2023-04-23 21:23:19.000000 wifitool-0.2.0/wifitool/multiplication.py
+drwxrwxrwx   0        0        0        0 2023-04-23 21:46:38.523901 wifitool-0.2.0/wifitool.egg-info/
+-rw-rw-rw-   0        0        0      694 2023-04-23 21:46:38.000000 wifitool-0.2.0/wifitool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-04-23 21:46:38.000000 wifitool-0.2.0/wifitool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 21:46:38.000000 wifitool-0.2.0/wifitool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-23 21:46:38.000000 wifitool-0.2.0/wifitool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-23 21:46:38.000000 wifitool-0.2.0/wifitool.egg-info/top_level.txt
```

### Comparing `wifitool-0.1.0/PKG-INFO` & `wifitool-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wifitool
-Version: 0.1.0
+Version: 0.2.0
 Summary: Demo library
 Home-page: https://medium-multiply.readthedocs.io/
 Author: Joffrey Bienvenu
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wifitool-0.1.0/wifitool/__init__.py` & `wifitool-0.2.0/wifitool/__init__.py`

 * *Files identical despite different names*

### Comparing `wifitool-0.1.0/wifitool.egg-info/PKG-INFO` & `wifitool-0.2.0/wifitool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wifitool
-Version: 0.1.0
+Version: 0.2.0
 Summary: Demo library
 Home-page: https://medium-multiply.readthedocs.io/
 Author: Joffrey Bienvenu
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

