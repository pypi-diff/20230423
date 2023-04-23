# Comparing `tmp/drf_nested_browsable-0.1.0.tar.gz` & `tmp/drf_nested_browsable-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_nested_browsable-0.1.0.tar", max compression
+gzip compressed data, was "drf_nested_browsable-0.1.1.tar", max compression
```

## Comparing `drf_nested_browsable-0.1.0.tar` & `drf_nested_browsable-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1332 2023-04-23 11:15:15.887977 drf_nested_browsable-0.1.0/README.md
--rw-r--r--   0        0        0      213 2023-04-23 08:13:02.976124 drf_nested_browsable-0.1.0/drf_nested_browsable/__init__.py
--rw-r--r--   0        0        0     4385 2023-04-23 08:23:30.043605 drf_nested_browsable-0.1.0/drf_nested_browsable/serializers.py
--rw-r--r--   0        0        0     3107 2023-04-23 08:30:02.544106 drf_nested_browsable-0.1.0/drf_nested_browsable/templates/writable_list.html
--rw-r--r--   0        0        0        0 2023-04-21 13:53:21.631214 drf_nested_browsable-0.1.0/drf_nested_browsable/templatetags/__init__.py
--rw-r--r--   0        0        0     1338 2023-04-23 11:12:11.747713 drf_nested_browsable-0.1.0/drf_nested_browsable/templatetags/drf_nested_browsable.py
--rw-r--r--   0        0        0      748 2023-04-23 09:42:25.338489 drf_nested_browsable-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2151 1970-01-01 00:00:00.000000 drf_nested_browsable-0.1.0/setup.py
--rw-r--r--   0        0        0     1891 1970-01-01 00:00:00.000000 drf_nested_browsable-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1332 2023-04-23 11:15:15.887977 drf_nested_browsable-0.1.1/README.md
+-rw-r--r--   0        0        0      213 2023-04-23 08:13:02.976124 drf_nested_browsable-0.1.1/drf_nested_browsable/__init__.py
+-rw-r--r--   0        0        0     4385 2023-04-23 08:23:30.043605 drf_nested_browsable-0.1.1/drf_nested_browsable/serializers.py
+-rw-r--r--   0        0        0     3107 2023-04-23 08:30:02.544106 drf_nested_browsable-0.1.1/drf_nested_browsable/templates/writable_list.html
+-rw-r--r--   0        0        0        0 2023-04-21 13:53:21.631214 drf_nested_browsable-0.1.1/drf_nested_browsable/templatetags/__init__.py
+-rw-r--r--   0        0        0     1338 2023-04-23 11:12:11.747713 drf_nested_browsable-0.1.1/drf_nested_browsable/templatetags/drf_nested_browsable.py
+-rw-r--r--   0        0        0     1099 2023-04-23 11:50:03.947558 drf_nested_browsable-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2211 1970-01-01 00:00:00.000000 drf_nested_browsable-0.1.1/setup.py
+-rw-r--r--   0        0        0     2231 1970-01-01 00:00:00.000000 drf_nested_browsable-0.1.1/PKG-INFO
```

### Comparing `drf_nested_browsable-0.1.0/README.md` & `drf_nested_browsable-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `drf_nested_browsable-0.1.0/drf_nested_browsable/serializers.py` & `drf_nested_browsable-0.1.1/drf_nested_browsable/serializers.py`

 * *Files identical despite different names*

### Comparing `drf_nested_browsable-0.1.0/drf_nested_browsable/templates/writable_list.html` & `drf_nested_browsable-0.1.1/drf_nested_browsable/templates/writable_list.html`

 * *Files identical despite different names*

### Comparing `drf_nested_browsable-0.1.0/drf_nested_browsable/templatetags/drf_nested_browsable.py` & `drf_nested_browsable-0.1.1/drf_nested_browsable/templatetags/drf_nested_browsable.py`

 * *Files identical despite different names*

### Comparing `drf_nested_browsable-0.1.0/setup.py` & `drf_nested_browsable-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 {'': ['*'], 'drf_nested_browsable': ['templates/*']}
 
 install_requires = \
 ['django>=4.2,<5.0', 'djangorestframework>=3.14.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'drf-nested-browsable',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Writable nested serializers with forms for the Browsable API',
     'long_description': ":warning: Work In Progress :warning:\n\n# Writable Nested Serializers with Browsable API Forms\n\nThis plugin is intended to provide writable nested serializers (similar to [the recommended plugin from DRF documentation](https://github.com/beda-software/drf-nested-browsable.git)) that bring their own forms for the Browsable API renderer.\n\n## Try it out\n\nThis project's dependencies are managed using [`poetry`](https://python-poetry.org/)\n\n```bash\ngit clone https://github.com/pcouy/drf-nested-browsable\ncd drf-nested-browsable\npoetry install\ncd example\npython manage.py migrate\npython manage.py runserver\n```\n\nThe above commands will install the dependencies, run the DB migrations, and launch a development server of the example project that uses the provided serializers.\n\n## Current state of the project\n\n### Done\n\n* Ability to write to a reverse `ForeignKey` relationship using serializer `Meta` class\n* Dynamic form for `WritableNestedListSerializer` that allows adding and removing children from the Browsable API\n* Basic example\n\n### To do\n\n* Make the current example work :\n  * Fix backend and form for multiple levels of nesting\n  * Do not show `parent` select list when showing forms as children of another form\n* Write documentation / Auto-generate it from the docstrings ([pdoc](https://pdoc.dev/) ?)\n* Write tests/specs\n",
-    'author': 'pcouy',
+    'author': 'Pierre Couy',
     'author_email': 'contact@pierre-couy.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://pierre-couy.dev/projects/drf-nested-browsable.html',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.10,<4.0',
 }
```

### Comparing `drf_nested_browsable-0.1.0/PKG-INFO` & `drf_nested_browsable-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 Metadata-Version: 2.1
 Name: drf-nested-browsable
-Version: 0.1.0
+Version: 0.1.1
 Summary: Writable nested serializers with forms for the Browsable API
+Home-page: https://pierre-couy.dev/projects/drf-nested-browsable.html
 License: MIT
-Author: pcouy
+Keywords: django,rest framework,drf,browsable api,nested serializers
+Author: Pierre Couy
 Author-email: contact@pierre-couy.dev
 Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Framework :: Django
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: django (>=4.2,<5.0)
 Requires-Dist: djangorestframework (>=3.14.0,<4.0.0)
+Project-URL: Repository, https://github.com/pcouy/drf-nested-browsable
 Description-Content-Type: text/markdown
 
 :warning: Work In Progress :warning:
 
 # Writable Nested Serializers with Browsable API Forms
 
 This plugin is intended to provide writable nested serializers (similar to [the recommended plugin from DRF documentation](https://github.com/beda-software/drf-nested-browsable.git)) that bring their own forms for the Browsable API renderer.
```

