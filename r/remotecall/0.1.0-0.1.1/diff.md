# Comparing `tmp/remotecall-0.1.0.tar.gz` & `tmp/remotecall-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/remotecall-0.1.0.tar", last modified: Mon Mar 20 18:28:05 2023, max compression
+gzip compressed data, was "remotecall-0.1.1.tar", last modified: Sun Apr 23 19:32:17 2023, max compression
```

## Comparing `remotecall-0.1.0.tar` & `remotecall-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,36 @@
-drwxr-xr-x   0 slaine   (1355619077) 1965124760        0 2023-03-20 18:28:05.000000 remotecall-0.1.0/
--rw-r--r--   0 slaine   (1355619077) 1965124760      353 2023-03-20 18:28:05.000000 remotecall-0.1.0/PKG-INFO
--rw-r--r--   0 slaine   (1355619077) 1965124760     7640 2023-03-19 20:05:21.000000 remotecall-0.1.0/README.md
--rw-r--r--   0 slaine   (1355619077) 1965124760       38 2023-03-20 18:28:05.000000 remotecall-0.1.0/setup.cfg
--rw-r--r--   0 slaine   (1355619077) 1965124760      970 2023-03-20 17:55:00.000000 remotecall-0.1.0/setup.py
-drwxr-xr-x   0 slaine   (1355619077) 1965124760        0 2023-03-20 18:28:05.000000 remotecall-0.1.0/src/
-drwxr-xr-x   0 slaine   (1355619077) 1965124760        0 2023-03-20 18:28:05.000000 remotecall-0.1.0/src/remotecall/
--rw-r--r--   0 slaine   (1355619077) 1965124760     1042 2023-03-20 07:11:43.000000 remotecall-0.1.0/src/remotecall/__init__.py
--rw-r--r--   0 slaine   (1355619077) 1965124760     3018 2023-03-18 08:49:15.000000 remotecall-0.1.0/src/remotecall/__main__.py
--rw-r--r--   0 slaine   (1355619077) 1965124760      212 2023-03-20 17:57:48.000000 remotecall-0.1.0/src/remotecall/_meta.py
-drwxr-xr-x   0 slaine   (1355619077) 1965124760        0 2023-03-20 18:28:05.000000 remotecall-0.1.0/src/remotecall/authentication/
--rw-r--r--   0 slaine   (1355619077) 1965124760      768 2023-03-17 11:15:02.000000 remotecall-0.1.0/src/remotecall/authentication/__init__.py
--rw-r--r--   0 slaine   (1355619077) 1965124760     2369 2023-03-19 09:02:03.000000 remotecall-0.1.0/src/remotecall/authentication/authenticator.py
--rw-r--r--   0 slaine   (1355619077) 1965124760     3590 2023-03-20 09:01:04.000000 remotecall-0.1.0/src/remotecall/client.py
--rw-r--r--   0 slaine   (1355619077) 1965124760     4452 2023-03-18 08:30:48.000000 remotecall-0.1.0/src/remotecall/clientfactory.py
--rw-r--r--   0 slaine   (1355619077) 1965124760     5504 2023-03-11 14:36:05.000000 remotecall-0.1.0/src/remotecall/codecs.py
--rw-r--r--   0 slaine   (1355619077) 1965124760     2186 2023-03-18 08:50:36.000000 remotecall-0.1.0/src/remotecall/endpoint.py
--rw-r--r--   0 slaine   (1355619077) 1965124760      456 2023-03-16 18:22:04.000000 remotecall-0.1.0/src/remotecall/errors.py
--rw-r--r--   0 slaine   (1355619077) 1965124760      629 2023-03-20 07:34:11.000000 remotecall-0.1.0/src/remotecall/gethandler.py
--rw-r--r--   0 slaine   (1355619077) 1965124760     6170 2023-03-20 07:48:34.000000 remotecall-0.1.0/src/remotecall/posthandler.py
--rw-r--r--   0 slaine   (1355619077) 1965124760     4588 2023-03-20 07:48:46.000000 remotecall-0.1.0/src/remotecall/requesthandler.py
--rw-r--r--   0 slaine   (1355619077) 1965124760      626 2023-03-19 20:16:41.000000 remotecall-0.1.0/src/remotecall/response.py
--rw-r--r--   0 slaine   (1355619077) 1965124760     2720 2023-03-20 07:49:47.000000 remotecall-0.1.0/src/remotecall/server.py
-drwxr-xr-x   0 slaine   (1355619077) 1965124760        0 2023-03-20 18:28:05.000000 remotecall-0.1.0/src/remotecall.egg-info/
--rw-r--r--   0 slaine   (1355619077) 1965124760      353 2023-03-20 18:28:05.000000 remotecall-0.1.0/src/remotecall.egg-info/PKG-INFO
--rw-r--r--   0 slaine   (1355619077) 1965124760      730 2023-03-20 18:28:05.000000 remotecall-0.1.0/src/remotecall.egg-info/SOURCES.txt
--rw-r--r--   0 slaine   (1355619077) 1965124760        1 2023-03-20 18:28:05.000000 remotecall-0.1.0/src/remotecall.egg-info/dependency_links.txt
--rw-r--r--   0 slaine   (1355619077) 1965124760       50 2023-03-20 18:28:05.000000 remotecall-0.1.0/src/remotecall.egg-info/entry_points.txt
--rw-r--r--   0 slaine   (1355619077) 1965124760        1 2023-02-07 05:13:42.000000 remotecall-0.1.0/src/remotecall.egg-info/not-zip-safe
--rw-r--r--   0 slaine   (1355619077) 1965124760       32 2023-03-20 18:28:05.000000 remotecall-0.1.0/src/remotecall.egg-info/requires.txt
--rw-r--r--   0 slaine   (1355619077) 1965124760       11 2023-03-20 18:28:05.000000 remotecall-0.1.0/src/remotecall.egg-info/top_level.txt
+drwxr-xr-x   0 slaine   (1355619077) 1965124760        0 2023-04-23 19:32:17.333120 remotecall-0.1.1/
+-rw-r--r--   0 slaine   (1355619077) 1965124760     1481 2023-03-11 14:26:45.000000 remotecall-0.1.1/LICENSE
+-rw-r--r--   0 slaine   (1355619077) 1965124760      364 2023-04-23 19:32:17.332840 remotecall-0.1.1/PKG-INFO
+-rw-r--r--   0 slaine   (1355619077) 1965124760     7640 2023-03-19 20:05:21.000000 remotecall-0.1.1/README.md
+-rw-r--r--   0 slaine   (1355619077) 1965124760       38 2023-04-23 19:32:17.333249 remotecall-0.1.1/setup.cfg
+-rw-r--r--   0 slaine   (1355619077) 1965124760      970 2023-03-20 17:55:00.000000 remotecall-0.1.1/setup.py
+drwxr-xr-x   0 slaine   (1355619077) 1965124760        0 2023-04-23 19:32:17.302357 remotecall-0.1.1/src/
+drwxr-xr-x   0 slaine   (1355619077) 1965124760        0 2023-04-23 19:32:17.311326 remotecall-0.1.1/src/remotecall/
+-rw-r--r--   0 slaine   (1355619077) 1965124760     1042 2023-03-20 07:11:43.000000 remotecall-0.1.1/src/remotecall/__init__.py
+-rw-r--r--   0 slaine   (1355619077) 1965124760     3018 2023-03-18 08:49:15.000000 remotecall-0.1.1/src/remotecall/__main__.py
+-rw-r--r--   0 slaine   (1355619077) 1965124760      212 2023-04-20 11:52:34.000000 remotecall-0.1.1/src/remotecall/_meta.py
+drwxr-xr-x   0 slaine   (1355619077) 1965124760        0 2023-04-23 19:32:17.330771 remotecall-0.1.1/src/remotecall/authentication/
+-rw-r--r--   0 slaine   (1355619077) 1965124760      768 2023-03-17 11:15:02.000000 remotecall-0.1.1/src/remotecall/authentication/__init__.py
+-rw-r--r--   0 slaine   (1355619077) 1965124760     2369 2023-03-19 09:02:03.000000 remotecall-0.1.1/src/remotecall/authentication/authenticator.py
+-rw-r--r--   0 slaine   (1355619077) 1965124760     3590 2023-03-20 09:01:04.000000 remotecall-0.1.1/src/remotecall/client.py
+-rw-r--r--   0 slaine   (1355619077) 1965124760     4452 2023-03-18 08:30:48.000000 remotecall-0.1.1/src/remotecall/clientfactory.py
+-rw-r--r--   0 slaine   (1355619077) 1965124760     5504 2023-03-11 14:36:05.000000 remotecall-0.1.1/src/remotecall/codecs.py
+drwxr-xr-x   0 slaine   (1355619077) 1965124760        0 2023-04-23 19:32:17.332365 remotecall-0.1.1/src/remotecall/constants/
+-rw-r--r--   0 slaine   (1355619077) 1965124760        0 2023-04-20 11:46:26.000000 remotecall-0.1.1/src/remotecall/constants/__init__.py
+-rw-r--r--   0 slaine   (1355619077) 1965124760      174 2023-04-20 11:38:21.000000 remotecall-0.1.1/src/remotecall/constants/headers.py
+-rw-r--r--   0 slaine   (1355619077) 1965124760      204 2023-03-19 20:17:29.000000 remotecall-0.1.1/src/remotecall/constants/statuscodes.py
+-rw-r--r--   0 slaine   (1355619077) 1965124760     2186 2023-03-18 08:50:36.000000 remotecall-0.1.1/src/remotecall/endpoint.py
+-rw-r--r--   0 slaine   (1355619077) 1965124760      456 2023-03-16 18:22:04.000000 remotecall-0.1.1/src/remotecall/errors.py
+-rw-r--r--   0 slaine   (1355619077) 1965124760      629 2023-03-20 07:34:11.000000 remotecall-0.1.1/src/remotecall/gethandler.py
+-rw-r--r--   0 slaine   (1355619077) 1965124760     6170 2023-03-20 07:48:34.000000 remotecall-0.1.1/src/remotecall/posthandler.py
+-rw-r--r--   0 slaine   (1355619077) 1965124760     4588 2023-03-20 07:48:46.000000 remotecall-0.1.1/src/remotecall/requesthandler.py
+-rw-r--r--   0 slaine   (1355619077) 1965124760      626 2023-03-19 20:16:41.000000 remotecall-0.1.1/src/remotecall/response.py
+-rw-r--r--   0 slaine   (1355619077) 1965124760     2720 2023-03-20 07:49:47.000000 remotecall-0.1.1/src/remotecall/server.py
+drwxr-xr-x   0 slaine   (1355619077) 1965124760        0 2023-04-23 19:32:17.316234 remotecall-0.1.1/src/remotecall.egg-info/
+-rw-r--r--   0 slaine   (1355619077) 1965124760      364 2023-04-23 19:32:17.000000 remotecall-0.1.1/src/remotecall.egg-info/PKG-INFO
+-rw-r--r--   0 slaine   (1355619077) 1965124760      851 2023-04-23 19:32:17.000000 remotecall-0.1.1/src/remotecall.egg-info/SOURCES.txt
+-rw-r--r--   0 slaine   (1355619077) 1965124760        1 2023-04-23 19:32:17.000000 remotecall-0.1.1/src/remotecall.egg-info/dependency_links.txt
+-rw-r--r--   0 slaine   (1355619077) 1965124760       50 2023-04-23 19:32:17.000000 remotecall-0.1.1/src/remotecall.egg-info/entry_points.txt
+-rw-r--r--   0 slaine   (1355619077) 1965124760        1 2023-02-07 05:13:42.000000 remotecall-0.1.1/src/remotecall.egg-info/not-zip-safe
+-rw-r--r--   0 slaine   (1355619077) 1965124760       32 2023-04-23 19:32:17.000000 remotecall-0.1.1/src/remotecall.egg-info/requires.txt
+-rw-r--r--   0 slaine   (1355619077) 1965124760       11 2023-04-23 19:32:17.000000 remotecall-0.1.1/src/remotecall.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `remotecall-0.1.0/README.md` & `remotecall-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.0/setup.py` & `remotecall-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.0/src/remotecall/__init__.py` & `remotecall-0.1.1/src/remotecall/__init__.py`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.0/src/remotecall/__main__.py` & `remotecall-0.1.1/src/remotecall/__main__.py`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.0/src/remotecall/authentication/__init__.py` & `remotecall-0.1.1/src/remotecall/authentication/__init__.py`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.0/src/remotecall/authentication/authenticator.py` & `remotecall-0.1.1/src/remotecall/authentication/authenticator.py`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.0/src/remotecall/client.py` & `remotecall-0.1.1/src/remotecall/client.py`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.0/src/remotecall/clientfactory.py` & `remotecall-0.1.1/src/remotecall/clientfactory.py`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.0/src/remotecall/codecs.py` & `remotecall-0.1.1/src/remotecall/codecs.py`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.0/src/remotecall/endpoint.py` & `remotecall-0.1.1/src/remotecall/endpoint.py`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.0/src/remotecall/gethandler.py` & `remotecall-0.1.1/src/remotecall/gethandler.py`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.0/src/remotecall/posthandler.py` & `remotecall-0.1.1/src/remotecall/posthandler.py`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.0/src/remotecall/requesthandler.py` & `remotecall-0.1.1/src/remotecall/requesthandler.py`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.0/src/remotecall/response.py` & `remotecall-0.1.1/src/remotecall/response.py`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.0/src/remotecall/server.py` & `remotecall-0.1.1/src/remotecall/server.py`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.0/src/remotecall.egg-info/SOURCES.txt` & `remotecall-0.1.1/src/remotecall.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 src/remotecall/__init__.py
 src/remotecall/__main__.py
 src/remotecall/_meta.py
 src/remotecall/client.py
 src/remotecall/clientfactory.py
@@ -17,8 +18,11 @@
 src/remotecall.egg-info/SOURCES.txt
 src/remotecall.egg-info/dependency_links.txt
 src/remotecall.egg-info/entry_points.txt
 src/remotecall.egg-info/not-zip-safe
 src/remotecall.egg-info/requires.txt
 src/remotecall.egg-info/top_level.txt
 src/remotecall/authentication/__init__.py
-src/remotecall/authentication/authenticator.py
+src/remotecall/authentication/authenticator.py
+src/remotecall/constants/__init__.py
+src/remotecall/constants/headers.py
+src/remotecall/constants/statuscodes.py
```

