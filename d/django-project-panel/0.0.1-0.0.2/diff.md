# Comparing `tmp/django-project-panel-0.0.1.tar.gz` & `tmp/django-project-panel-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-project-panel-0.0.1.tar", last modified: Sun Apr 23 12:46:42 2023, max compression
+gzip compressed data, was "django-project-panel-0.0.2.tar", last modified: Sun Apr 23 12:57:49 2023, max compression
```

## Comparing `django-project-panel-0.0.1.tar` & `django-project-panel-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 12:46:42.109105 django-project-panel-0.0.1/
--rw-rw-rw-   0        0        0     2140 2023-04-23 12:46:42.109105 django-project-panel-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-23 12:46:42.108106 django-project-panel-0.0.1/django_project_panel.egg-info/
--rw-rw-rw-   0        0        0     2140 2023-04-23 12:46:42.000000 django-project-panel-0.0.1/django_project_panel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-04-23 12:46:42.000000 django-project-panel-0.0.1/django_project_panel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 12:46:42.000000 django-project-panel-0.0.1/django_project_panel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-23 12:46:42.000000 django-project-panel-0.0.1/django_project_panel.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 12:46:42.000000 django-project-panel-0.0.1/django_project_panel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 12:46:42.109105 django-project-panel-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1064 2023-04-23 12:46:26.000000 django-project-panel-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 12:57:49.834872 django-project-panel-0.0.2/
+-rw-rw-rw-   0        0        0     2140 2023-04-23 12:57:49.834872 django-project-panel-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-23 12:57:49.833874 django-project-panel-0.0.2/django_project_panel.egg-info/
+-rw-rw-rw-   0        0        0     2140 2023-04-23 12:57:49.000000 django-project-panel-0.0.2/django_project_panel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-04-23 12:57:49.000000 django-project-panel-0.0.2/django_project_panel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 12:57:49.000000 django-project-panel-0.0.2/django_project_panel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-23 12:57:49.000000 django-project-panel-0.0.2/django_project_panel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 12:57:49.000000 django-project-panel-0.0.2/django_project_panel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 12:57:49.834872 django-project-panel-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1064 2023-04-23 12:56:43.000000 django-project-panel-0.0.2/setup.py
```

### Comparing `django-project-panel-0.0.1/PKG-INFO` & `django-project-panel-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-project-panel
-Version: 0.0.1
+Version: 0.0.2
 Summary: Простая мониторинг-панель проекта (размеры всех таблиц в базе данных, медиа файлов и т.д)
 Home-page: https://github.com/EfrosiniaPetrovna/django-project-panel
 Author: EfrosiniaPetrovna
 Author-email: je.to.prace@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text
```

### Comparing `django-project-panel-0.0.1/django_project_panel.egg-info/PKG-INFO` & `django-project-panel-0.0.2/django_project_panel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-project-panel
-Version: 0.0.1
+Version: 0.0.2
 Summary: Простая мониторинг-панель проекта (размеры всех таблиц в базе данных, медиа файлов и т.д)
 Home-page: https://github.com/EfrosiniaPetrovna/django-project-panel
 Author: EfrosiniaPetrovna
 Author-email: je.to.prace@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text
```

### Comparing `django-project-panel-0.0.1/setup.py` & `django-project-panel-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 requirements = [
 	"psutil<=5.9.5"
 ]
 
 setuptools.setup(
 	name="django-project-panel",
-	version="0.0.1",
+	version="0.0.2",
 	author="EfrosiniaPetrovna",
 	author_email="je.to.prace@gmail.com",
 	description="Простая мониторинг-панель проекта (размеры всех таблиц в базе данных, медиа файлов и т.д)",
 	long_description=long_description,
 	long_description_content_type="text",
 	url="https://github.com/EfrosiniaPetrovna/django-project-panel",
 	packages=setuptools.find_packages(),
```

