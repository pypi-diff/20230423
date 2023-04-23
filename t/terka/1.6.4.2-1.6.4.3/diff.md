# Comparing `tmp/terka-1.6.4.2.tar.gz` & `tmp/terka-1.6.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terka-1.6.4.2.tar", last modified: Sun Apr 23 14:15:55 2023, max compression
+gzip compressed data, was "terka-1.6.4.3.tar", last modified: Sun Apr 23 14:21:06 2023, max compression
```

## Comparing `terka-1.6.4.2.tar` & `terka-1.6.4.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 14:15:55.686387 terka-1.6.4.2/
--rw-r--r--   0 am        (1000) am        (1000)     1212 2023-04-23 14:15:55.686387 terka-1.6.4.2/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)       38 2023-04-23 14:15:55.686387 terka-1.6.4.2/setup.cfg
--rw-r--r--   0 am        (1000) am        (1000)      895 2023-04-23 14:15:43.000000 terka-1.6.4.2/setup.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 14:15:55.682387 terka-1.6.4.2/terka/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-23 14:06:23.000000 terka-1.6.4.2/terka/__init__.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 14:15:55.682387 terka-1.6.4.2/terka/adapters/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.2/terka/adapters/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    16083 2023-04-23 14:14:21.000000 terka-1.6.4.2/terka/adapters/orm.py
--rw-r--r--   0 am        (1000) am        (1000)     6150 2023-04-23 14:10:47.000000 terka-1.6.4.2/terka/adapters/repository.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 14:15:55.686387 terka-1.6.4.2/terka/domain/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.2/terka/domain/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-06 18:49:11.000000 terka-1.6.4.2/terka/domain/collaborators.py
--rw-r--r--   0 am        (1000) am        (1000)    41005 2023-04-23 14:11:14.000000 terka-1.6.4.2/terka/domain/commands.py
--rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-12 20:16:29.000000 terka-1.6.4.2/terka/domain/commentary.py
--rw-r--r--   0 am        (1000) am        (1000)      102 2023-01-26 19:46:39.000000 terka-1.6.4.2/terka/domain/element.py
--rw-r--r--   0 am        (1000) am        (1000)      961 2023-04-23 14:11:41.000000 terka-1.6.4.2/terka/domain/epic.py
--rw-r--r--   0 am        (1000) am        (1000)     1440 2023-03-12 20:44:34.000000 terka-1.6.4.2/terka/domain/event_history.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 14:15:55.686387 terka-1.6.4.2/terka/domain/external_connectors/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-23 13:50:48.000000 terka-1.6.4.2/terka/domain/external_connectors/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      187 2023-04-23 13:40:28.000000 terka-1.6.4.2/terka/domain/external_connectors/asana.py
--rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.6.4.2/terka/domain/helpers.py
--rw-r--r--   0 am        (1000) am        (1000)      892 2023-03-17 11:37:47.000000 terka-1.6.4.2/terka/domain/project.py
--rw-r--r--   0 am        (1000) am        (1000)     2167 2023-04-23 14:12:42.000000 terka-1.6.4.2/terka/domain/sprint.py
--rw-r--r--   0 am        (1000) am        (1000)      955 2023-04-23 14:12:46.000000 terka-1.6.4.2/terka/domain/story.py
--rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-06 19:04:21.000000 terka-1.6.4.2/terka/domain/tag.py
--rw-r--r--   0 am        (1000) am        (1000)     2039 2023-04-07 19:10:02.000000 terka-1.6.4.2/terka/domain/task.py
--rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-08 10:39:03.000000 terka-1.6.4.2/terka/domain/time_tracker.py
--rw-r--r--   0 am        (1000) am        (1000)      338 2023-04-23 14:13:11.000000 terka-1.6.4.2/terka/domain/user.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 14:15:55.686387 terka-1.6.4.2/terka/entrypoints/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-02-11 17:56:56.000000 terka-1.6.4.2/terka/entrypoints/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)     5079 2023-04-23 14:13:55.000000 terka-1.6.4.2/terka/entrypoints/cli.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 14:15:55.686387 terka-1.6.4.2/terka/service_layer/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.2/terka/service_layer/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    27276 2023-04-23 14:14:50.000000 terka-1.6.4.2/terka/service_layer/printer.py
--rw-r--r--   0 am        (1000) am        (1000)     2924 2023-04-23 14:14:34.000000 terka-1.6.4.2/terka/service_layer/services.py
--rw-r--r--   0 am        (1000) am        (1000)     3882 2023-02-12 14:00:44.000000 terka-1.6.4.2/terka/service_layer/ui.py
--rw-r--r--   0 am        (1000) am        (1000)      698 2023-02-12 13:59:50.000000 terka-1.6.4.2/terka/service_layer/vertical_layout.css
--rw-r--r--   0 am        (1000) am        (1000)     1441 2023-04-23 13:10:22.000000 terka-1.6.4.2/terka/service_layer/views.py
--rw-r--r--   0 am        (1000) am        (1000)     7743 2023-04-23 13:28:15.000000 terka-1.6.4.2/terka/utils.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 14:15:55.682387 terka-1.6.4.2/terka.egg-info/
--rw-r--r--   0 am        (1000) am        (1000)     1212 2023-04-23 14:15:55.000000 terka-1.6.4.2/terka.egg-info/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)      993 2023-04-23 14:15:55.000000 terka-1.6.4.2/terka.egg-info/SOURCES.txt
--rw-r--r--   0 am        (1000) am        (1000)        1 2023-04-23 14:15:55.000000 terka-1.6.4.2/terka.egg-info/dependency_links.txt
--rw-r--r--   0 am        (1000) am        (1000)       51 2023-04-23 14:15:55.000000 terka-1.6.4.2/terka.egg-info/entry_points.txt
--rw-r--r--   0 am        (1000) am        (1000)       52 2023-04-23 14:15:55.000000 terka-1.6.4.2/terka.egg-info/requires.txt
--rw-r--r--   0 am        (1000) am        (1000)        6 2023-04-23 14:15:55.000000 terka-1.6.4.2/terka.egg-info/top_level.txt
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 14:21:06.300977 terka-1.6.4.3/
+-rw-r--r--   0 am        (1000) am        (1000)     1212 2023-04-23 14:21:06.300977 terka-1.6.4.3/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)       38 2023-04-23 14:21:06.300977 terka-1.6.4.3/setup.cfg
+-rw-r--r--   0 am        (1000) am        (1000)      899 2023-04-23 14:21:04.000000 terka-1.6.4.3/setup.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 14:21:06.296977 terka-1.6.4.3/terka/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-23 14:06:23.000000 terka-1.6.4.3/terka/__init__.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 14:21:06.300977 terka-1.6.4.3/terka/adapters/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.3/terka/adapters/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    16083 2023-04-23 14:14:21.000000 terka-1.6.4.3/terka/adapters/orm.py
+-rw-r--r--   0 am        (1000) am        (1000)     6150 2023-04-23 14:10:47.000000 terka-1.6.4.3/terka/adapters/repository.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 14:21:06.300977 terka-1.6.4.3/terka/domain/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.3/terka/domain/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-06 18:49:11.000000 terka-1.6.4.3/terka/domain/collaborators.py
+-rw-r--r--   0 am        (1000) am        (1000)    41005 2023-04-23 14:11:14.000000 terka-1.6.4.3/terka/domain/commands.py
+-rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-12 20:16:29.000000 terka-1.6.4.3/terka/domain/commentary.py
+-rw-r--r--   0 am        (1000) am        (1000)      102 2023-01-26 19:46:39.000000 terka-1.6.4.3/terka/domain/element.py
+-rw-r--r--   0 am        (1000) am        (1000)      961 2023-04-23 14:11:41.000000 terka-1.6.4.3/terka/domain/epic.py
+-rw-r--r--   0 am        (1000) am        (1000)     1440 2023-03-12 20:44:34.000000 terka-1.6.4.3/terka/domain/event_history.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 14:21:06.300977 terka-1.6.4.3/terka/domain/external_connectors/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-23 13:50:48.000000 terka-1.6.4.3/terka/domain/external_connectors/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      187 2023-04-23 13:40:28.000000 terka-1.6.4.3/terka/domain/external_connectors/asana.py
+-rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.6.4.3/terka/domain/helpers.py
+-rw-r--r--   0 am        (1000) am        (1000)      892 2023-03-17 11:37:47.000000 terka-1.6.4.3/terka/domain/project.py
+-rw-r--r--   0 am        (1000) am        (1000)     2167 2023-04-23 14:12:42.000000 terka-1.6.4.3/terka/domain/sprint.py
+-rw-r--r--   0 am        (1000) am        (1000)      955 2023-04-23 14:12:46.000000 terka-1.6.4.3/terka/domain/story.py
+-rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-06 19:04:21.000000 terka-1.6.4.3/terka/domain/tag.py
+-rw-r--r--   0 am        (1000) am        (1000)     2039 2023-04-07 19:10:02.000000 terka-1.6.4.3/terka/domain/task.py
+-rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-08 10:39:03.000000 terka-1.6.4.3/terka/domain/time_tracker.py
+-rw-r--r--   0 am        (1000) am        (1000)      338 2023-04-23 14:13:11.000000 terka-1.6.4.3/terka/domain/user.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 14:21:06.300977 terka-1.6.4.3/terka/entrypoints/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-02-11 17:56:56.000000 terka-1.6.4.3/terka/entrypoints/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)     5079 2023-04-23 14:13:55.000000 terka-1.6.4.3/terka/entrypoints/cli.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 14:21:06.300977 terka-1.6.4.3/terka/service_layer/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.3/terka/service_layer/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    27276 2023-04-23 14:14:50.000000 terka-1.6.4.3/terka/service_layer/printer.py
+-rw-r--r--   0 am        (1000) am        (1000)     2924 2023-04-23 14:14:34.000000 terka-1.6.4.3/terka/service_layer/services.py
+-rw-r--r--   0 am        (1000) am        (1000)     3882 2023-02-12 14:00:44.000000 terka-1.6.4.3/terka/service_layer/ui.py
+-rw-r--r--   0 am        (1000) am        (1000)      698 2023-02-12 13:59:50.000000 terka-1.6.4.3/terka/service_layer/vertical_layout.css
+-rw-r--r--   0 am        (1000) am        (1000)     1441 2023-04-23 13:10:22.000000 terka-1.6.4.3/terka/service_layer/views.py
+-rw-r--r--   0 am        (1000) am        (1000)     7743 2023-04-23 13:28:15.000000 terka-1.6.4.3/terka/utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 14:21:06.300977 terka-1.6.4.3/terka.egg-info/
+-rw-r--r--   0 am        (1000) am        (1000)     1212 2023-04-23 14:21:06.000000 terka-1.6.4.3/terka.egg-info/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)      993 2023-04-23 14:21:06.000000 terka-1.6.4.3/terka.egg-info/SOURCES.txt
+-rw-r--r--   0 am        (1000) am        (1000)        1 2023-04-23 14:21:06.000000 terka-1.6.4.3/terka.egg-info/dependency_links.txt
+-rw-r--r--   0 am        (1000) am        (1000)       51 2023-04-23 14:21:06.000000 terka-1.6.4.3/terka.egg-info/entry_points.txt
+-rw-r--r--   0 am        (1000) am        (1000)       52 2023-04-23 14:21:06.000000 terka-1.6.4.3/terka.egg-info/requires.txt
+-rw-r--r--   0 am        (1000) am        (1000)        6 2023-04-23 14:21:06.000000 terka-1.6.4.3/terka.egg-info/top_level.txt
```

### Comparing `terka-1.6.4.2/PKG-INFO` & `terka-1.6.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terka
-Version: 1.6.4.2
+Version: 1.6.4.3
 Summary: CLI utility for creating and managing tasks in a terminal
 Home-page: https://github.com/AndreyMarkinPPC/terka
 Author: Andrei Markin
 Author-email: andrey.markin.ppc@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
```

### Comparing `terka-1.6.4.2/setup.py` & `terka-1.6.4.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pathlib
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
-README = (HERE / "../README.md").read_text()
+README = (HERE.parent / "README.md").read_text()
 
 setup(
     name="terka",
-    version="1.6.4.2",
+    version="1.6.4.3",
     description="CLI utility for creating and managing tasks in a terminal",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Andrei Markin",
     author_email="andrey.markin.ppc@gmail.com",
     license="Apache 2.0",
     url="https://github.com/AndreyMarkinPPC/terka",
```

### Comparing `terka-1.6.4.2/terka/adapters/orm.py` & `terka-1.6.4.3/terka/adapters/orm.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.2/terka/adapters/repository.py` & `terka-1.6.4.3/terka/adapters/repository.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.2/terka/domain/collaborators.py` & `terka-1.6.4.3/terka/domain/collaborators.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.2/terka/domain/commands.py` & `terka-1.6.4.3/terka/domain/commands.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.2/terka/domain/commentary.py` & `terka-1.6.4.3/terka/domain/commentary.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.2/terka/domain/epic.py` & `terka-1.6.4.3/terka/domain/epic.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.2/terka/domain/event_history.py` & `terka-1.6.4.3/terka/domain/event_history.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.2/terka/domain/project.py` & `terka-1.6.4.3/terka/domain/project.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.2/terka/domain/sprint.py` & `terka-1.6.4.3/terka/domain/sprint.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.2/terka/domain/story.py` & `terka-1.6.4.3/terka/domain/story.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.2/terka/domain/tag.py` & `terka-1.6.4.3/terka/domain/tag.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.2/terka/domain/task.py` & `terka-1.6.4.3/terka/domain/task.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.2/terka/domain/time_tracker.py` & `terka-1.6.4.3/terka/domain/time_tracker.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.2/terka/entrypoints/cli.py` & `terka-1.6.4.3/terka/entrypoints/cli.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.2/terka/service_layer/printer.py` & `terka-1.6.4.3/terka/service_layer/printer.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.2/terka/service_layer/services.py` & `terka-1.6.4.3/terka/service_layer/services.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.2/terka/service_layer/ui.py` & `terka-1.6.4.3/terka/service_layer/ui.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.2/terka/service_layer/vertical_layout.css` & `terka-1.6.4.3/terka/service_layer/vertical_layout.css`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.2/terka/service_layer/views.py` & `terka-1.6.4.3/terka/service_layer/views.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.2/terka/utils.py` & `terka-1.6.4.3/terka/utils.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.2/terka.egg-info/PKG-INFO` & `terka-1.6.4.3/terka.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terka
-Version: 1.6.4.2
+Version: 1.6.4.3
 Summary: CLI utility for creating and managing tasks in a terminal
 Home-page: https://github.com/AndreyMarkinPPC/terka
 Author: Andrei Markin
 Author-email: andrey.markin.ppc@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
```

### Comparing `terka-1.6.4.2/terka.egg-info/SOURCES.txt` & `terka-1.6.4.3/terka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

