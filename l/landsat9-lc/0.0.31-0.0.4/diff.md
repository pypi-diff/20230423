# Comparing `tmp/landsat9_lc-0.0.31.tar.gz` & `tmp/landsat9_lc-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "dist\landsat9_lc-0.0.4.tar", last modified: Sun Apr 23 20:57:32 2023, max compression
```

## Comparing `landsat9_lc-0.0.31.tar` & `landsat9_lc-0.0.4.tar`

### file list

```diff
@@ -1,45 +1,29 @@
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/.editorconfig
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/.gitattributes
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/MANIFEST.in
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/environment.yml
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/mkdocs.yml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/requirements.txt
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/requirements_dev.txt
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/setup.cfg
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/setup.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/tox.ini
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/.github/workflows/build.yml
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/.github/workflows/pypi.yml
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/config/__init__.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/config/data.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/config/model.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/config/package.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/config/xarray_dims.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/docs/api.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/docs/how_to_use.md
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/docs/index.md
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/docs/installation.md
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/landsat9_lc/__init__.py
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/landsat9_lc/l9_lc_classifier.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/landsat9_lc/train_pipeline.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/landsat9_lc/models/label_encoder.json
--rw-r--r--   0        0        0  9055506 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/landsat9_lc/models/pipeline_0.0.1.pkl
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/landsat9_lc/pipeline/__init__.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/landsat9_lc/pipeline/model_pipeline.py
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/landsat9_lc/pipeline/spyndex_transformer.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/landsat9_lc/processing/__init__.py
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/landsat9_lc/processing/data_manager.py
--rw-r--r--   0        0        0     9008 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/landsat9_lc/processing/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/tests/__init__.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/tests/conftest.py
--rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/tests/test_make_prediction.py
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/.gitignore
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/AUTHORS.rst
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/LICENSE
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/README.md
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/pyproject.toml
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 landsat9_lc-0.0.31/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-23 20:57:32.000000 landsat9_lc-0.0.4/
+-rw-rw-rw-   0        0        0      176 2023-04-22 16:46:50.000000 landsat9_lc-0.0.4/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1094 2023-04-22 16:46:50.000000 landsat9_lc-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      127 2023-04-22 16:46:50.000000 landsat9_lc-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1422 2023-04-23 20:57:32.000000 landsat9_lc-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      725 2023-04-22 16:46:50.000000 landsat9_lc-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 20:57:32.000000 landsat9_lc-0.0.4/landsat9_lc/
+-rw-rw-rw-   0        0        0       52 2023-04-22 16:46:51.000000 landsat9_lc-0.0.4/landsat9_lc/__init__.py
+-rw-rw-rw-   0        0        0     3356 2023-04-22 16:46:51.000000 landsat9_lc-0.0.4/landsat9_lc/l9_lc_classifier.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:57:32.000000 landsat9_lc-0.0.4/landsat9_lc/pipeline/
+-rw-rw-rw-   0        0        0       38 2023-04-22 16:46:51.000000 landsat9_lc-0.0.4/landsat9_lc/pipeline/__init__.py
+-rw-rw-rw-   0        0        0     1782 2023-04-22 16:46:51.000000 landsat9_lc-0.0.4/landsat9_lc/pipeline/model_pipeline.py
+-rw-rw-rw-   0        0        0     2366 2023-04-22 16:46:51.000000 landsat9_lc-0.0.4/landsat9_lc/pipeline/spyndex_transformer.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:57:32.000000 landsat9_lc-0.0.4/landsat9_lc/processing/
+-rw-rw-rw-   0        0        0       22 2023-04-22 16:46:51.000000 landsat9_lc-0.0.4/landsat9_lc/processing/__init__.py
+-rw-rw-rw-   0        0        0     2113 2023-04-22 16:46:51.000000 landsat9_lc-0.0.4/landsat9_lc/processing/data_manager.py
+-rw-rw-rw-   0        0        0     9008 2023-04-22 16:46:51.000000 landsat9_lc-0.0.4/landsat9_lc/processing/utils.py
+-rw-rw-rw-   0        0        0     1008 2023-04-22 16:46:51.000000 landsat9_lc-0.0.4/landsat9_lc/train_pipeline.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:57:32.000000 landsat9_lc-0.0.4/landsat9_lc.egg-info/
+-rw-rw-rw-   0        0        0     1422 2023-04-23 20:57:31.000000 landsat9_lc-0.0.4/landsat9_lc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      608 2023-04-23 20:57:32.000000 landsat9_lc-0.0.4/landsat9_lc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      266 2023-04-23 20:57:31.000000 landsat9_lc-0.0.4/landsat9_lc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-22 17:23:39.000000 landsat9_lc-0.0.4/landsat9_lc.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      266 2023-04-23 20:57:31.000000 landsat9_lc-0.0.4/landsat9_lc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-23 20:57:31.000000 landsat9_lc-0.0.4/landsat9_lc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      593 2023-04-23 20:57:20.000000 landsat9_lc-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      279 2023-04-22 16:46:51.000000 landsat9_lc-0.0.4/requirements.txt
+-rw-rw-rw-   0        0        0      482 2023-04-23 20:57:32.000000 landsat9_lc-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2206 2023-04-23 20:57:20.000000 landsat9_lc-0.0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `landsat9_lc-0.0.31/setup.py` & `landsat9_lc-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,10 +65,10 @@
     keywords='landsat9_lc',
     name='landsat9_lc',
     packages=find_packages(include=['landsat9_lc', 'landsat9_lc.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/hectorpatino/landsat9_lc',
-    version='0.0.31',
+    version='0.0.4',
     zip_safe=False,
 )
```

### Comparing `landsat9_lc-0.0.31/landsat9_lc/l9_lc_classifier.py` & `landsat9_lc-0.0.4/landsat9_lc/l9_lc_classifier.py`

 * *Files identical despite different names*

### Comparing `landsat9_lc-0.0.31/landsat9_lc/train_pipeline.py` & `landsat9_lc-0.0.4/landsat9_lc/train_pipeline.py`

 * *Files identical despite different names*

### Comparing `landsat9_lc-0.0.31/landsat9_lc/pipeline/model_pipeline.py` & `landsat9_lc-0.0.4/landsat9_lc/pipeline/model_pipeline.py`

 * *Files identical despite different names*

### Comparing `landsat9_lc-0.0.31/landsat9_lc/pipeline/spyndex_transformer.py` & `landsat9_lc-0.0.4/landsat9_lc/pipeline/spyndex_transformer.py`

 * *Files identical despite different names*

### Comparing `landsat9_lc-0.0.31/landsat9_lc/processing/data_manager.py` & `landsat9_lc-0.0.4/landsat9_lc/processing/data_manager.py`

 * *Files identical despite different names*

### Comparing `landsat9_lc-0.0.31/landsat9_lc/processing/utils.py` & `landsat9_lc-0.0.4/landsat9_lc/processing/utils.py`

 * *Files identical despite different names*

### Comparing `landsat9_lc-0.0.31/LICENSE` & `landsat9_lc-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `landsat9_lc-0.0.31/README.md` & `landsat9_lc-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `landsat9_lc-0.0.31/pyproject.toml` & `landsat9_lc-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "landsat9_lc"
-version = "0.0.31"
+version = "0.0.4"
 authors = [
   { name="Hector Patiño", email="hectorpatino24@gmail.com" },
 ]
 description = "A python ML model to classify landsat 9 images"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `landsat9_lc-0.0.31/PKG-INFO` & `landsat9_lc-0.0.4/landsat9_lc.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,42 @@
-Metadata-Version: 2.1
-Name: landsat9_lc
-Version: 0.0.31
-Summary: A python ML model to classify landsat 9 images
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
-Author-email: Hector Patiño <hectorpatino24@gmail.com>
-License-File: AUTHORS.rst
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-
-# landsat9_lc
-
-
-[![image](https://img.shields.io/pypi/v/landsat9_lc.svg)](https://pypi.python.org/pypi/landsat9_lc)
-[![image](https://img.shields.io/conda/vn/conda-forge/landsat9_lc.svg)](https://anaconda.org/conda-forge/landsat9_lc)
-
-[![image](https://pyup.io/repos/github/hectorpatino/landsat9_lc/shield.svg)](https://pyup.io/repos/github/hectorpatino/landsat9_lc)
-
-
-**A Short description**
-
-
--   Free software: MIT license
--   Documentation: https://hectorpatino.github.io/landsat9_lc
-    
-
-## Features
-
--   TODO
-
-## Credits
-
-This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
+Metadata-Version: 2.1
+Name: landsat9-lc
+Version: 0.0.4
+Summary: A python ML model to classify landsat 9 images
+Home-page: https://github.com/hectorpatino/landsat9_lc
+Author: Hector Patino
+Author-email: Hector Patiño <hectorpatino24@gmail.com>
+License: MIT license
+Project-URL: Homepage, https://github.com/pypa/sampleproject
+Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Keywords: landsat9_lc
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+# landsat9_lc
+
+
+[![image](https://img.shields.io/pypi/v/landsat9_lc.svg)](https://pypi.python.org/pypi/landsat9_lc)
+[![image](https://img.shields.io/conda/vn/conda-forge/landsat9_lc.svg)](https://anaconda.org/conda-forge/landsat9_lc)
+
+[![image](https://pyup.io/repos/github/hectorpatino/landsat9_lc/shield.svg)](https://pyup.io/repos/github/hectorpatino/landsat9_lc)
+
+
+**A Short description**
+
+
+-   Free software: MIT license
+-   Documentation: https://hectorpatino.github.io/landsat9_lc
+    
+
+## Features
+
+-   TODO
+
+## Credits
+
+This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

