# Comparing `tmp/terka-1.6.4.tar.gz` & `tmp/terka-1.6.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terka-1.6.4.tar", last modified: Sun Apr 23 13:44:51 2023, max compression
+gzip compressed data, was "terka-1.6.4.1.tar", last modified: Sun Apr 23 13:51:20 2023, max compression
```

## Comparing `terka-1.6.4.tar` & `terka-1.6.4.1.tar`

### file list

```diff
@@ -1,54 +1,57 @@
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:44:51.492537 terka-1.6.4/
--rw-r--r--   0 am        (1000) am        (1000)    11357 2023-04-05 21:39:45.000000 terka-1.6.4/LICENSE
--rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-23 13:44:51.492537 terka-1.6.4/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)      917 2023-03-06 22:25:53.000000 terka-1.6.4/README.md
--rw-r--r--   0 am        (1000) am        (1000)       38 2023-04-23 13:44:51.492537 terka-1.6.4/setup.cfg
--rw-r--r--   0 am        (1000) am        (1000)      890 2023-04-23 13:44:41.000000 terka-1.6.4/setup.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:44:51.488535 terka-1.6.4/src/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4/src/__init__.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:44:51.488535 terka-1.6.4/src/adapters/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4/src/adapters/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    16059 2023-04-23 13:38:52.000000 terka-1.6.4/src/adapters/orm.py
--rw-r--r--   0 am        (1000) am        (1000)     6139 2023-04-19 21:12:52.000000 terka-1.6.4/src/adapters/repository.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:44:51.488535 terka-1.6.4/src/domain/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4/src/domain/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-06 18:49:11.000000 terka-1.6.4/src/domain/collaborators.py
--rw-r--r--   0 am        (1000) am        (1000)    41043 2023-04-23 13:40:04.000000 terka-1.6.4/src/domain/commands.py
--rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-12 20:16:29.000000 terka-1.6.4/src/domain/commentary.py
--rw-r--r--   0 am        (1000) am        (1000)      102 2023-01-26 19:46:39.000000 terka-1.6.4/src/domain/element.py
--rw-r--r--   0 am        (1000) am        (1000)      959 2023-04-08 10:39:03.000000 terka-1.6.4/src/domain/epic.py
--rw-r--r--   0 am        (1000) am        (1000)     1440 2023-03-12 20:44:34.000000 terka-1.6.4/src/domain/event_history.py
--rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.6.4/src/domain/helpers.py
--rw-r--r--   0 am        (1000) am        (1000)      892 2023-03-17 11:37:47.000000 terka-1.6.4/src/domain/project.py
--rw-r--r--   0 am        (1000) am        (1000)     2177 2023-04-15 18:25:02.000000 terka-1.6.4/src/domain/sprint.py
--rw-r--r--   0 am        (1000) am        (1000)      965 2023-04-08 10:39:03.000000 terka-1.6.4/src/domain/story.py
--rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-06 19:04:21.000000 terka-1.6.4/src/domain/tag.py
--rw-r--r--   0 am        (1000) am        (1000)     2039 2023-04-07 19:10:02.000000 terka-1.6.4/src/domain/task.py
--rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-08 10:39:03.000000 terka-1.6.4/src/domain/time_tracker.py
--rw-r--r--   0 am        (1000) am        (1000)      792 2023-01-26 19:46:39.000000 terka-1.6.4/src/domain/user.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:44:51.488535 terka-1.6.4/src/entrypoints/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-02-11 17:56:56.000000 terka-1.6.4/src/entrypoints/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)     5069 2023-04-23 13:13:52.000000 terka-1.6.4/src/entrypoints/cli.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:44:51.492537 terka-1.6.4/src/service_layer/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4/src/service_layer/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    27272 2023-04-23 12:13:55.000000 terka-1.6.4/src/service_layer/printer.py
--rw-r--r--   0 am        (1000) am        (1000)     2918 2023-04-11 15:29:13.000000 terka-1.6.4/src/service_layer/services.py
--rw-r--r--   0 am        (1000) am        (1000)     3882 2023-02-12 14:00:44.000000 terka-1.6.4/src/service_layer/ui.py
--rw-r--r--   0 am        (1000) am        (1000)      698 2023-02-12 13:59:50.000000 terka-1.6.4/src/service_layer/vertical_layout.css
--rw-r--r--   0 am        (1000) am        (1000)     1441 2023-04-23 13:10:22.000000 terka-1.6.4/src/service_layer/views.py
--rw-r--r--   0 am        (1000) am        (1000)     7743 2023-04-23 13:28:15.000000 terka-1.6.4/src/utils.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:44:51.492537 terka-1.6.4/terka.egg-info/
--rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-23 13:44:51.000000 terka-1.6.4/terka.egg-info/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)     1003 2023-04-23 13:44:51.000000 terka-1.6.4/terka.egg-info/SOURCES.txt
--rw-r--r--   0 am        (1000) am        (1000)        1 2023-04-23 13:44:51.000000 terka-1.6.4/terka.egg-info/dependency_links.txt
--rw-r--r--   0 am        (1000) am        (1000)       51 2023-04-23 13:44:51.000000 terka-1.6.4/terka.egg-info/entry_points.txt
--rw-r--r--   0 am        (1000) am        (1000)       52 2023-04-23 13:44:51.000000 terka-1.6.4/terka.egg-info/requires.txt
--rw-r--r--   0 am        (1000) am        (1000)       10 2023-04-23 13:44:51.000000 terka-1.6.4/terka.egg-info/top_level.txt
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:44:51.492537 terka-1.6.4/tests/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4/tests/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      424 2023-01-26 19:46:39.000000 terka-1.6.4/tests/conftest.py
--rw-r--r--   0 am        (1000) am        (1000)       43 2023-01-26 19:46:39.000000 terka-1.6.4/tests/test_commands.py
--rw-r--r--   0 am        (1000) am        (1000)     2818 2023-01-26 19:46:39.000000 terka-1.6.4/tests/test_orm.py
--rw-r--r--   0 am        (1000) am        (1000)      956 2023-01-26 19:46:39.000000 terka-1.6.4/tests/test_task.py
--rw-r--r--   0 am        (1000) am        (1000)     1281 2023-01-26 19:46:39.000000 terka-1.6.4/tests/test_user.py
--rw-r--r--   0 am        (1000) am        (1000)      265 2023-01-26 19:46:39.000000 terka-1.6.4/tests/test_utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:51:20.324544 terka-1.6.4.1/
+-rw-r--r--   0 am        (1000) am        (1000)    11357 2023-04-05 21:39:45.000000 terka-1.6.4.1/LICENSE
+-rw-r--r--   0 am        (1000) am        (1000)     1234 2023-04-23 13:51:20.324544 terka-1.6.4.1/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)      917 2023-03-06 22:25:53.000000 terka-1.6.4.1/README.md
+-rw-r--r--   0 am        (1000) am        (1000)       38 2023-04-23 13:51:20.324544 terka-1.6.4.1/setup.cfg
+-rw-r--r--   0 am        (1000) am        (1000)      892 2023-04-23 13:51:07.000000 terka-1.6.4.1/setup.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:51:20.320544 terka-1.6.4.1/src/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.1/src/__init__.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:51:20.320544 terka-1.6.4.1/src/adapters/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.1/src/adapters/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    16059 2023-04-23 13:38:52.000000 terka-1.6.4.1/src/adapters/orm.py
+-rw-r--r--   0 am        (1000) am        (1000)     6139 2023-04-19 21:12:52.000000 terka-1.6.4.1/src/adapters/repository.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:51:20.324544 terka-1.6.4.1/src/domain/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.1/src/domain/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-06 18:49:11.000000 terka-1.6.4.1/src/domain/collaborators.py
+-rw-r--r--   0 am        (1000) am        (1000)    41043 2023-04-23 13:40:04.000000 terka-1.6.4.1/src/domain/commands.py
+-rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-12 20:16:29.000000 terka-1.6.4.1/src/domain/commentary.py
+-rw-r--r--   0 am        (1000) am        (1000)      102 2023-01-26 19:46:39.000000 terka-1.6.4.1/src/domain/element.py
+-rw-r--r--   0 am        (1000) am        (1000)      959 2023-04-08 10:39:03.000000 terka-1.6.4.1/src/domain/epic.py
+-rw-r--r--   0 am        (1000) am        (1000)     1440 2023-03-12 20:44:34.000000 terka-1.6.4.1/src/domain/event_history.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:51:20.324544 terka-1.6.4.1/src/domain/external_connectors/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-23 13:50:48.000000 terka-1.6.4.1/src/domain/external_connectors/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      187 2023-04-23 13:40:28.000000 terka-1.6.4.1/src/domain/external_connectors/asana.py
+-rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.6.4.1/src/domain/helpers.py
+-rw-r--r--   0 am        (1000) am        (1000)      892 2023-03-17 11:37:47.000000 terka-1.6.4.1/src/domain/project.py
+-rw-r--r--   0 am        (1000) am        (1000)     2177 2023-04-15 18:25:02.000000 terka-1.6.4.1/src/domain/sprint.py
+-rw-r--r--   0 am        (1000) am        (1000)      965 2023-04-08 10:39:03.000000 terka-1.6.4.1/src/domain/story.py
+-rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-06 19:04:21.000000 terka-1.6.4.1/src/domain/tag.py
+-rw-r--r--   0 am        (1000) am        (1000)     2039 2023-04-07 19:10:02.000000 terka-1.6.4.1/src/domain/task.py
+-rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-08 10:39:03.000000 terka-1.6.4.1/src/domain/time_tracker.py
+-rw-r--r--   0 am        (1000) am        (1000)      792 2023-01-26 19:46:39.000000 terka-1.6.4.1/src/domain/user.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:51:20.324544 terka-1.6.4.1/src/entrypoints/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-02-11 17:56:56.000000 terka-1.6.4.1/src/entrypoints/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)     5069 2023-04-23 13:13:52.000000 terka-1.6.4.1/src/entrypoints/cli.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:51:20.324544 terka-1.6.4.1/src/service_layer/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.1/src/service_layer/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    27272 2023-04-23 12:13:55.000000 terka-1.6.4.1/src/service_layer/printer.py
+-rw-r--r--   0 am        (1000) am        (1000)     2918 2023-04-11 15:29:13.000000 terka-1.6.4.1/src/service_layer/services.py
+-rw-r--r--   0 am        (1000) am        (1000)     3882 2023-02-12 14:00:44.000000 terka-1.6.4.1/src/service_layer/ui.py
+-rw-r--r--   0 am        (1000) am        (1000)      698 2023-02-12 13:59:50.000000 terka-1.6.4.1/src/service_layer/vertical_layout.css
+-rw-r--r--   0 am        (1000) am        (1000)     1441 2023-04-23 13:10:22.000000 terka-1.6.4.1/src/service_layer/views.py
+-rw-r--r--   0 am        (1000) am        (1000)     7743 2023-04-23 13:28:15.000000 terka-1.6.4.1/src/utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:51:20.324544 terka-1.6.4.1/terka.egg-info/
+-rw-r--r--   0 am        (1000) am        (1000)     1234 2023-04-23 13:51:20.000000 terka-1.6.4.1/terka.egg-info/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)     1086 2023-04-23 13:51:20.000000 terka-1.6.4.1/terka.egg-info/SOURCES.txt
+-rw-r--r--   0 am        (1000) am        (1000)        1 2023-04-23 13:51:20.000000 terka-1.6.4.1/terka.egg-info/dependency_links.txt
+-rw-r--r--   0 am        (1000) am        (1000)       51 2023-04-23 13:51:20.000000 terka-1.6.4.1/terka.egg-info/entry_points.txt
+-rw-r--r--   0 am        (1000) am        (1000)       52 2023-04-23 13:51:20.000000 terka-1.6.4.1/terka.egg-info/requires.txt
+-rw-r--r--   0 am        (1000) am        (1000)       10 2023-04-23 13:51:20.000000 terka-1.6.4.1/terka.egg-info/top_level.txt
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:51:20.324544 terka-1.6.4.1/tests/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.1/tests/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      424 2023-01-26 19:46:39.000000 terka-1.6.4.1/tests/conftest.py
+-rw-r--r--   0 am        (1000) am        (1000)       43 2023-01-26 19:46:39.000000 terka-1.6.4.1/tests/test_commands.py
+-rw-r--r--   0 am        (1000) am        (1000)     2818 2023-01-26 19:46:39.000000 terka-1.6.4.1/tests/test_orm.py
+-rw-r--r--   0 am        (1000) am        (1000)      956 2023-01-26 19:46:39.000000 terka-1.6.4.1/tests/test_task.py
+-rw-r--r--   0 am        (1000) am        (1000)     1281 2023-01-26 19:46:39.000000 terka-1.6.4.1/tests/test_user.py
+-rw-r--r--   0 am        (1000) am        (1000)      265 2023-01-26 19:46:39.000000 terka-1.6.4.1/tests/test_utils.py
```

### Comparing `terka-1.6.4/LICENSE` & `terka-1.6.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `terka-1.6.4/PKG-INFO` & `terka-1.6.4.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terka
-Version: 1.6.4
+Version: 1.6.4.1
 Summary: CLI utility for creating and managing tasks in a terminal
 Home-page: https://github.com/AndreyMarkinPPC/terka
 Author: Andrei Markin
 Author-email: andrey.markin.ppc@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `terka-1.6.4/README.md` & `terka-1.6.4.1/README.md`

 * *Files identical despite different names*

### Comparing `terka-1.6.4/setup.py` & `terka-1.6.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(
     name="terka",
-    version="1.6.4",
+    version="1.6.4.1",
     description="CLI utility for creating and managing tasks in a terminal",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Andrei Markin",
     author_email="andrey.markin.ppc@gmail.com",
     license="Apache 2.0",
     url="https://github.com/AndreyMarkinPPC/terka",
```

### Comparing `terka-1.6.4/src/adapters/orm.py` & `terka-1.6.4.1/src/adapters/orm.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4/src/adapters/repository.py` & `terka-1.6.4.1/src/adapters/repository.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4/src/domain/collaborators.py` & `terka-1.6.4.1/src/domain/collaborators.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4/src/domain/commands.py` & `terka-1.6.4.1/src/domain/commands.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4/src/domain/commentary.py` & `terka-1.6.4.1/src/domain/commentary.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4/src/domain/epic.py` & `terka-1.6.4.1/src/domain/epic.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4/src/domain/event_history.py` & `terka-1.6.4.1/src/domain/event_history.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4/src/domain/project.py` & `terka-1.6.4.1/src/domain/project.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4/src/domain/sprint.py` & `terka-1.6.4.1/src/domain/sprint.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4/src/domain/story.py` & `terka-1.6.4.1/src/domain/story.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4/src/domain/tag.py` & `terka-1.6.4.1/src/domain/tag.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4/src/domain/task.py` & `terka-1.6.4.1/src/domain/task.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4/src/domain/time_tracker.py` & `terka-1.6.4.1/src/domain/time_tracker.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4/src/domain/user.py` & `terka-1.6.4.1/src/domain/user.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4/src/entrypoints/cli.py` & `terka-1.6.4.1/src/entrypoints/cli.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4/src/service_layer/printer.py` & `terka-1.6.4.1/src/service_layer/printer.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4/src/service_layer/services.py` & `terka-1.6.4.1/src/service_layer/services.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4/src/service_layer/ui.py` & `terka-1.6.4.1/src/service_layer/ui.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4/src/service_layer/vertical_layout.css` & `terka-1.6.4.1/src/service_layer/vertical_layout.css`

 * *Files identical despite different names*

### Comparing `terka-1.6.4/src/service_layer/views.py` & `terka-1.6.4.1/src/service_layer/views.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4/src/utils.py` & `terka-1.6.4.1/src/utils.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4/terka.egg-info/PKG-INFO` & `terka-1.6.4.1/terka.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terka
-Version: 1.6.4
+Version: 1.6.4.1
 Summary: CLI utility for creating and managing tasks in a terminal
 Home-page: https://github.com/AndreyMarkinPPC/terka
 Author: Andrei Markin
 Author-email: andrey.markin.ppc@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `terka-1.6.4/terka.egg-info/SOURCES.txt` & `terka-1.6.4.1/terka.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 src/domain/project.py
 src/domain/sprint.py
 src/domain/story.py
 src/domain/tag.py
 src/domain/task.py
 src/domain/time_tracker.py
 src/domain/user.py
+src/domain/external_connectors/__init__.py
+src/domain/external_connectors/asana.py
 src/entrypoints/__init__.py
 src/entrypoints/cli.py
 src/service_layer/__init__.py
 src/service_layer/printer.py
 src/service_layer/services.py
 src/service_layer/ui.py
 src/service_layer/vertical_layout.css
```

### Comparing `terka-1.6.4/tests/test_orm.py` & `terka-1.6.4.1/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4/tests/test_task.py` & `terka-1.6.4.1/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4/tests/test_user.py` & `terka-1.6.4.1/tests/test_user.py`

 * *Files identical despite different names*

