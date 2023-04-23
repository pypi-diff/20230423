# Comparing `tmp/kuki-0.0.1.tar.gz` & `tmp/kuki-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuki-0.0.1.tar", last modified: Sun Apr 23 13:40:46 2023, max compression
+gzip compressed data, was "kuki-0.0.2.tar", last modified: Sun Apr 23 13:46:43 2023, max compression
```

## Comparing `kuki-0.0.1.tar` & `kuki-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-04-23 13:40:46.947236 kuki-0.0.1/
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      182 2023-04-23 13:40:46.947236 kuki-0.0.1/PKG-INFO
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      997 2023-04-23 13:21:01.000000 kuki-0.0.1/README.md
-drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-04-23 13:40:46.946236 kuki-0.0.1/kuki/
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-04-06 13:33:17.000000 kuki-0.0.1/kuki/__init__.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      793 2023-04-23 12:18:00.000000 kuki-0.0.1/kuki/config_api.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       21 2023-04-16 07:55:05.000000 kuki-0.0.1/kuki/krun.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     2596 2023-04-23 13:21:05.000000 kuki-0.0.1/kuki/kuki.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1911 2023-04-23 13:27:53.000000 kuki-0.0.1/kuki/kukijson.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     2235 2023-04-23 12:19:44.000000 kuki-0.0.1/kuki/registry_api.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       22 2023-04-23 09:44:31.000000 kuki-0.0.1/kuki/version.py
-drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-04-23 13:40:46.947236 kuki-0.0.1/kuki.egg-info/
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      182 2023-04-23 13:40:46.000000 kuki-0.0.1/kuki.egg-info/PKG-INFO
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      341 2023-04-23 13:40:46.000000 kuki-0.0.1/kuki.egg-info/SOURCES.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        1 2023-04-23 13:40:46.000000 kuki-0.0.1/kuki.egg-info/dependency_links.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       62 2023-04-23 13:40:46.000000 kuki-0.0.1/kuki.egg-info/entry_points.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        1 2023-04-23 13:30:11.000000 kuki-0.0.1/kuki.egg-info/not-zip-safe
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       17 2023-04-23 13:40:46.000000 kuki-0.0.1/kuki.egg-info/requires.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        5 2023-04-23 13:40:46.000000 kuki-0.0.1/kuki.egg-info/top_level.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      388 2023-04-23 13:40:46.947236 kuki-0.0.1/setup.cfg
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      280 2023-04-23 09:47:47.000000 kuki-0.0.1/setup.py
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-04-23 13:46:43.316654 kuki-0.0.2/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1178 2023-04-23 13:46:43.316654 kuki-0.0.2/PKG-INFO
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      997 2023-04-23 13:21:01.000000 kuki-0.0.2/README.md
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-04-23 13:46:43.315654 kuki-0.0.2/kuki/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-04-06 13:33:17.000000 kuki-0.0.2/kuki/__init__.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      793 2023-04-23 12:18:00.000000 kuki-0.0.2/kuki/config_api.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       21 2023-04-16 07:55:05.000000 kuki-0.0.2/kuki/krun.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     2596 2023-04-23 13:21:05.000000 kuki-0.0.2/kuki/kuki.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1911 2023-04-23 13:27:53.000000 kuki-0.0.2/kuki/kukijson.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     2235 2023-04-23 12:19:44.000000 kuki-0.0.2/kuki/registry_api.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       22 2023-04-23 13:43:39.000000 kuki-0.0.2/kuki/version.py
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-04-23 13:46:43.316654 kuki-0.0.2/kuki.egg-info/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1178 2023-04-23 13:46:43.000000 kuki-0.0.2/kuki.egg-info/PKG-INFO
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      341 2023-04-23 13:46:43.000000 kuki-0.0.2/kuki.egg-info/SOURCES.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        1 2023-04-23 13:46:43.000000 kuki-0.0.2/kuki.egg-info/dependency_links.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       62 2023-04-23 13:46:43.000000 kuki-0.0.2/kuki.egg-info/entry_points.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        1 2023-04-23 13:46:43.000000 kuki-0.0.2/kuki.egg-info/not-zip-safe
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       17 2023-04-23 13:46:43.000000 kuki-0.0.2/kuki.egg-info/requires.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        5 2023-04-23 13:46:43.000000 kuki-0.0.2/kuki.egg-info/top_level.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      421 2023-04-23 13:46:43.317654 kuki-0.0.2/setup.cfg
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      280 2023-04-23 09:47:47.000000 kuki-0.0.2/setup.py
```

### Comparing `kuki-0.0.1/README.md` & `kuki-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `kuki-0.0.1/kuki/config_api.py` & `kuki-0.0.2/kuki/config_api.py`

 * *Files identical despite different names*

### Comparing `kuki-0.0.1/kuki/kuki.py` & `kuki-0.0.2/kuki/kuki.py`

 * *Files identical despite different names*

### Comparing `kuki-0.0.1/kuki/kukijson.py` & `kuki-0.0.2/kuki/kukijson.py`

 * *Files identical despite different names*

### Comparing `kuki-0.0.1/kuki/registry_api.py` & `kuki-0.0.2/kuki/registry_api.py`

 * *Files identical despite different names*

