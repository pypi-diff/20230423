# Comparing `tmp/drf-recaptcha-2.2.2.tar.gz` & `tmp/drf-recaptcha-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-recaptcha-2.2.2.tar", last modified: Tue Oct 25 13:26:19 2022, max compression
+gzip compressed data, was "drf-recaptcha-2.2.3.tar", last modified: Sun Apr 23 05:39:50 2023, max compression
```

## Comparing `drf-recaptcha-2.2.2.tar` & `drf-recaptcha-2.2.3.tar`

### file list

```diff
@@ -1,22 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 13:26:19.546959 drf-recaptcha-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-10-25 13:26:09.000000 drf-recaptcha-2.2.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-10-25 13:26:09.000000 drf-recaptcha-2.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5699 2022-10-25 13:26:19.546959 drf-recaptcha-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4331 2022-10-25 13:26:09.000000 drf-recaptcha-2.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 13:26:19.546959 drf-recaptcha-2.2.2/drf_recaptcha/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-25 13:26:09.000000 drf-recaptcha-2.2.2/drf_recaptcha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-10-25 13:26:09.000000 drf-recaptcha-2.2.2/drf_recaptcha/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1120 2022-10-25 13:26:09.000000 drf-recaptcha-2.2.2/drf_recaptcha/checks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1665 2022-10-25 13:26:09.000000 drf-recaptcha-2.2.2/drf_recaptcha/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      697 2022-10-25 13:26:09.000000 drf-recaptcha-2.2.2/drf_recaptcha/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     3210 2022-10-25 13:26:09.000000 drf-recaptcha-2.2.2/drf_recaptcha/fields.py
--rw-r--r--   0 runner    (1001) docker     (121)     4932 2022-10-25 13:26:09.000000 drf-recaptcha-2.2.2/drf_recaptcha/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 13:26:19.546959 drf-recaptcha-2.2.2/drf_recaptcha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5699 2022-10-25 13:26:19.000000 drf-recaptcha-2.2.2/drf_recaptcha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      446 2022-10-25 13:26:19.000000 drf-recaptcha-2.2.2/drf_recaptcha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-25 13:26:19.000000 drf-recaptcha-2.2.2/drf_recaptcha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-25 13:26:19.000000 drf-recaptcha-2.2.2/drf_recaptcha.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-10-25 13:26:19.000000 drf-recaptcha-2.2.2/drf_recaptcha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-10-25 13:26:19.000000 drf-recaptcha-2.2.2/drf_recaptcha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      642 2022-10-25 13:26:19.546959 drf-recaptcha-2.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1957 2022-10-25 13:26:09.000000 drf-recaptcha-2.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 05:39:50.908832 drf-recaptcha-2.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-23 05:39:39.000000 drf-recaptcha-2.2.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-23 05:39:39.000000 drf-recaptcha-2.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-04-23 05:39:50.908832 drf-recaptcha-2.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-04-23 05:39:39.000000 drf-recaptcha-2.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 05:39:50.904832 drf-recaptcha-2.2.3/drf_recaptcha/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 05:39:39.000000 drf-recaptcha-2.2.3/drf_recaptcha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-23 05:39:39.000000 drf-recaptcha-2.2.3/drf_recaptcha/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-23 05:39:39.000000 drf-recaptcha-2.2.3/drf_recaptcha/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-23 05:39:39.000000 drf-recaptcha-2.2.3/drf_recaptcha/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-23 05:39:39.000000 drf-recaptcha-2.2.3/drf_recaptcha/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-04-23 05:39:39.000000 drf-recaptcha-2.2.3/drf_recaptcha/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-04-23 05:39:39.000000 drf-recaptcha-2.2.3/drf_recaptcha/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 05:39:50.908832 drf-recaptcha-2.2.3/drf_recaptcha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-04-23 05:39:50.000000 drf-recaptcha-2.2.3/drf_recaptcha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-23 05:39:50.000000 drf-recaptcha-2.2.3/drf_recaptcha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 05:39:50.000000 drf-recaptcha-2.2.3/drf_recaptcha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 05:39:50.000000 drf-recaptcha-2.2.3/drf_recaptcha.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-23 05:39:50.000000 drf-recaptcha-2.2.3/drf_recaptcha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-23 05:39:50.000000 drf-recaptcha-2.2.3/drf_recaptcha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-23 05:39:50.908832 drf-recaptcha-2.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-23 05:39:39.000000 drf-recaptcha-2.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 05:39:50.908832 drf-recaptcha-2.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-23 05:39:39.000000 drf-recaptcha-2.2.3/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-23 05:39:39.000000 drf-recaptcha-2.2.3/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-23 05:39:39.000000 drf-recaptcha-2.2.3/tests/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-23 05:39:39.000000 drf-recaptcha-2.2.3/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-04-23 05:39:39.000000 drf-recaptcha-2.2.3/tests/test_validator.py
```

### Comparing `drf-recaptcha-2.2.2/LICENSE.md` & `drf-recaptcha-2.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `drf-recaptcha-2.2.2/PKG-INFO` & `drf-recaptcha-2.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 Metadata-Version: 2.1
 Name: drf-recaptcha
-Version: 2.2.2
+Version: 2.2.3
 Summary: Django rest framework recaptcha field serializer.
 Home-page: https://github.com/llybin/drf-recaptcha
 Author: Lev Lybin
 Author-email: lev.lybin@gmail.com
 License: MIT
 Keywords: django,drf,rest,django-rest-framework,reCAPTCHA,reCAPTCHA v2,reCAPTCHA v3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Django REST reCAPTCHA
 
 **Django REST reCAPTCHA v2 and v3 field serializer**
@@ -42,16 +44,16 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI](https://img.shields.io/pypi/v/drf-recaptcha)](https://pypi.org/project/drf-recaptcha/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/drf-recaptcha)](https://pypi.org/project/drf-recaptcha/)
 [![PyPI - License](https://img.shields.io/pypi/l/drf-recaptcha)](https://pypi.org/project/drf-recaptcha/)
 
 ## Requirements
 
-*   Python: 3.7, 3.8, 3.9, 3.10
-*   Django: 3.2, 4.0, 4.1
+*   Python: 3.7, 3.8, 3.9, 3.10, 3.11
+*   Django: 3.2, 4.0, 4.1, 4.2
 *   DRF: 3.11, 3.12, 3.13, 3.14
 
 ## Installation
 
 1.  [Sign up for reCAPTCHA](https://www.google.com/recaptcha/)
 2.  Install with `pip install drf-recaptcha`
 3.  Add `"drf_recaptcha"` to your `INSTALLED_APPS` settings.
```

### Comparing `drf-recaptcha-2.2.2/README.md` & `drf-recaptcha-2.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI](https://img.shields.io/pypi/v/drf-recaptcha)](https://pypi.org/project/drf-recaptcha/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/drf-recaptcha)](https://pypi.org/project/drf-recaptcha/)
 [![PyPI - License](https://img.shields.io/pypi/l/drf-recaptcha)](https://pypi.org/project/drf-recaptcha/)
 
 ## Requirements
 
-*   Python: 3.7, 3.8, 3.9, 3.10
-*   Django: 3.2, 4.0, 4.1
+*   Python: 3.7, 3.8, 3.9, 3.10, 3.11
+*   Django: 3.2, 4.0, 4.1, 4.2
 *   DRF: 3.11, 3.12, 3.13, 3.14
 
 ## Installation
 
 1.  [Sign up for reCAPTCHA](https://www.google.com/recaptcha/)
 2.  Install with `pip install drf-recaptcha`
 3.  Add `"drf_recaptcha"` to your `INSTALLED_APPS` settings.
```

### Comparing `drf-recaptcha-2.2.2/drf_recaptcha/checks.py` & `drf-recaptcha-2.2.3/drf_recaptcha/checks.py`

 * *Files identical despite different names*

### Comparing `drf-recaptcha-2.2.2/drf_recaptcha/client.py` & `drf-recaptcha-2.2.3/drf_recaptcha/client.py`

 * *Files identical despite different names*

### Comparing `drf-recaptcha-2.2.2/drf_recaptcha/constants.py` & `drf-recaptcha-2.2.3/drf_recaptcha/constants.py`

 * *Files identical despite different names*

### Comparing `drf-recaptcha-2.2.2/drf_recaptcha/fields.py` & `drf-recaptcha-2.2.3/drf_recaptcha/fields.py`

 * *Files identical despite different names*

### Comparing `drf-recaptcha-2.2.2/drf_recaptcha/validators.py` & `drf-recaptcha-2.2.3/drf_recaptcha/validators.py`

 * *Files identical despite different names*

### Comparing `drf-recaptcha-2.2.2/drf_recaptcha.egg-info/PKG-INFO` & `drf-recaptcha-2.2.3/drf_recaptcha.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 Metadata-Version: 2.1
 Name: drf-recaptcha
-Version: 2.2.2
+Version: 2.2.3
 Summary: Django rest framework recaptcha field serializer.
 Home-page: https://github.com/llybin/drf-recaptcha
 Author: Lev Lybin
 Author-email: lev.lybin@gmail.com
 License: MIT
 Keywords: django,drf,rest,django-rest-framework,reCAPTCHA,reCAPTCHA v2,reCAPTCHA v3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Django REST reCAPTCHA
 
 **Django REST reCAPTCHA v2 and v3 field serializer**
@@ -42,16 +44,16 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI](https://img.shields.io/pypi/v/drf-recaptcha)](https://pypi.org/project/drf-recaptcha/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/drf-recaptcha)](https://pypi.org/project/drf-recaptcha/)
 [![PyPI - License](https://img.shields.io/pypi/l/drf-recaptcha)](https://pypi.org/project/drf-recaptcha/)
 
 ## Requirements
 
-*   Python: 3.7, 3.8, 3.9, 3.10
-*   Django: 3.2, 4.0, 4.1
+*   Python: 3.7, 3.8, 3.9, 3.10, 3.11
+*   Django: 3.2, 4.0, 4.1, 4.2
 *   DRF: 3.11, 3.12, 3.13, 3.14
 
 ## Installation
 
 1.  [Sign up for reCAPTCHA](https://www.google.com/recaptcha/)
 2.  Install with `pip install drf-recaptcha`
 3.  Add `"drf_recaptcha"` to your `INSTALLED_APPS` settings.
```

### Comparing `drf-recaptcha-2.2.2/setup.cfg` & `drf-recaptcha-2.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `drf-recaptcha-2.2.2/setup.py` & `drf-recaptcha-2.2.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 
 def read(f):
     return open(f, encoding="utf-8").read()
 
 
 setup(
     name="drf-recaptcha",
-    version="2.2.2",
+    version="2.2.3",
     description="Django rest framework recaptcha field serializer.",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     author="Lev Lybin",
     author_email="lev.lybin@gmail.com",
     license="MIT",
     url="https://github.com/llybin/drf-recaptcha",
     packages=find_packages(exclude=["tests*"]),
     install_requires=[
-        "django>=3.2,<4.2",
-        "djangorestframework>=3.11,<4.0",
-        "django-ipware>=2.1,<4.1",
+        "django>=3.2",
+        "djangorestframework>=3.11",
+        "django-ipware>=2.1",
     ],
     setup_requires=["pytest-runner"],
     tests_require=["pytest", "pytest-django", "pytest-cov"],
     python_requires=">=3.7",
     include_package_data=True,
     zip_safe=False,
     keywords=[
@@ -40,22 +40,24 @@
         "Environment :: Web Environment",
         "Environment :: Plugins",
         "Intended Audience :: Developers",
         "Framework :: Django",
         "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.0",
         "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
         "Topic :: Security",
         "Topic :: Software Development :: Libraries",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

