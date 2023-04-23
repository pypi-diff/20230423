# Comparing `tmp/terka-1.6.4.1.tar.gz` & `tmp/terka-1.6.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terka-1.6.4.1.tar", last modified: Sun Apr 23 13:51:20 2023, max compression
+gzip compressed data, was "terka-1.6.4.2.tar", last modified: Sun Apr 23 14:15:55 2023, max compression
```

## Comparing `terka-1.6.4.1.tar` & `terka-1.6.4.2.tar`

### file list

```diff
@@ -1,57 +1,47 @@
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:51:20.324544 terka-1.6.4.1/
--rw-r--r--   0 am        (1000) am        (1000)    11357 2023-04-05 21:39:45.000000 terka-1.6.4.1/LICENSE
--rw-r--r--   0 am        (1000) am        (1000)     1234 2023-04-23 13:51:20.324544 terka-1.6.4.1/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)      917 2023-03-06 22:25:53.000000 terka-1.6.4.1/README.md
--rw-r--r--   0 am        (1000) am        (1000)       38 2023-04-23 13:51:20.324544 terka-1.6.4.1/setup.cfg
--rw-r--r--   0 am        (1000) am        (1000)      892 2023-04-23 13:51:07.000000 terka-1.6.4.1/setup.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:51:20.320544 terka-1.6.4.1/src/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.1/src/__init__.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:51:20.320544 terka-1.6.4.1/src/adapters/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.1/src/adapters/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    16059 2023-04-23 13:38:52.000000 terka-1.6.4.1/src/adapters/orm.py
--rw-r--r--   0 am        (1000) am        (1000)     6139 2023-04-19 21:12:52.000000 terka-1.6.4.1/src/adapters/repository.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:51:20.324544 terka-1.6.4.1/src/domain/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.1/src/domain/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-06 18:49:11.000000 terka-1.6.4.1/src/domain/collaborators.py
--rw-r--r--   0 am        (1000) am        (1000)    41043 2023-04-23 13:40:04.000000 terka-1.6.4.1/src/domain/commands.py
--rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-12 20:16:29.000000 terka-1.6.4.1/src/domain/commentary.py
--rw-r--r--   0 am        (1000) am        (1000)      102 2023-01-26 19:46:39.000000 terka-1.6.4.1/src/domain/element.py
--rw-r--r--   0 am        (1000) am        (1000)      959 2023-04-08 10:39:03.000000 terka-1.6.4.1/src/domain/epic.py
--rw-r--r--   0 am        (1000) am        (1000)     1440 2023-03-12 20:44:34.000000 terka-1.6.4.1/src/domain/event_history.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:51:20.324544 terka-1.6.4.1/src/domain/external_connectors/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-23 13:50:48.000000 terka-1.6.4.1/src/domain/external_connectors/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      187 2023-04-23 13:40:28.000000 terka-1.6.4.1/src/domain/external_connectors/asana.py
--rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.6.4.1/src/domain/helpers.py
--rw-r--r--   0 am        (1000) am        (1000)      892 2023-03-17 11:37:47.000000 terka-1.6.4.1/src/domain/project.py
--rw-r--r--   0 am        (1000) am        (1000)     2177 2023-04-15 18:25:02.000000 terka-1.6.4.1/src/domain/sprint.py
--rw-r--r--   0 am        (1000) am        (1000)      965 2023-04-08 10:39:03.000000 terka-1.6.4.1/src/domain/story.py
--rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-06 19:04:21.000000 terka-1.6.4.1/src/domain/tag.py
--rw-r--r--   0 am        (1000) am        (1000)     2039 2023-04-07 19:10:02.000000 terka-1.6.4.1/src/domain/task.py
--rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-08 10:39:03.000000 terka-1.6.4.1/src/domain/time_tracker.py
--rw-r--r--   0 am        (1000) am        (1000)      792 2023-01-26 19:46:39.000000 terka-1.6.4.1/src/domain/user.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:51:20.324544 terka-1.6.4.1/src/entrypoints/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-02-11 17:56:56.000000 terka-1.6.4.1/src/entrypoints/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)     5069 2023-04-23 13:13:52.000000 terka-1.6.4.1/src/entrypoints/cli.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:51:20.324544 terka-1.6.4.1/src/service_layer/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.1/src/service_layer/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    27272 2023-04-23 12:13:55.000000 terka-1.6.4.1/src/service_layer/printer.py
--rw-r--r--   0 am        (1000) am        (1000)     2918 2023-04-11 15:29:13.000000 terka-1.6.4.1/src/service_layer/services.py
--rw-r--r--   0 am        (1000) am        (1000)     3882 2023-02-12 14:00:44.000000 terka-1.6.4.1/src/service_layer/ui.py
--rw-r--r--   0 am        (1000) am        (1000)      698 2023-02-12 13:59:50.000000 terka-1.6.4.1/src/service_layer/vertical_layout.css
--rw-r--r--   0 am        (1000) am        (1000)     1441 2023-04-23 13:10:22.000000 terka-1.6.4.1/src/service_layer/views.py
--rw-r--r--   0 am        (1000) am        (1000)     7743 2023-04-23 13:28:15.000000 terka-1.6.4.1/src/utils.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:51:20.324544 terka-1.6.4.1/terka.egg-info/
--rw-r--r--   0 am        (1000) am        (1000)     1234 2023-04-23 13:51:20.000000 terka-1.6.4.1/terka.egg-info/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)     1086 2023-04-23 13:51:20.000000 terka-1.6.4.1/terka.egg-info/SOURCES.txt
--rw-r--r--   0 am        (1000) am        (1000)        1 2023-04-23 13:51:20.000000 terka-1.6.4.1/terka.egg-info/dependency_links.txt
--rw-r--r--   0 am        (1000) am        (1000)       51 2023-04-23 13:51:20.000000 terka-1.6.4.1/terka.egg-info/entry_points.txt
--rw-r--r--   0 am        (1000) am        (1000)       52 2023-04-23 13:51:20.000000 terka-1.6.4.1/terka.egg-info/requires.txt
--rw-r--r--   0 am        (1000) am        (1000)       10 2023-04-23 13:51:20.000000 terka-1.6.4.1/terka.egg-info/top_level.txt
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:51:20.324544 terka-1.6.4.1/tests/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.1/tests/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      424 2023-01-26 19:46:39.000000 terka-1.6.4.1/tests/conftest.py
--rw-r--r--   0 am        (1000) am        (1000)       43 2023-01-26 19:46:39.000000 terka-1.6.4.1/tests/test_commands.py
--rw-r--r--   0 am        (1000) am        (1000)     2818 2023-01-26 19:46:39.000000 terka-1.6.4.1/tests/test_orm.py
--rw-r--r--   0 am        (1000) am        (1000)      956 2023-01-26 19:46:39.000000 terka-1.6.4.1/tests/test_task.py
--rw-r--r--   0 am        (1000) am        (1000)     1281 2023-01-26 19:46:39.000000 terka-1.6.4.1/tests/test_user.py
--rw-r--r--   0 am        (1000) am        (1000)      265 2023-01-26 19:46:39.000000 terka-1.6.4.1/tests/test_utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 14:15:55.686387 terka-1.6.4.2/
+-rw-r--r--   0 am        (1000) am        (1000)     1212 2023-04-23 14:15:55.686387 terka-1.6.4.2/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)       38 2023-04-23 14:15:55.686387 terka-1.6.4.2/setup.cfg
+-rw-r--r--   0 am        (1000) am        (1000)      895 2023-04-23 14:15:43.000000 terka-1.6.4.2/setup.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 14:15:55.682387 terka-1.6.4.2/terka/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-23 14:06:23.000000 terka-1.6.4.2/terka/__init__.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 14:15:55.682387 terka-1.6.4.2/terka/adapters/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.2/terka/adapters/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    16083 2023-04-23 14:14:21.000000 terka-1.6.4.2/terka/adapters/orm.py
+-rw-r--r--   0 am        (1000) am        (1000)     6150 2023-04-23 14:10:47.000000 terka-1.6.4.2/terka/adapters/repository.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 14:15:55.686387 terka-1.6.4.2/terka/domain/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.2/terka/domain/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-06 18:49:11.000000 terka-1.6.4.2/terka/domain/collaborators.py
+-rw-r--r--   0 am        (1000) am        (1000)    41005 2023-04-23 14:11:14.000000 terka-1.6.4.2/terka/domain/commands.py
+-rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-12 20:16:29.000000 terka-1.6.4.2/terka/domain/commentary.py
+-rw-r--r--   0 am        (1000) am        (1000)      102 2023-01-26 19:46:39.000000 terka-1.6.4.2/terka/domain/element.py
+-rw-r--r--   0 am        (1000) am        (1000)      961 2023-04-23 14:11:41.000000 terka-1.6.4.2/terka/domain/epic.py
+-rw-r--r--   0 am        (1000) am        (1000)     1440 2023-03-12 20:44:34.000000 terka-1.6.4.2/terka/domain/event_history.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 14:15:55.686387 terka-1.6.4.2/terka/domain/external_connectors/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-23 13:50:48.000000 terka-1.6.4.2/terka/domain/external_connectors/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      187 2023-04-23 13:40:28.000000 terka-1.6.4.2/terka/domain/external_connectors/asana.py
+-rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.6.4.2/terka/domain/helpers.py
+-rw-r--r--   0 am        (1000) am        (1000)      892 2023-03-17 11:37:47.000000 terka-1.6.4.2/terka/domain/project.py
+-rw-r--r--   0 am        (1000) am        (1000)     2167 2023-04-23 14:12:42.000000 terka-1.6.4.2/terka/domain/sprint.py
+-rw-r--r--   0 am        (1000) am        (1000)      955 2023-04-23 14:12:46.000000 terka-1.6.4.2/terka/domain/story.py
+-rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-06 19:04:21.000000 terka-1.6.4.2/terka/domain/tag.py
+-rw-r--r--   0 am        (1000) am        (1000)     2039 2023-04-07 19:10:02.000000 terka-1.6.4.2/terka/domain/task.py
+-rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-08 10:39:03.000000 terka-1.6.4.2/terka/domain/time_tracker.py
+-rw-r--r--   0 am        (1000) am        (1000)      338 2023-04-23 14:13:11.000000 terka-1.6.4.2/terka/domain/user.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 14:15:55.686387 terka-1.6.4.2/terka/entrypoints/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-02-11 17:56:56.000000 terka-1.6.4.2/terka/entrypoints/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)     5079 2023-04-23 14:13:55.000000 terka-1.6.4.2/terka/entrypoints/cli.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 14:15:55.686387 terka-1.6.4.2/terka/service_layer/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4.2/terka/service_layer/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    27276 2023-04-23 14:14:50.000000 terka-1.6.4.2/terka/service_layer/printer.py
+-rw-r--r--   0 am        (1000) am        (1000)     2924 2023-04-23 14:14:34.000000 terka-1.6.4.2/terka/service_layer/services.py
+-rw-r--r--   0 am        (1000) am        (1000)     3882 2023-02-12 14:00:44.000000 terka-1.6.4.2/terka/service_layer/ui.py
+-rw-r--r--   0 am        (1000) am        (1000)      698 2023-02-12 13:59:50.000000 terka-1.6.4.2/terka/service_layer/vertical_layout.css
+-rw-r--r--   0 am        (1000) am        (1000)     1441 2023-04-23 13:10:22.000000 terka-1.6.4.2/terka/service_layer/views.py
+-rw-r--r--   0 am        (1000) am        (1000)     7743 2023-04-23 13:28:15.000000 terka-1.6.4.2/terka/utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 14:15:55.682387 terka-1.6.4.2/terka.egg-info/
+-rw-r--r--   0 am        (1000) am        (1000)     1212 2023-04-23 14:15:55.000000 terka-1.6.4.2/terka.egg-info/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)      993 2023-04-23 14:15:55.000000 terka-1.6.4.2/terka.egg-info/SOURCES.txt
+-rw-r--r--   0 am        (1000) am        (1000)        1 2023-04-23 14:15:55.000000 terka-1.6.4.2/terka.egg-info/dependency_links.txt
+-rw-r--r--   0 am        (1000) am        (1000)       51 2023-04-23 14:15:55.000000 terka-1.6.4.2/terka.egg-info/entry_points.txt
+-rw-r--r--   0 am        (1000) am        (1000)       52 2023-04-23 14:15:55.000000 terka-1.6.4.2/terka.egg-info/requires.txt
+-rw-r--r--   0 am        (1000) am        (1000)        6 2023-04-23 14:15:55.000000 terka-1.6.4.2/terka.egg-info/top_level.txt
```

### Comparing `terka-1.6.4.1/PKG-INFO` & `terka-1.6.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: terka
-Version: 1.6.4.1
+Version: 1.6.4.2
 Summary: CLI utility for creating and managing tasks in a terminal
 Home-page: https://github.com/AndreyMarkinPPC/terka
 Author: Andrei Markin
 Author-email: andrey.markin.ppc@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Terka - Ter[minal] Ka[nban]
 
 `terka` (pronounced *tyorka* or *Тёрка*) is a CLI tool that helps you manage your tasks
 in the terminal. Create task, assign it to a project, update it status, write
 comments and many more!
```

### Comparing `terka-1.6.4.1/README.md` & `terka-1.6.4.2/terka.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: terka
+Version: 1.6.4.2
+Summary: CLI utility for creating and managing tasks in a terminal
+Home-page: https://github.com/AndreyMarkinPPC/terka
+Author: Andrei Markin
+Author-email: andrey.markin.ppc@gmail.com
+License: Apache 2.0
+Description-Content-Type: text/markdown
+
 # Terka - Ter[minal] Ka[nban]
 
 `terka` (pronounced *tyorka* or *Тёрка*) is a CLI tool that helps you manage your tasks
 in the terminal. Create task, assign it to a project, update it status, write
 comments and many more!
 
 ## Installation
```

### Comparing `terka-1.6.4.1/setup.py` & `terka-1.6.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pathlib
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
-README = (HERE / "README.md").read_text()
+README = (HERE / "../README.md").read_text()
 
 setup(
     name="terka",
-    version="1.6.4.1",
+    version="1.6.4.2",
     description="CLI utility for creating and managing tasks in a terminal",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Andrei Markin",
     author_email="andrey.markin.ppc@gmail.com",
     license="Apache 2.0",
     url="https://github.com/AndreyMarkinPPC/terka",
```

### Comparing `terka-1.6.4.1/src/adapters/orm.py` & `terka-1.6.4.2/terka/adapters/orm.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,27 +11,27 @@
     Boolean,
     Enum,
     ForeignKey,
     event,
 )
 from sqlalchemy.orm import mapper, registry, relationship, validates, declarative_base
 
-from src.domain.task import Task, TaskStatus, TaskPriority
-from src.domain.user import User
-from src.domain.project import Project, ProjectStatus
-from src.domain.event_history import TaskEvent, ProjectEvent, EventType
-from src.domain.commentary import TaskCommentary, ProjectCommentary, EpicCommentary, StoryCommentary, SprintCommentary
-from src.domain.tag import BaseTag, TaskTag, ProjectTag
-from src.domain.collaborators import TaskCollaborator, ProjectCollaborator
-from src.domain.sprint import Sprint, SprintStatus, SprintTask
-from src.domain.time_tracker import TimeTrackerEntry
-from src.domain.epic import Epic, EpicTask
-from src.domain.story import Story, StoryTask
+from terka.domain.task import Task, TaskStatus, TaskPriority
+from terka.domain.user import User
+from terka.domain.project import Project, ProjectStatus
+from terka.domain.event_history import TaskEvent, ProjectEvent, EventType
+from terka.domain.commentary import TaskCommentary, ProjectCommentary, EpicCommentary, StoryCommentary, SprintCommentary
+from terka.domain.tag import BaseTag, TaskTag, ProjectTag
+from terka.domain.collaborators import TaskCollaborator, ProjectCollaborator
+from terka.domain.sprint import Sprint, SprintStatus, SprintTask
+from terka.domain.time_tracker import TimeTrackerEntry
+from terka.domain.epic import Epic, EpicTask
+from terka.domain.story import Story, StoryTask
 
-from src.domain.external_connectors.asana import AsanaTask, AsanaProject
+from terka.domain.external_connectors.asana import AsanaTask, AsanaProject
 
 Base = declarative_base()
 metadata = MetaData()
 
 tasks = Table("tasks", metadata,
               Column("id", Integer, primary_key=True, autoincrement=True),
               Column("name", String(255)),
```

### Comparing `terka-1.6.4.1/src/adapters/repository.py` & `terka-1.6.4.2/terka/adapters/repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from typing import Dict, Optional
 
 import abc
 from datetime import datetime, timedelta
-from . import orm
-from src.domain.element import Element
-from src.domain.task import Task
-from src.domain.project import Project
-from src.domain.user import User
-from src.domain.event_history import TaskEvent
 from sqlalchemy import and_, or_, not_
 
+from terka.domain.element import Element
+from terka.domain.task import Task
+from terka.domain.project import Project
+from terka.domain.user import User
+from terka.domain.event_history import TaskEvent
+from . import orm
+
 
 class AbsRepository(abc.ABC):
 
     def __init__(self):
         pass
 
     def add(self, element: Element) -> None:
```

### Comparing `terka-1.6.4.1/src/domain/collaborators.py` & `terka-1.6.4.2/terka/domain/collaborators.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.1/src/domain/commands.py` & `terka-1.6.4.2/terka/domain/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,31 +9,31 @@
 import yaml
 
 import logging
 import rich
 from rich.console import Console
 from rich.table import Table
 
-from src.domain.task import Task
-from src.domain.project import Project
-from src.domain.user import User
-from src.domain.commentary import TaskCommentary, ProjectCommentary, EpicCommentary, StoryCommentary, SprintCommentary
-from src.domain.tag import BaseTag, TaskTag, ProjectTag
-from src.domain.collaborators import TaskCollaborator, ProjectCollaborator
-from src.domain.event_history import TaskEvent, ProjectEvent
-from src.domain.sprint import Sprint, SprintTask
-from src.domain.time_tracker import TimeTrackerEntry
-from src.domain.epic import Epic, EpicTask
-from src.domain.story import Story, StoryTask
-from src.domain.external_connectors.asana import AsanaTask, AsanaProject
-
-from src.service_layer import services, printer
-from src.service_layer.ui import TerkaTask
-from src.adapters.repository import AbsRepository
-from src.utils import format_command, format_task_dict
+from terka.domain.task import Task
+from terka.domain.project import Project
+from terka.domain.user import User
+from terka.domain.commentary import TaskCommentary, ProjectCommentary, EpicCommentary, StoryCommentary, SprintCommentary
+from terka.domain.tag import BaseTag, TaskTag, ProjectTag
+from terka.domain.collaborators import TaskCollaborator, ProjectCollaborator
+from terka.domain.event_history import TaskEvent, ProjectEvent
+from terka.domain.sprint import Sprint, SprintTask
+from terka.domain.time_tracker import TimeTrackerEntry
+from terka.domain.epic import Epic, EpicTask
+from terka.domain.story import Story, StoryTask
+from terka.domain.external_connectors.asana import AsanaTask, AsanaProject
+
+from terka.service_layer import services, printer
+from terka.service_layer.ui import TerkaTask
+from terka.adapters.repository import AbsRepository
+from terka.utils import format_command, format_task_dict
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class CurrentEntry:
     value: str
@@ -627,18 +627,16 @@
             if entity not in (Task, Project):
                 raise ValueError("'connect' operation only allowed for tasks and project!")
             task_ids = get_ids(kwargs.get("id"))
             for task_id in task_ids:
                 if entity_type == "projects":
                     asana_project_id = kwargs.get("external_project")
                     asana_project = self.repo.get_by_id(AsanaProject, task_id)
-                    breakpoint()
                     if not asana_project:
                         obj = AsanaProject(id=task_id, asana_project_id=asana_project_id)
-                        breakpoint()
                         self.repo.add(obj)
                     else:
                         self.repo.update(AsanaProject, task_id, {"asana_project_id": asana_project_id})
                 elif entity_type == "tasks":
                     asana_task_id = kwargs.get("external_task")
                     asana_task = self.repo.get_by_id(AsanaProject, task_id)
                     if not asana_task:
```

### Comparing `terka-1.6.4.1/src/domain/commentary.py` & `terka-1.6.4.2/terka/domain/commentary.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.1/src/domain/epic.py` & `terka-1.6.4.2/terka/domain/epic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass
 from datetime import datetime
 
-from src.domain.task import Task
+from terka.domain.task import Task
 
 
 class Epic:
 
     def __init__(self,
                  name: str,
                  description: str = None,
```

### Comparing `terka-1.6.4.1/src/domain/event_history.py` & `terka-1.6.4.2/terka/domain/event_history.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.1/src/domain/project.py` & `terka-1.6.4.2/terka/domain/project.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.1/src/domain/sprint.py` & `terka-1.6.4.2/terka/domain/sprint.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Set
 from enum import Enum
 import logging
 from datetime import datetime
 from dataclasses import dataclass
 
-from src.domain.task import Task
+from .task import Task
 
 logger = logging.getLogger(__name__)
 
 
 class SprintStatus(Enum):
     PLANNED = 1
     ACTIVE = 2
```

### Comparing `terka-1.6.4.1/src/domain/story.py` & `terka-1.6.4.2/terka/domain/story.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass
 from datetime import datetime
 
-from src.domain.task import Task
+from .task import Task
 
 
 class Story:
 
     def __init__(self,
                  name: str,
                  description: str = None,
```

### Comparing `terka-1.6.4.1/src/domain/tag.py` & `terka-1.6.4.2/terka/domain/tag.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.1/src/domain/task.py` & `terka-1.6.4.2/terka/domain/task.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.1/src/domain/time_tracker.py` & `terka-1.6.4.2/terka/domain/time_tracker.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.1/src/entrypoints/cli.py` & `terka-1.6.4.2/terka/entrypoints/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 
 import rich
 from rich.console import Console
 from rich.table import Table
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker, clear_mappers
 
-from src.adapters.orm import metadata, start_mappers
-from src.adapters.repository import SqlAlchemyRepository
+from terka.adapters.orm import metadata, start_mappers
+from terka.adapters.repository import SqlAlchemyRepository
 
-from src.domain.commands import CommandHandler
-from src.utils import format_task_dict, process_command, update_task_dict, create_task_dict
-from src.service_layer import services
+from terka.domain.commands import CommandHandler
+from terka.utils import format_task_dict, process_command, update_task_dict, create_task_dict
+from terka.service_layer import services
 
 
 def init_db(home_dir):
     engine = create_engine(f"sqlite:////{home_dir}/.terka/tasks.db")
     metadata.create_all(engine)
     return engine
```

### Comparing `terka-1.6.4.1/src/service_layer/printer.py` & `terka-1.6.4.2/terka/service_layer/printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from datetime import datetime, date, timedelta
 import plotext as plt
 import rich
 from rich.console import Console
 from rich.table import Table
 from statistics import mean, median
 
-from src.service_layer import services, views
-from src.service_layer.ui import TerkaTask
+from terka.service_layer import services, views
+from terka.service_layer.ui import TerkaTask
 
 
 @dataclass
 class PrintOptions:
     show_tasks: bool = True
     show_history: bool = False
     show_commentaries: bool = False
```

### Comparing `terka-1.6.4.1/src/service_layer/services.py` & `terka-1.6.4.2/terka/service_layer/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, Optional
 import os
 import yaml
 
-from src.adapters.repository import AbsRepository
-from src.domain.project import Project
-from src.domain.user import User
+from terka.adapters.repository import AbsRepository
+from terka.domain.project import Project
+from terka.domain.user import User
 
 
 def update_config(update_pair: Dict[str, Any]):
     config = get_config()
     config.update(update_pair)
     with open(f"{home_dir}/.terka/config.yaml", "w") as f:
         yaml.dump(config, f)
```

### Comparing `terka-1.6.4.1/src/service_layer/ui.py` & `terka-1.6.4.2/terka/service_layer/ui.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.1/src/service_layer/vertical_layout.css` & `terka-1.6.4.2/terka/service_layer/vertical_layout.css`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.1/src/service_layer/views.py` & `terka-1.6.4.2/terka/service_layer/views.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.1/src/utils.py` & `terka-1.6.4.2/terka/utils.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.4.1/terka.egg-info/SOURCES.txt` & `terka-1.6.4.2/terka.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,37 @@
-LICENSE
-README.md
 setup.py
-src/__init__.py
-src/utils.py
-src/adapters/__init__.py
-src/adapters/orm.py
-src/adapters/repository.py
-src/domain/__init__.py
-src/domain/collaborators.py
-src/domain/commands.py
-src/domain/commentary.py
-src/domain/element.py
-src/domain/epic.py
-src/domain/event_history.py
-src/domain/helpers.py
-src/domain/project.py
-src/domain/sprint.py
-src/domain/story.py
-src/domain/tag.py
-src/domain/task.py
-src/domain/time_tracker.py
-src/domain/user.py
-src/domain/external_connectors/__init__.py
-src/domain/external_connectors/asana.py
-src/entrypoints/__init__.py
-src/entrypoints/cli.py
-src/service_layer/__init__.py
-src/service_layer/printer.py
-src/service_layer/services.py
-src/service_layer/ui.py
-src/service_layer/vertical_layout.css
-src/service_layer/views.py
+terka/__init__.py
+terka/utils.py
 terka.egg-info/PKG-INFO
 terka.egg-info/SOURCES.txt
 terka.egg-info/dependency_links.txt
 terka.egg-info/entry_points.txt
 terka.egg-info/requires.txt
 terka.egg-info/top_level.txt
-tests/__init__.py
-tests/conftest.py
-tests/test_commands.py
-tests/test_orm.py
-tests/test_task.py
-tests/test_user.py
-tests/test_utils.py
+terka/adapters/__init__.py
+terka/adapters/orm.py
+terka/adapters/repository.py
+terka/domain/__init__.py
+terka/domain/collaborators.py
+terka/domain/commands.py
+terka/domain/commentary.py
+terka/domain/element.py
+terka/domain/epic.py
+terka/domain/event_history.py
+terka/domain/helpers.py
+terka/domain/project.py
+terka/domain/sprint.py
+terka/domain/story.py
+terka/domain/tag.py
+terka/domain/task.py
+terka/domain/time_tracker.py
+terka/domain/user.py
+terka/domain/external_connectors/__init__.py
+terka/domain/external_connectors/asana.py
+terka/entrypoints/__init__.py
+terka/entrypoints/cli.py
+terka/service_layer/__init__.py
+terka/service_layer/printer.py
+terka/service_layer/services.py
+terka/service_layer/ui.py
+terka/service_layer/vertical_layout.css
+terka/service_layer/views.py
```

