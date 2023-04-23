# Comparing `tmp/terka-1.6.3.tar.gz` & `tmp/terka-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terka-1.6.3.tar", last modified: Mon Apr 17 20:21:09 2023, max compression
+gzip compressed data, was "terka-1.6.4.tar", last modified: Sun Apr 23 13:44:51 2023, max compression
```

## Comparing `terka-1.6.3.tar` & `terka-1.6.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-17 20:21:09.063365 terka-1.6.3/
--rw-r--r--   0 am        (1000) am        (1000)    11357 2023-04-05 21:39:45.000000 terka-1.6.3/LICENSE
--rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-17 20:21:09.063365 terka-1.6.3/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)      917 2023-03-06 22:25:53.000000 terka-1.6.3/README.md
--rw-r--r--   0 am        (1000) am        (1000)       38 2023-04-17 20:21:09.063365 terka-1.6.3/setup.cfg
--rw-r--r--   0 am        (1000) am        (1000)      890 2023-04-17 20:21:02.000000 terka-1.6.3/setup.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-17 20:21:09.055365 terka-1.6.3/src/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.3/src/__init__.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-17 20:21:09.055365 terka-1.6.3/src/adapters/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.3/src/adapters/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    15295 2023-04-12 20:19:39.000000 terka-1.6.3/src/adapters/orm.py
--rw-r--r--   0 am        (1000) am        (1000)     6136 2023-04-08 10:39:03.000000 terka-1.6.3/src/adapters/repository.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-17 20:21:09.059365 terka-1.6.3/src/domain/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.3/src/domain/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-06 18:49:11.000000 terka-1.6.3/src/domain/collaborators.py
--rw-r--r--   0 am        (1000) am        (1000)    38030 2023-04-17 14:44:32.000000 terka-1.6.3/src/domain/commands.py
--rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-12 20:16:29.000000 terka-1.6.3/src/domain/commentary.py
--rw-r--r--   0 am        (1000) am        (1000)      102 2023-01-26 19:46:39.000000 terka-1.6.3/src/domain/element.py
--rw-r--r--   0 am        (1000) am        (1000)      959 2023-04-08 10:39:03.000000 terka-1.6.3/src/domain/epic.py
--rw-r--r--   0 am        (1000) am        (1000)     1440 2023-03-12 20:44:34.000000 terka-1.6.3/src/domain/event_history.py
--rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.6.3/src/domain/helpers.py
--rw-r--r--   0 am        (1000) am        (1000)      892 2023-03-17 11:37:47.000000 terka-1.6.3/src/domain/project.py
--rw-r--r--   0 am        (1000) am        (1000)     2177 2023-04-15 18:25:02.000000 terka-1.6.3/src/domain/sprint.py
--rw-r--r--   0 am        (1000) am        (1000)      965 2023-04-08 10:39:03.000000 terka-1.6.3/src/domain/story.py
--rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-06 19:04:21.000000 terka-1.6.3/src/domain/tag.py
--rw-r--r--   0 am        (1000) am        (1000)     2039 2023-04-07 19:10:02.000000 terka-1.6.3/src/domain/task.py
--rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-08 10:39:03.000000 terka-1.6.3/src/domain/time_tracker.py
--rw-r--r--   0 am        (1000) am        (1000)      792 2023-01-26 19:46:39.000000 terka-1.6.3/src/domain/user.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-17 20:21:09.059365 terka-1.6.3/src/entrypoints/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-02-11 17:56:56.000000 terka-1.6.3/src/entrypoints/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)     5069 2023-04-17 20:19:14.000000 terka-1.6.3/src/entrypoints/cli.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-17 20:21:09.059365 terka-1.6.3/src/service_layer/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.3/src/service_layer/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    26602 2023-04-17 20:07:43.000000 terka-1.6.3/src/service_layer/printer.py
--rw-r--r--   0 am        (1000) am        (1000)     2918 2023-04-11 15:29:13.000000 terka-1.6.3/src/service_layer/services.py
--rw-r--r--   0 am        (1000) am        (1000)     3882 2023-02-12 14:00:44.000000 terka-1.6.3/src/service_layer/ui.py
--rw-r--r--   0 am        (1000) am        (1000)      698 2023-02-12 13:59:50.000000 terka-1.6.3/src/service_layer/vertical_layout.css
--rw-r--r--   0 am        (1000) am        (1000)      529 2023-04-17 20:19:26.000000 terka-1.6.3/src/service_layer/views.py
--rw-r--r--   0 am        (1000) am        (1000)     7617 2023-04-16 08:47:06.000000 terka-1.6.3/src/utils.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-17 20:21:09.059365 terka-1.6.3/terka.egg-info/
--rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-17 20:21:09.000000 terka-1.6.3/terka.egg-info/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)     1003 2023-04-17 20:21:09.000000 terka-1.6.3/terka.egg-info/SOURCES.txt
--rw-r--r--   0 am        (1000) am        (1000)        1 2023-04-17 20:21:09.000000 terka-1.6.3/terka.egg-info/dependency_links.txt
--rw-r--r--   0 am        (1000) am        (1000)       51 2023-04-17 20:21:09.000000 terka-1.6.3/terka.egg-info/entry_points.txt
--rw-r--r--   0 am        (1000) am        (1000)       52 2023-04-17 20:21:09.000000 terka-1.6.3/terka.egg-info/requires.txt
--rw-r--r--   0 am        (1000) am        (1000)       10 2023-04-17 20:21:09.000000 terka-1.6.3/terka.egg-info/top_level.txt
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-17 20:21:09.063365 terka-1.6.3/tests/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.3/tests/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      424 2023-01-26 19:46:39.000000 terka-1.6.3/tests/conftest.py
--rw-r--r--   0 am        (1000) am        (1000)       43 2023-01-26 19:46:39.000000 terka-1.6.3/tests/test_commands.py
--rw-r--r--   0 am        (1000) am        (1000)     2818 2023-01-26 19:46:39.000000 terka-1.6.3/tests/test_orm.py
--rw-r--r--   0 am        (1000) am        (1000)      956 2023-01-26 19:46:39.000000 terka-1.6.3/tests/test_task.py
--rw-r--r--   0 am        (1000) am        (1000)     1281 2023-01-26 19:46:39.000000 terka-1.6.3/tests/test_user.py
--rw-r--r--   0 am        (1000) am        (1000)      265 2023-01-26 19:46:39.000000 terka-1.6.3/tests/test_utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:44:51.492537 terka-1.6.4/
+-rw-r--r--   0 am        (1000) am        (1000)    11357 2023-04-05 21:39:45.000000 terka-1.6.4/LICENSE
+-rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-23 13:44:51.492537 terka-1.6.4/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)      917 2023-03-06 22:25:53.000000 terka-1.6.4/README.md
+-rw-r--r--   0 am        (1000) am        (1000)       38 2023-04-23 13:44:51.492537 terka-1.6.4/setup.cfg
+-rw-r--r--   0 am        (1000) am        (1000)      890 2023-04-23 13:44:41.000000 terka-1.6.4/setup.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:44:51.488535 terka-1.6.4/src/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4/src/__init__.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:44:51.488535 terka-1.6.4/src/adapters/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4/src/adapters/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    16059 2023-04-23 13:38:52.000000 terka-1.6.4/src/adapters/orm.py
+-rw-r--r--   0 am        (1000) am        (1000)     6139 2023-04-19 21:12:52.000000 terka-1.6.4/src/adapters/repository.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:44:51.488535 terka-1.6.4/src/domain/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4/src/domain/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-06 18:49:11.000000 terka-1.6.4/src/domain/collaborators.py
+-rw-r--r--   0 am        (1000) am        (1000)    41043 2023-04-23 13:40:04.000000 terka-1.6.4/src/domain/commands.py
+-rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-12 20:16:29.000000 terka-1.6.4/src/domain/commentary.py
+-rw-r--r--   0 am        (1000) am        (1000)      102 2023-01-26 19:46:39.000000 terka-1.6.4/src/domain/element.py
+-rw-r--r--   0 am        (1000) am        (1000)      959 2023-04-08 10:39:03.000000 terka-1.6.4/src/domain/epic.py
+-rw-r--r--   0 am        (1000) am        (1000)     1440 2023-03-12 20:44:34.000000 terka-1.6.4/src/domain/event_history.py
+-rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.6.4/src/domain/helpers.py
+-rw-r--r--   0 am        (1000) am        (1000)      892 2023-03-17 11:37:47.000000 terka-1.6.4/src/domain/project.py
+-rw-r--r--   0 am        (1000) am        (1000)     2177 2023-04-15 18:25:02.000000 terka-1.6.4/src/domain/sprint.py
+-rw-r--r--   0 am        (1000) am        (1000)      965 2023-04-08 10:39:03.000000 terka-1.6.4/src/domain/story.py
+-rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-06 19:04:21.000000 terka-1.6.4/src/domain/tag.py
+-rw-r--r--   0 am        (1000) am        (1000)     2039 2023-04-07 19:10:02.000000 terka-1.6.4/src/domain/task.py
+-rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-08 10:39:03.000000 terka-1.6.4/src/domain/time_tracker.py
+-rw-r--r--   0 am        (1000) am        (1000)      792 2023-01-26 19:46:39.000000 terka-1.6.4/src/domain/user.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:44:51.488535 terka-1.6.4/src/entrypoints/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-02-11 17:56:56.000000 terka-1.6.4/src/entrypoints/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)     5069 2023-04-23 13:13:52.000000 terka-1.6.4/src/entrypoints/cli.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:44:51.492537 terka-1.6.4/src/service_layer/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4/src/service_layer/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    27272 2023-04-23 12:13:55.000000 terka-1.6.4/src/service_layer/printer.py
+-rw-r--r--   0 am        (1000) am        (1000)     2918 2023-04-11 15:29:13.000000 terka-1.6.4/src/service_layer/services.py
+-rw-r--r--   0 am        (1000) am        (1000)     3882 2023-02-12 14:00:44.000000 terka-1.6.4/src/service_layer/ui.py
+-rw-r--r--   0 am        (1000) am        (1000)      698 2023-02-12 13:59:50.000000 terka-1.6.4/src/service_layer/vertical_layout.css
+-rw-r--r--   0 am        (1000) am        (1000)     1441 2023-04-23 13:10:22.000000 terka-1.6.4/src/service_layer/views.py
+-rw-r--r--   0 am        (1000) am        (1000)     7743 2023-04-23 13:28:15.000000 terka-1.6.4/src/utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:44:51.492537 terka-1.6.4/terka.egg-info/
+-rw-r--r--   0 am        (1000) am        (1000)     1232 2023-04-23 13:44:51.000000 terka-1.6.4/terka.egg-info/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)     1003 2023-04-23 13:44:51.000000 terka-1.6.4/terka.egg-info/SOURCES.txt
+-rw-r--r--   0 am        (1000) am        (1000)        1 2023-04-23 13:44:51.000000 terka-1.6.4/terka.egg-info/dependency_links.txt
+-rw-r--r--   0 am        (1000) am        (1000)       51 2023-04-23 13:44:51.000000 terka-1.6.4/terka.egg-info/entry_points.txt
+-rw-r--r--   0 am        (1000) am        (1000)       52 2023-04-23 13:44:51.000000 terka-1.6.4/terka.egg-info/requires.txt
+-rw-r--r--   0 am        (1000) am        (1000)       10 2023-04-23 13:44:51.000000 terka-1.6.4/terka.egg-info/top_level.txt
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-04-23 13:44:51.492537 terka-1.6.4/tests/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-01-26 19:46:39.000000 terka-1.6.4/tests/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      424 2023-01-26 19:46:39.000000 terka-1.6.4/tests/conftest.py
+-rw-r--r--   0 am        (1000) am        (1000)       43 2023-01-26 19:46:39.000000 terka-1.6.4/tests/test_commands.py
+-rw-r--r--   0 am        (1000) am        (1000)     2818 2023-01-26 19:46:39.000000 terka-1.6.4/tests/test_orm.py
+-rw-r--r--   0 am        (1000) am        (1000)      956 2023-01-26 19:46:39.000000 terka-1.6.4/tests/test_task.py
+-rw-r--r--   0 am        (1000) am        (1000)     1281 2023-01-26 19:46:39.000000 terka-1.6.4/tests/test_user.py
+-rw-r--r--   0 am        (1000) am        (1000)      265 2023-01-26 19:46:39.000000 terka-1.6.4/tests/test_utils.py
```

### Comparing `terka-1.6.3/LICENSE` & `terka-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `terka-1.6.3/PKG-INFO` & `terka-1.6.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terka
-Version: 1.6.3
+Version: 1.6.4
 Summary: CLI utility for creating and managing tasks in a terminal
 Home-page: https://github.com/AndreyMarkinPPC/terka
 Author: Andrei Markin
 Author-email: andrey.markin.ppc@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `terka-1.6.3/README.md` & `terka-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `terka-1.6.3/setup.py` & `terka-1.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(
     name="terka",
-    version="1.6.3",
+    version="1.6.4",
     description="CLI utility for creating and managing tasks in a terminal",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Andrei Markin",
     author_email="andrey.markin.ppc@gmail.com",
     license="Apache 2.0",
     url="https://github.com/AndreyMarkinPPC/terka",
```

### Comparing `terka-1.6.3/src/adapters/orm.py` & `terka-1.6.4/src/adapters/orm.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 from src.domain.tag import BaseTag, TaskTag, ProjectTag
 from src.domain.collaborators import TaskCollaborator, ProjectCollaborator
 from src.domain.sprint import Sprint, SprintStatus, SprintTask
 from src.domain.time_tracker import TimeTrackerEntry
 from src.domain.epic import Epic, EpicTask
 from src.domain.story import Story, StoryTask
 
+from src.domain.external_connectors.asana import AsanaTask, AsanaProject
+
 Base = declarative_base()
 metadata = MetaData()
 
 tasks = Table("tasks", metadata,
               Column("id", Integer, primary_key=True, autoincrement=True),
               Column("name", String(255)),
               Column("creation_date", DateTime, nullable=True),
@@ -214,16 +216,30 @@
 # class SprintTasks(Base):
 #     __tablename__ = "sprint_tasks"
 #     id = Integer(primary_key=True, autoincrement=True)
 #     task_id = Integer(nullable=False)
 #     sprint_id = Integer(nullable=False)
 #     ta
 
+asana_tasks = Table(
+    "external_connectors.asana.tasks", metadata,
+    # Column("id", Integer, primary_key=True, autoincrement=True),
+    Column("project", ForeignKey("projects.id")),
+    Column("id", ForeignKey("tasks.id"), nullable=False, primary_key=True),
+    Column("asana_task_id", String(20)))
+
+asana_projects = Table(
+    "external_connectors.asana.projects", metadata,
+    # Column("id", Integer, primary_key=True, autoincrement=True),
+    Column("id", ForeignKey("projects.id"), nullable=False, primary_key=True),
+    Column("asana_project_id", String(20)))
 
 def start_mappers():
+    asana_task_mapper = mapper(AsanaTask, asana_tasks)
+    asana_project_mapper = mapper(AsanaProject, asana_projects)
     task_commentary_mapper = mapper(TaskCommentary, task_commentaries)
     project_commentary_mapper = mapper(ProjectCommentary, project_commentaries)
     epic_commentary_mapper = mapper(EpicCommentary, epic_commentaries)
     story_commentary_mapper = mapper(StoryCommentary, story_commentaries)
     sprint_commentary_mapper = mapper(SprintCommentary, sprint_commentaries)
     task_event_mapper = mapper(TaskEvent, task_events)
     project_event_mapper = mapper(ProjectEvent, project_events)
```

### Comparing `terka-1.6.3/src/adapters/repository.py` & `terka-1.6.4/src/adapters/repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,8 +143,8 @@
     def _add(self, element):
         self.session.add(element)
 
     def _get(self, element, element_name):
         return self.session.query(element).filter_by(name=element_name).first()
 
     def _get_by_element_id(self, element, element_id):
-        return (self.session.query(element).filter(id=element_id).first())
+        return (self.session.query(element).filter_by(id=element_id).first())
```

### Comparing `terka-1.6.3/src/domain/collaborators.py` & `terka-1.6.4/src/domain/collaborators.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.3/src/domain/commands.py` & `terka-1.6.4/src/domain/commands.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,42 +20,58 @@
 from src.domain.tag import BaseTag, TaskTag, ProjectTag
 from src.domain.collaborators import TaskCollaborator, ProjectCollaborator
 from src.domain.event_history import TaskEvent, ProjectEvent
 from src.domain.sprint import Sprint, SprintTask
 from src.domain.time_tracker import TimeTrackerEntry
 from src.domain.epic import Epic, EpicTask
 from src.domain.story import Story, StoryTask
+from src.domain.external_connectors.asana import AsanaTask, AsanaProject
 
 from src.service_layer import services, printer
 from src.service_layer.ui import TerkaTask
 from src.adapters.repository import AbsRepository
 from src.utils import format_command, format_task_dict
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class CurrentEntry:
     value: str
     type: str
+    source: str = None
 
 
 def generate_message_template(current_entry: CurrentEntry, task: Task,
                               repo) -> str:
-    project = services.lookup_project_name(task.project, repo)
-    message_template = f"""
-    # You are editing {current_entry.type}, enter below:
-    {current_entry.value}
-    ---
-    Task context:
-    id: {task.id}
-    name: {task.name}
-    description: {task.description}
-    project: {project.name}
-    """
+    if isinstance(task, (Task, Story, Epic)):
+        project = services.lookup_project_name(task.project, repo)
+        project_name = project.name
+    elif isinstance(task, Project):
+        project_name = task.name
+    if current_entry.source == "sprints":
+        message_template = f"""
+        # You are editing {current_entry.type}, enter below:
+        {current_entry.value}
+        ---
+        {current_entry.source} context:
+        id: {task.id}
+        goal: {task.goal}
+        """
+    else:
+        message_template = f"""
+        # You are editing {current_entry.type}, enter below:
+        {current_entry.value}
+        ---
+        {current_entry.source} context:
+        id: {task.id}
+        name: {task.name}
+        description: {task.description}
+        project: {project_name}
+        """
     return re.sub("\n +", "\n", message_template.lstrip())
 
 
 class BaseHandler:
 
     def __init__(self, successor) -> None:
         self._successor = successor
@@ -553,16 +569,28 @@
                 self.repo.add(obj)
                 session.commit()
         elif command == "delete":
             if entity not in (Task, ):
                 raise ValueError("'delete' operation only allowed for tasks!")
             task_ids = get_ids(kwargs.get("id"))
             for task_id in task_ids:
-                if not self.repo.list(Task, {"id": task_id}):
+                if not (task := self.repo.get_by_id(Task, task_id)):
                     exit(f"Task id {task_id} is not found")
+                else:
+                    if all(key == "id" for key in kwargs.keys()):
+                        deletion_reason = input(
+                            f"Provide brief explanation why you're deleting task <{task_id}>: "
+                        )
+                        if deletion_reason:
+                            self.execute("comment", "tasks", {
+                                "id": task_id,
+                                "text": deletion_reason
+                            })
+                        kwargs.update({"status": "DELETED"})
+                        self.execute("update", entity_type, kwargs)
                 if epic_id := kwargs.get("epic_id"):
                     epic = self.repo.list(Epic, {"id": epic_id})
                     if not epic:
                         exit(f"Epic id {epic_id} is not found")
                     if not (epic_task := self.repo.list(
                             EpicTask, {
                                 "task": task_id,
@@ -591,20 +619,44 @@
                             SprintTask, {
                                 "task": task_id,
                                 "sprint": sprint_id
                             })):
                         exit("task is not in sprint")
                     self.repo.delete(SprintTask, sprint_task[0].id)
             session.commit()
+        elif command == "connect":
+            if entity not in (Task, Project):
+                raise ValueError("'connect' operation only allowed for tasks and project!")
+            task_ids = get_ids(kwargs.get("id"))
+            for task_id in task_ids:
+                if entity_type == "projects":
+                    asana_project_id = kwargs.get("external_project")
+                    asana_project = self.repo.get_by_id(AsanaProject, task_id)
+                    breakpoint()
+                    if not asana_project:
+                        obj = AsanaProject(id=task_id, asana_project_id=asana_project_id)
+                        breakpoint()
+                        self.repo.add(obj)
+                    else:
+                        self.repo.update(AsanaProject, task_id, {"asana_project_id": asana_project_id})
+                elif entity_type == "tasks":
+                    asana_task_id = kwargs.get("external_task")
+                    asana_task = self.repo.get_by_id(AsanaProject, task_id)
+                    if not asana_task:
+                        obj = AsanaTask(project=task.project, id=task_id, asana_task_id=kwargs.get("external_task"))
+                        self.repo.add(obj)
+                    else:
+                        self.repo.update(AsanaTask, task_id, {"asana_task_id": asana_task_id})
+            self.repo.session.commit()
         elif command == "add":
             if entity not in (Task, ):
                 raise ValueError("'add' operation only allowed for tasks!")
             task_ids = get_ids(kwargs.get("id"))
             for task_id in task_ids:
-                if not self.repo.list(Task, {"id": task_id}):
+                if not (added_task := self.repo.get_by_id(Task, task_id)):
                     exit(f"Task id {task_id} is not found")
 
                 if epic_id := kwargs.get("epic_id"):
                     epic = self.repo.list(Epic, {"id": epic_id})
                     if not epic:
                         exit(f"Epic id {epic_id} is not found")
                     obj = EpicTask(task=task_id, epic=epic_id)
@@ -622,31 +674,38 @@
                     if self.repo.list(StoryTask, {
                             "task": obj.task,
                             "story": obj.story
                     }):
                         exit("task already added to story")
                     self.repo.add(obj)
                 if sprint_id := kwargs.get("sprint_id"):
-                    sprint = self.repo.list(Sprint, {"id": sprint_id})
+                    sprint = self.repo.get_by_id(Sprint, sprint_id)
                     if not sprint:
                         exit(f"Sprint id {sprint_id} is not found")
-                    if sprint[0].status.name == "COMPLETED":
+                    if sprint.status.name == "COMPLETED":
                         exit("Cannot add task to a finished sprint")
                     obj = SprintTask(task=task_id,
                                      sprint=sprint_id,
                                      is_active_link=True)
                     if self.repo.list(SprintTask, {
                             "task": obj.task,
                             "sprint": obj.sprint
                     }):
                         exit("task already added to sprint")
                     self.repo.add(obj)
                     sprint_task_id = obj.id
                 else:
                     sprint_task_id = None
+                # Update task status and due date
+                task_params = {"id": added_task.id}
+                if added_task.status.name == "BACKLOG":
+                    task_params.update({"status": "TODO"})
+                if not added_task.due_date or added_task.due_date > sprint.end_date:
+                    task_params.update({"due_date": sprint.end_date})
+                self.execute("update", "tasks", task_params)
                 if story_points := kwargs.get("story_points"):
                     if not sprint_task_id:
                         sprint_task = self.execute("get", "sprint_tasks",
                                                    {"task": task_id})
                         if not sprint_task:
                             exit(
                                 f"Task id {task_id} is not part of any sprint")
@@ -724,44 +783,42 @@
                             print(
                                 "No changes were proposed to the existing entity"
                             )
                     session.commit()
                 return entity, None
             else:
                 raise ValueError("No task_id is provided")
-        elif command == "delete":
-            kwargs.update({"status": "DELETED"})
-            self.execute("update", entity_type, kwargs)
-            logger.info("<delete> %s", entity_type)
-            return entity, None
         elif command == "edit":
             if (task_id := kwargs.get("id")):
                 tasks = get_ids(task_id)
                 for task in tasks:
                     if task.isdigit():
-                        entities = self.repo.list(entity, {"id": task})
+                        entities = self.repo.get_by_id(entity, task)
                         task_id = task
                     else:
-                        entities = self.repo.list(entity, {"name": task})
-                        task_id = entities[0].id
-                    if entity_type == "tasks":
-                        task = entities[0]
+                        entities = self.repo.get(entity, task)
+                        task_id = entities.id
+                    if entity_type in ("tasks", "projects", "sprints", "epics", "stories"):
+                        task = entities
                         if kwargs.get("description"):
                             current_entry = task.description
                             current_type = "description"
                         elif kwargs.get("name"):
                             current_entry = task.name
                             current_type = "name"
+                        elif kwargs.get("goal"):
+                            current_entry = task.goal
+                            current_type = "goal"
                         else:
                             raise ValueError(
                                 "Either name or description should be specified!"
                             )
 
                     message_template = generate_message_template(
-                        CurrentEntry(current_entry, current_type), task,
+                        CurrentEntry(current_entry, current_type, entity_type), task,
                         self.repo)
                     with tempfile.NamedTemporaryFile(suffix=".tmp") as tf:
                         tf.write(message_template.encode("utf-8"))
                         tf.flush()
                         run(["vim", "+2", tf.name])
                         tf.seek(0)
                         new_entry = tf.read()
```

### Comparing `terka-1.6.3/src/domain/commentary.py` & `terka-1.6.4/src/domain/commentary.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.3/src/domain/epic.py` & `terka-1.6.4/src/domain/epic.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.3/src/domain/event_history.py` & `terka-1.6.4/src/domain/event_history.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.3/src/domain/project.py` & `terka-1.6.4/src/domain/project.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.3/src/domain/sprint.py` & `terka-1.6.4/src/domain/sprint.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.3/src/domain/story.py` & `terka-1.6.4/src/domain/story.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.3/src/domain/tag.py` & `terka-1.6.4/src/domain/tag.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.3/src/domain/task.py` & `terka-1.6.4/src/domain/task.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.3/src/domain/time_tracker.py` & `terka-1.6.4/src/domain/time_tracker.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.3/src/domain/user.py` & `terka-1.6.4/src/domain/user.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.3/src/entrypoints/cli.py` & `terka-1.6.4/src/entrypoints/cli.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.3/src/service_layer/printer.py` & `terka-1.6.4/src/service_layer/printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -293,29 +293,40 @@
         plt.bar(dates, times)
         plt.show()
 
     def print_project(self, entities, print_options, kwargs=None):
         table = Table(box=rich.box.SQUARE_DOUBLE_HEAD, expand=True)
         non_active_projects = Table(box=rich.box.SQUARE_DOUBLE_HEAD)
         for column in ("id", "name", "description", "status", "open_tasks",
-                       "overdue", "backlog", "todo", "in_progress", "review",
-                       "done", "median_task_age"):
+                       "overdue", "stale", "backlog", "todo", "in_progress",
+                       "review", "done", "median_task_age"):
             table.add_column(column)
         for column in ("id", "name", "description", "status", "open_tasks"):
             non_active_projects.add_column(column)
         for entity in entities:
             # if entity.status.name != "ACTIVE":
             #     continue
             open_tasks = self._sort_open_tasks(entity)
             if open_tasks > 0 and entity.status.name == "ACTIVE":
                 overdue_tasks = [
                     task for task in entity.tasks
                     if task.due_date and task.due_date <= datetime.now().date(
                     ) and task.status.name not in ("DELETED", "DONE")
                 ]
+                stale_tasks = []
+                for task in entity.tasks:
+                    if (event_history :=
+                            task.history) and task.status.name in (
+                                "TODO", "IN_PROGRESS", "REVIEW"):
+                        for event in event_history:
+                            if max([
+                                    event.date for event in event_history
+                            ]) < (datetime.today() - timedelta(days=5)):
+                                stale_tasks.append(task)
+                stale_tasks = list(set(stale_tasks))
                 median_task_age = round(
                     median([(datetime.now() - task.creation_date).days
                             for task in entity.tasks
                             if task.status.name not in ("DELETED", "DONE")]))
                 backlog = self._count_task_status(entity.tasks, "BACKLOG")
                 todo = self._count_task_status(entity.tasks, "TODO")
                 in_progress = self._count_task_status(entity.tasks,
@@ -325,17 +336,17 @@
 
                 if overdue_tasks:
                     entity_id = f"[red]{entity.id}[/red]"
                 else:
                     entity_id = f"[green]{entity.id}[/green]"
                 table.add_row(f"{entity_id}", entity.name, entity.description,
                               entity.status.name, str(open_tasks),
-                              str(len(overdue_tasks)), str(backlog), str(todo),
-                              str(in_progress), str(review), str(done),
-                              str(median_task_age))
+                              str(len(overdue_tasks)), str(len(stale_tasks)),
+                              str(backlog), str(todo), str(in_progress),
+                              str(review), str(done), str(median_task_age))
             else:
                 non_active_projects.add_row(str(entity.id), entity.name,
                                             entity.description,
                                             entity.status.name,
                                             str(open_tasks))
 
         if table.row_count:
@@ -417,20 +428,14 @@
                 repo=repo,
                 story_points=completed_story_points,
                 show_window=show_window,
                 all_tasks=False)
             if table.row_count:
                 self.console.print(f"[green]****COMPLETED TASKS*****[/green]")
                 self.console.print(table)
-        # TODO: not working
-        if print_options.show_commentaries and (commentaries :=
-                                                entity.commentaries):
-            self.print_commentaries(commentaries)
-        if print_options.show_history and (history := entity.history):
-            self.print_history(history)
 
     def _get_attributes(self, obj) -> List[Tuple[str, str]]:
         import inspect
         attributes = []
         for name, value in inspect.getmembers(obj):
             if not name.startswith("_") and not inspect.ismethod(value):
                 if not value:
@@ -601,8 +606,15 @@
                               collaborator_string, str(time_spent))
         if table.row_count == 1 and show_window:
             app = TerkaTask(entity=entity,
                             project=project,
                             history=history,
                             commentaries=comments)
             app.run()
+        # # TODO: not working
+        # if print_options.show_commentaries and (commentaries :=
+        #                                         entity.commentaries):
+        #     self.print_commentaries(commentaries)
+        # # TODO: not working
+        # if print_options.show_history and (history := entity.history):
+        #     self.print_history(history)
         return table, completed_tasks, completed_story_points
```

### Comparing `terka-1.6.3/src/service_layer/services.py` & `terka-1.6.4/src/service_layer/services.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.3/src/service_layer/ui.py` & `terka-1.6.4/src/service_layer/ui.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.3/src/service_layer/vertical_layout.css` & `terka-1.6.4/src/service_layer/vertical_layout.css`

 * *Files identical despite different names*

### Comparing `terka-1.6.3/src/utils.py` & `terka-1.6.4/src/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,14 +73,16 @@
             "hours": new_dict.get("H"),
             "minutes": new_dict.get("M"),
             "show_history": new_dict.get("show-history"),
             "show_commentaries": new_dict.get("show-commentaries") or new_dict.get("show-comments"),
             "epics": new_dict.get("epics"),
             "stories": new_dict.get("stories"),
             "tasks": new_dict.get("tasks"),
+            "external_project": new_dict.get("external-project"),
+            "external_task": new_dict.get("external-task"),
         }
         if "--show-completed" in kwargs:
             task_dict.update({"show_completed": True})
         if "--sort" in kwargs:
             sort_statement = kwargs[kwargs.index("--sort"):]
             task_dict.update(create_task_dict(sort_statement))
     elif len(kwargs) == 1:
```

### Comparing `terka-1.6.3/terka.egg-info/PKG-INFO` & `terka-1.6.4/terka.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terka
-Version: 1.6.3
+Version: 1.6.4
 Summary: CLI utility for creating and managing tasks in a terminal
 Home-page: https://github.com/AndreyMarkinPPC/terka
 Author: Andrei Markin
 Author-email: andrey.markin.ppc@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `terka-1.6.3/terka.egg-info/SOURCES.txt` & `terka-1.6.4/terka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `terka-1.6.3/tests/test_orm.py` & `terka-1.6.4/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.3/tests/test_task.py` & `terka-1.6.4/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `terka-1.6.3/tests/test_user.py` & `terka-1.6.4/tests/test_user.py`

 * *Files identical despite different names*

