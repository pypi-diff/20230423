# Comparing `tmp/napari-zulip-0.0.1.tar.gz` & `tmp/napari-zulip-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-zulip-0.0.1.tar", last modified: Sat Apr 22 21:50:50 2023, max compression
+gzip compressed data, was "napari-zulip-0.0.2.tar", last modified: Sat Apr 22 23:02:07 2023, max compression
```

## Comparing `napari-zulip-0.0.1.tar` & `napari-zulip-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kharrington   (503) staff       (20)        0 2023-04-22 21:50:50.902270 napari-zulip-0.0.1/
--rw-r--r--   0 kharrington   (503) staff       (20)     1491 2023-04-22 13:45:53.000000 napari-zulip-0.0.1/LICENSE
--rw-r--r--   0 kharrington   (503) staff       (20)       96 2023-04-22 13:45:53.000000 napari-zulip-0.0.1/MANIFEST.in
--rw-r--r--   0 kharrington   (503) staff       (20)     4454 2023-04-22 21:50:50.902333 napari-zulip-0.0.1/PKG-INFO
--rw-r--r--   0 kharrington   (503) staff       (20)     3264 2023-04-22 21:12:27.000000 napari-zulip-0.0.1/README.md
--rw-r--r--   0 kharrington   (503) staff       (20)     1177 2023-04-22 13:45:53.000000 napari-zulip-0.0.1/pyproject.toml
--rw-r--r--   0 kharrington   (503) staff       (20)     1650 2023-04-22 21:50:50.902675 napari-zulip-0.0.1/setup.cfg
-drwxr-xr-x   0 kharrington   (503) staff       (20)        0 2023-04-22 21:50:50.899339 napari-zulip-0.0.1/src/
-drwxr-xr-x   0 kharrington   (503) staff       (20)        0 2023-04-22 21:50:50.900925 napari-zulip-0.0.1/src/napari_zulip/
--rw-r--r--   0 kharrington   (503) staff       (20)      105 2023-04-22 13:58:03.000000 napari-zulip-0.0.1/src/napari_zulip/__init__.py
-drwxr-xr-x   0 kharrington   (503) staff       (20)        0 2023-04-22 21:50:50.902148 napari-zulip-0.0.1/src/napari_zulip/_tests/
--rw-r--r--   0 kharrington   (503) staff       (20)        0 2023-04-22 13:45:53.000000 napari-zulip-0.0.1/src/napari_zulip/_tests/__init__.py
--rw-r--r--   0 kharrington   (503) staff       (20)      325 2023-04-22 21:41:18.000000 napari-zulip-0.0.1/src/napari_zulip/_tests/test_widget.py
--rw-r--r--   0 kharrington   (503) staff       (20)     1751 2023-04-22 21:31:58.000000 napari-zulip-0.0.1/src/napari_zulip/_widget.py
--rw-r--r--   0 kharrington   (503) staff       (20)      342 2023-04-22 13:56:06.000000 napari-zulip-0.0.1/src/napari_zulip/napari.yaml
-drwxr-xr-x   0 kharrington   (503) staff       (20)        0 2023-04-22 21:50:50.901884 napari-zulip-0.0.1/src/napari_zulip.egg-info/
--rw-r--r--   0 kharrington   (503) staff       (20)     4454 2023-04-22 21:50:50.000000 napari-zulip-0.0.1/src/napari_zulip.egg-info/PKG-INFO
--rw-r--r--   0 kharrington   (503) staff       (20)      457 2023-04-22 21:50:50.000000 napari-zulip-0.0.1/src/napari_zulip.egg-info/SOURCES.txt
--rw-r--r--   0 kharrington   (503) staff       (20)        1 2023-04-22 21:50:50.000000 napari-zulip-0.0.1/src/napari_zulip.egg-info/dependency_links.txt
--rw-r--r--   0 kharrington   (503) staff       (20)       58 2023-04-22 21:50:50.000000 napari-zulip-0.0.1/src/napari_zulip.egg-info/entry_points.txt
--rw-r--r--   0 kharrington   (503) staff       (20)       82 2023-04-22 21:50:50.000000 napari-zulip-0.0.1/src/napari_zulip.egg-info/requires.txt
--rw-r--r--   0 kharrington   (503) staff       (20)       13 2023-04-22 21:50:50.000000 napari-zulip-0.0.1/src/napari_zulip.egg-info/top_level.txt
+drwxr-xr-x   0 kharrington   (503) staff       (20)        0 2023-04-22 23:02:07.563813 napari-zulip-0.0.2/
+-rw-r--r--   0 kharrington   (503) staff       (20)     1491 2023-04-22 13:45:53.000000 napari-zulip-0.0.2/LICENSE
+-rw-r--r--   0 kharrington   (503) staff       (20)       96 2023-04-22 13:45:53.000000 napari-zulip-0.0.2/MANIFEST.in
+-rw-r--r--   0 kharrington   (503) staff       (20)     4453 2023-04-22 23:02:07.563880 napari-zulip-0.0.2/PKG-INFO
+-rw-r--r--   0 kharrington   (503) staff       (20)     3264 2023-04-22 21:12:27.000000 napari-zulip-0.0.2/README.md
+-rw-r--r--   0 kharrington   (503) staff       (20)     1177 2023-04-22 13:45:53.000000 napari-zulip-0.0.2/pyproject.toml
+-rw-r--r--   0 kharrington   (503) staff       (20)     1649 2023-04-22 23:02:07.564347 napari-zulip-0.0.2/setup.cfg
+drwxr-xr-x   0 kharrington   (503) staff       (20)        0 2023-04-22 23:02:07.560912 napari-zulip-0.0.2/src/
+drwxr-xr-x   0 kharrington   (503) staff       (20)        0 2023-04-22 23:02:07.562569 napari-zulip-0.0.2/src/napari_zulip/
+-rw-r--r--   0 kharrington   (503) staff       (20)      105 2023-04-22 23:01:26.000000 napari-zulip-0.0.2/src/napari_zulip/__init__.py
+drwxr-xr-x   0 kharrington   (503) staff       (20)        0 2023-04-22 23:02:07.563691 napari-zulip-0.0.2/src/napari_zulip/_tests/
+-rw-r--r--   0 kharrington   (503) staff       (20)        0 2023-04-22 13:45:53.000000 napari-zulip-0.0.2/src/napari_zulip/_tests/__init__.py
+-rw-r--r--   0 kharrington   (503) staff       (20)      325 2023-04-22 21:41:18.000000 napari-zulip-0.0.2/src/napari_zulip/_tests/test_widget.py
+-rw-r--r--   0 kharrington   (503) staff       (20)     1751 2023-04-22 21:31:58.000000 napari-zulip-0.0.2/src/napari_zulip/_widget.py
+-rw-r--r--   0 kharrington   (503) staff       (20)      342 2023-04-22 13:56:06.000000 napari-zulip-0.0.2/src/napari_zulip/napari.yaml
+drwxr-xr-x   0 kharrington   (503) staff       (20)        0 2023-04-22 23:02:07.563434 napari-zulip-0.0.2/src/napari_zulip.egg-info/
+-rw-r--r--   0 kharrington   (503) staff       (20)     4453 2023-04-22 23:02:07.000000 napari-zulip-0.0.2/src/napari_zulip.egg-info/PKG-INFO
+-rw-r--r--   0 kharrington   (503) staff       (20)      457 2023-04-22 23:02:07.000000 napari-zulip-0.0.2/src/napari_zulip.egg-info/SOURCES.txt
+-rw-r--r--   0 kharrington   (503) staff       (20)        1 2023-04-22 23:02:07.000000 napari-zulip-0.0.2/src/napari_zulip.egg-info/dependency_links.txt
+-rw-r--r--   0 kharrington   (503) staff       (20)       58 2023-04-22 23:02:07.000000 napari-zulip-0.0.2/src/napari_zulip.egg-info/entry_points.txt
+-rw-r--r--   0 kharrington   (503) staff       (20)       82 2023-04-22 23:02:07.000000 napari-zulip-0.0.2/src/napari_zulip.egg-info/requires.txt
+-rw-r--r--   0 kharrington   (503) staff       (20)       13 2023-04-22 23:02:07.000000 napari-zulip-0.0.2/src/napari_zulip.egg-info/top_level.txt
```

### Comparing `napari-zulip-0.0.1/LICENSE` & `napari-zulip-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-zulip-0.0.1/PKG-INFO` & `napari-zulip-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: napari-zulip
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple plugin for interacting with Zulip from napari
 Home-page: https://github.com/kephale/napari-zulip
-Author: jKyle Harrington
+Author: Kyle Harrington
 Author-email: czi@kyleharrington.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/kephale/napari-zulip/issues
 Project-URL: Documentation, https://github.com/kephale/napari-zulip#README.md
 Project-URL: Source Code, https://github.com/kephale/napari-zulip
 Project-URL: User Support, https://github.com/kephale/napari-zulip/issues
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `napari-zulip-0.0.1/README.md` & `napari-zulip-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `napari-zulip-0.0.1/pyproject.toml` & `napari-zulip-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari-zulip-0.0.1/setup.cfg` & `napari-zulip-0.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [metadata]
 name = napari-zulip
 version = attr: napari_zulip.__version__
 description = A simple plugin for interacting with Zulip from napari
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/kephale/napari-zulip
-author = jKyle Harrington
+author = Kyle Harrington
 author_email = czi@kyleharrington.com
 license = BSD-3-Clause
 license_files = LICENSE
 classifiers = 
 	Development Status :: 2 - Pre-Alpha
 	Framework :: napari
 	Intended Audience :: Developers
```

### Comparing `napari-zulip-0.0.1/src/napari_zulip/_widget.py` & `napari-zulip-0.0.2/src/napari_zulip/_widget.py`

 * *Files identical despite different names*

### Comparing `napari-zulip-0.0.1/src/napari_zulip.egg-info/PKG-INFO` & `napari-zulip-0.0.2/src/napari_zulip.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: napari-zulip
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple plugin for interacting with Zulip from napari
 Home-page: https://github.com/kephale/napari-zulip
-Author: jKyle Harrington
+Author: Kyle Harrington
 Author-email: czi@kyleharrington.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/kephale/napari-zulip/issues
 Project-URL: Documentation, https://github.com/kephale/napari-zulip#README.md
 Project-URL: Source Code, https://github.com/kephale/napari-zulip
 Project-URL: User Support, https://github.com/kephale/napari-zulip/issues
 Classifier: Development Status :: 2 - Pre-Alpha
```

