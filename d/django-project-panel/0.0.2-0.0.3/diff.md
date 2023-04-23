# Comparing `tmp/django-project-panel-0.0.2.tar.gz` & `tmp/django-project-panel-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-project-panel-0.0.2.tar", last modified: Sun Apr 23 12:57:49 2023, max compression
+gzip compressed data, was "django-project-panel-0.0.3.tar", last modified: Sun Apr 23 13:24:29 2023, max compression
```

## Comparing `django-project-panel-0.0.2.tar` & `django-project-panel-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 12:57:49.834872 django-project-panel-0.0.2/
--rw-rw-rw-   0        0        0     2140 2023-04-23 12:57:49.834872 django-project-panel-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-23 12:57:49.833874 django-project-panel-0.0.2/django_project_panel.egg-info/
--rw-rw-rw-   0        0        0     2140 2023-04-23 12:57:49.000000 django-project-panel-0.0.2/django_project_panel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-04-23 12:57:49.000000 django-project-panel-0.0.2/django_project_panel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 12:57:49.000000 django-project-panel-0.0.2/django_project_panel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-23 12:57:49.000000 django-project-panel-0.0.2/django_project_panel.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 12:57:49.000000 django-project-panel-0.0.2/django_project_panel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 12:57:49.834872 django-project-panel-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1064 2023-04-23 12:56:43.000000 django-project-panel-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 13:24:29.508209 django-project-panel-0.0.3/
+-rw-rw-rw-   0        0        0     2140 2023-04-23 13:24:29.508209 django-project-panel-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-23 13:24:29.505218 django-project-panel-0.0.3/django-project-panel/
+-rw-rw-rw-   0        0        0        0 2023-04-23 13:23:20.000000 django-project-panel-0.0.3/django-project-panel/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-04-22 12:09:57.000000 django-project-panel-0.0.3/django-project-panel/admin.py
+-rw-rw-rw-   0        0        0      170 2023-04-22 12:09:57.000000 django-project-panel-0.0.3/django-project-panel/apps.py
+-rw-rw-rw-   0        0        0      742 2023-04-23 12:42:50.000000 django-project-panel-0.0.3/django-project-panel/models.py
+-rw-rw-rw-   0        0        0     5125 2023-04-23 10:46:50.000000 django-project-panel-0.0.3/django-project-panel/project_panel.py
+-rw-rw-rw-   0        0        0      246 2023-04-23 12:41:48.000000 django-project-panel-0.0.3/django-project-panel/urls.py
+-rw-rw-rw-   0        0        0     3262 2023-04-23 12:42:21.000000 django-project-panel-0.0.3/django-project-panel/views.py
+drwxrwxrwx   0        0        0        0 2023-04-23 13:24:29.507212 django-project-panel-0.0.3/django_project_panel.egg-info/
+-rw-rw-rw-   0        0        0     2140 2023-04-23 13:24:29.000000 django-project-panel-0.0.3/django_project_panel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      447 2023-04-23 13:24:29.000000 django-project-panel-0.0.3/django_project_panel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 13:24:29.000000 django-project-panel-0.0.3/django_project_panel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-23 13:24:29.000000 django-project-panel-0.0.3/django_project_panel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-23 13:24:29.000000 django-project-panel-0.0.3/django_project_panel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 13:24:29.508209 django-project-panel-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1060 2023-04-23 13:24:16.000000 django-project-panel-0.0.3/setup.py
```

### Comparing `django-project-panel-0.0.2/PKG-INFO` & `django-project-panel-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-project-panel
-Version: 0.0.2
+Version: 0.0.3
 Summary: Простая мониторинг-панель проекта (размеры всех таблиц в базе данных, медиа файлов и т.д)
 Home-page: https://github.com/EfrosiniaPetrovna/django-project-panel
 Author: EfrosiniaPetrovna
 Author-email: je.to.prace@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text
```

### Comparing `django-project-panel-0.0.2/django_project_panel.egg-info/PKG-INFO` & `django-project-panel-0.0.3/django_project_panel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-project-panel
-Version: 0.0.2
+Version: 0.0.3
 Summary: Простая мониторинг-панель проекта (размеры всех таблиц в базе данных, медиа файлов и т.д)
 Home-page: https://github.com/EfrosiniaPetrovna/django-project-panel
 Author: EfrosiniaPetrovna
 Author-email: je.to.prace@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text
```

### Comparing `django-project-panel-0.0.2/setup.py` & `django-project-panel-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 # py setup.py sdist bdist_wheel
-# py -m twine upload --repository testpypi dist/*
+# py -m twine upload --repository pypi dist/*
 
 with open("readme.txt", "r", encoding='utf-8') as fh:
 	long_description = fh.read()
 
 requirements = [
 	"psutil<=5.9.5"
 ]
 
 setuptools.setup(
 	name="django-project-panel",
-	version="0.0.2",
+	version="0.0.3",
 	author="EfrosiniaPetrovna",
 	author_email="je.to.prace@gmail.com",
 	description="Простая мониторинг-панель проекта (размеры всех таблиц в базе данных, медиа файлов и т.д)",
 	long_description=long_description,
 	long_description_content_type="text",
 	url="https://github.com/EfrosiniaPetrovna/django-project-panel",
 	packages=setuptools.find_packages(),
```

