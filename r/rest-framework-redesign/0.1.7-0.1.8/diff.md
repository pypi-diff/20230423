# Comparing `tmp/rest_framework_redesign-0.1.7.tar.gz` & `tmp/rest_framework_redesign-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rest_framework_redesign-0.1.7.tar", max compression
+gzip compressed data, was "rest_framework_redesign-0.1.8.tar", max compression
```

## Comparing `rest_framework_redesign-0.1.7.tar` & `rest_framework_redesign-0.1.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1095 2023-04-17 08:21:25.010142 rest_framework_redesign-0.1.7/LICENSE
--rw-r--r--   0        0        0      617 2023-04-23 05:13:06.611169 rest_framework_redesign-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      792 2023-04-18 08:20:43.087539 rest_framework_redesign-0.1.7/README.md
--rw-r--r--   0        0        0        0 2023-04-17 08:27:28.035216 rest_framework_redesign-0.1.7/rest_framework_redesign/__init__.py
--rw-r--r--   0        0        0      111 2023-04-17 08:32:42.129922 rest_framework_redesign-0.1.7/rest_framework_redesign/admin.py
--rw-r--r--   0        0        0      248 2023-04-17 08:33:14.492981 rest_framework_redesign-0.1.7/rest_framework_redesign/apps.py
--rw-r--r--   0        0        0        0 2023-04-17 08:27:28.038933 rest_framework_redesign-0.1.7/rest_framework_redesign/migrations/__init__.py
--rw-r--r--   0        0        0       84 2023-04-17 08:33:33.145101 rest_framework_redesign-0.1.7/rest_framework_redesign/models.py
--rw-r--r--   0        0        0    23750 2023-04-20 09:09:17.444650 rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/api.html
--rw-r--r--   0        0        0     1085 2023-04-20 09:11:06.989223 rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/filters/base.html
--rw-r--r--   0        0        0      700 2023-04-18 08:50:06.523205 rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/filters/ordering.html
--rw-r--r--   0        0        0      608 2023-04-18 08:49:46.702650 rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/filters/search.html
--rw-r--r--   0        0        0      866 2023-04-19 11:57:00.707959 rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html
--rw-r--r--   0        0        0     1567 2023-04-19 11:56:43.779104 rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2023-04-16 10:47:42.246290 rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/horizontal/dict_field.html
--rw-r--r--   0        0        0      427 2023-04-16 10:49:02.575135 rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/horizontal/fieldset.html
--rw-r--r--   0        0        0      150 2023-04-16 10:49:14.840634 rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/horizontal/form.html
--rw-r--r--   0        0        0     1182 2023-04-19 11:59:11.581766 rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/horizontal/input.html
--rw-r--r--   0        0        0      262 2023-04-16 10:53:49.067743 rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/horizontal/list_field.html
--rw-r--r--   0        0        0      330 2023-04-16 10:54:36.132965 rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/horizontal/list_fieldset.html
--rw-r--r--   0        0        0     1499 2023-04-19 11:58:53.030223 rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/horizontal/radio.html
--rw-r--r--   0        0        0     1220 2023-04-19 11:59:53.039237 rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/horizontal/select.html
--rw-r--r--   0        0        0     1254 2023-04-19 11:59:33.439478 rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html
--rw-r--r--   0        0        0      828 2023-04-19 12:00:12.217896 rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html
--rw-r--r--   0        0        0     4375 2023-04-18 08:11:26.812363 rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/login.html
--rw-r--r--   0        0        0     1715 2023-04-16 10:26:12.389947 rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/pagination/numbers.html
--rw-r--r--   0        0        0      692 2023-04-16 10:31:24.701736 rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html
--rw-r--r--   0        0        0      307 2023-04-18 06:07:45.314176 rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/raw_data_form.html
--rw-r--r--   0        0        0       86 2023-04-17 08:33:49.776642 rest_framework_redesign-0.1.7/rest_framework_redesign/tests.py
--rw-r--r--   0        0        0       89 2023-04-17 08:34:08.004477 rest_framework_redesign-0.1.7/rest_framework_redesign/views.py
--rw-r--r--   0        0        0     1503 1970-01-01 00:00:00.000000 rest_framework_redesign-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-04-17 08:21:25.010142 rest_framework_redesign-0.1.8/LICENSE
+-rw-r--r--   0        0        0      618 2023-04-23 05:25:09.177260 rest_framework_redesign-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      792 2023-04-18 08:20:43.087539 rest_framework_redesign-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 08:27:28.035216 rest_framework_redesign-0.1.8/rest_framework_redesign/__init__.py
+-rw-r--r--   0        0        0      111 2023-04-17 08:32:42.129922 rest_framework_redesign-0.1.8/rest_framework_redesign/admin.py
+-rw-r--r--   0        0        0      248 2023-04-17 08:33:14.492981 rest_framework_redesign-0.1.8/rest_framework_redesign/apps.py
+-rw-r--r--   0        0        0        0 2023-04-17 08:27:28.038933 rest_framework_redesign-0.1.8/rest_framework_redesign/migrations/__init__.py
+-rw-r--r--   0        0        0       84 2023-04-17 08:33:33.145101 rest_framework_redesign-0.1.8/rest_framework_redesign/models.py
+-rw-r--r--   0        0        0    23750 2023-04-20 09:09:17.444650 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/api.html
+-rw-r--r--   0        0        0     1085 2023-04-20 09:11:06.989223 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/filters/base.html
+-rw-r--r--   0        0        0      700 2023-04-18 08:50:06.523205 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/filters/ordering.html
+-rw-r--r--   0        0        0      608 2023-04-18 08:49:46.702650 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/filters/search.html
+-rw-r--r--   0        0        0      866 2023-04-19 11:57:00.707959 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html
+-rw-r--r--   0        0        0     1567 2023-04-19 11:56:43.779104 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2023-04-16 10:47:42.246290 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/dict_field.html
+-rw-r--r--   0        0        0      427 2023-04-16 10:49:02.575135 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/fieldset.html
+-rw-r--r--   0        0        0      150 2023-04-16 10:49:14.840634 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/form.html
+-rw-r--r--   0        0        0     1182 2023-04-19 11:59:11.581766 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/input.html
+-rw-r--r--   0        0        0      262 2023-04-16 10:53:49.067743 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/list_field.html
+-rw-r--r--   0        0        0      330 2023-04-16 10:54:36.132965 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/list_fieldset.html
+-rw-r--r--   0        0        0     1499 2023-04-19 11:58:53.030223 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/radio.html
+-rw-r--r--   0        0        0     1220 2023-04-19 11:59:53.039237 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/select.html
+-rw-r--r--   0        0        0     1254 2023-04-19 11:59:33.439478 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html
+-rw-r--r--   0        0        0      828 2023-04-19 12:00:12.217896 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html
+-rw-r--r--   0        0        0     4375 2023-04-18 08:11:26.812363 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/login.html
+-rw-r--r--   0        0        0     1715 2023-04-16 10:26:12.389947 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/pagination/numbers.html
+-rw-r--r--   0        0        0      692 2023-04-16 10:31:24.701736 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html
+-rw-r--r--   0        0        0      307 2023-04-18 06:07:45.314176 rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/raw_data_form.html
+-rw-r--r--   0        0        0       86 2023-04-17 08:33:49.776642 rest_framework_redesign-0.1.8/rest_framework_redesign/tests.py
+-rw-r--r--   0        0        0       89 2023-04-17 08:34:08.004477 rest_framework_redesign-0.1.8/rest_framework_redesign/views.py
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 rest_framework_redesign-0.1.8/PKG-INFO
```

### Comparing `rest_framework_redesign-0.1.7/LICENSE` & `rest_framework_redesign-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.7/pyproject.toml` & `rest_framework_redesign-0.1.8/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "rest-framework-redesign"
-version = "0.1.7"
+version = "0.1.8"
 description = "Redesign of the browsable api of Django REST Framework"
 authors = ["Yousef Abu Shanab <josephyousef249@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "rest_framework_redesign"}]
 homepage = "https://github.com/youzarsiph/rest-framework-redesign/"
 repository = "https://github.com/youzarsiph/rest-framework-redesign/"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 django = "^4.2"
-djangorestframework = "^4.2"
+djangorestframework = "^3.14"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `rest_framework_redesign-0.1.7/README.md` & `rest_framework_redesign-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/api.html` & `rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/api.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/filters/base.html` & `rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/filters/base.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/filters/ordering.html` & `rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/filters/ordering.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/filters/search.html` & `rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/filters/search.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html` & `rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html` & `rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/horizontal/input.html` & `rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/input.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/horizontal/radio.html` & `rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/radio.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/horizontal/select.html` & `rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/select.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html` & `rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html` & `rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/login.html` & `rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/login.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/pagination/numbers.html` & `rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/pagination/numbers.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.7/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html` & `rest_framework_redesign-0.1.8/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.7/PKG-INFO` & `rest_framework_redesign-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: rest-framework-redesign
-Version: 0.1.7
+Version: 0.1.8
 Summary: Redesign of the browsable api of Django REST Framework
 Home-page: https://github.com/youzarsiph/rest-framework-redesign/
 License: MIT
 Author: Yousef Abu Shanab
 Author-email: josephyousef249@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: django (>=4.2,<5.0)
-Requires-Dist: djangorestframework (>=4.2,<5.0)
+Requires-Dist: djangorestframework (>=3.14,<4.0)
 Project-URL: Repository, https://github.com/youzarsiph/rest-framework-redesign/
 Description-Content-Type: text/markdown
 
 # rest-framework-redesign
 
 Redesign of the browsable api of Django REST Framework
```

