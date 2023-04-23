# Comparing `tmp/sphinxcontrib-exceltable-0.3.0.dev0.tar.gz` & `tmp/sphinxcontrib-exceltable-0.3.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib-exceltable-0.3.0.dev0.tar", last modified: Mon Apr 17 18:20:33 2023, max compression
+gzip compressed data, was "sphinxcontrib-exceltable-0.3.0.dev1.tar", last modified: Sun Apr 23 15:50:01 2023, max compression
```

## Comparing `sphinxcontrib-exceltable-0.3.0.dev0.tar` & `sphinxcontrib-exceltable-0.3.0.dev1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:20:33.954236 sphinxcontrib-exceltable-0.3.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-17 18:20:16.000000 sphinxcontrib-exceltable-0.3.0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-17 18:20:16.000000 sphinxcontrib-exceltable-0.3.0.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-17 18:20:33.954236 sphinxcontrib-exceltable-0.3.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-17 18:20:16.000000 sphinxcontrib-exceltable-0.3.0.dev0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:20:33.950236 sphinxcontrib-exceltable-0.3.0.dev0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-04-17 18:20:16.000000 sphinxcontrib-exceltable-0.3.0.dev0/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-17 18:20:33.954236 sphinxcontrib-exceltable-0.3.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-17 18:20:16.000000 sphinxcontrib-exceltable-0.3.0.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:20:33.950236 sphinxcontrib-exceltable-0.3.0.dev0/sphinxcontrib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:20:33.950236 sphinxcontrib-exceltable-0.3.0.dev0/sphinxcontrib/exceltable/
--rw-r--r--   0 runner    (1001) docker     (123)    18270 2023-04-17 18:20:16.000000 sphinxcontrib-exceltable-0.3.0.dev0/sphinxcontrib/exceltable/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:20:33.954236 sphinxcontrib-exceltable-0.3.0.dev0/sphinxcontrib_exceltable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-17 18:20:33.000000 sphinxcontrib-exceltable-0.3.0.dev0/sphinxcontrib_exceltable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-17 18:20:33.000000 sphinxcontrib-exceltable-0.3.0.dev0/sphinxcontrib_exceltable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 18:20:33.000000 sphinxcontrib-exceltable-0.3.0.dev0/sphinxcontrib_exceltable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 18:20:33.000000 sphinxcontrib-exceltable-0.3.0.dev0/sphinxcontrib_exceltable.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-17 18:20:33.000000 sphinxcontrib-exceltable-0.3.0.dev0/sphinxcontrib_exceltable.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-17 18:20:33.000000 sphinxcontrib-exceltable-0.3.0.dev0/sphinxcontrib_exceltable.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:20:33.954236 sphinxcontrib-exceltable-0.3.0.dev0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-17 18:20:16.000000 sphinxcontrib-exceltable-0.3.0.dev0/test/test_exceltable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:50:01.745522 sphinxcontrib-exceltable-0.3.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-23 15:49:51.000000 sphinxcontrib-exceltable-0.3.0.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-23 15:49:51.000000 sphinxcontrib-exceltable-0.3.0.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-23 15:50:01.745522 sphinxcontrib-exceltable-0.3.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-23 15:49:51.000000 sphinxcontrib-exceltable-0.3.0.dev1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-23 15:49:51.000000 sphinxcontrib-exceltable-0.3.0.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-23 15:50:01.745522 sphinxcontrib-exceltable-0.3.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-23 15:49:51.000000 sphinxcontrib-exceltable-0.3.0.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:50:01.741522 sphinxcontrib-exceltable-0.3.0.dev1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:50:01.741522 sphinxcontrib-exceltable-0.3.0.dev1/src/sphinxcontrib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:50:01.741522 sphinxcontrib-exceltable-0.3.0.dev1/src/sphinxcontrib/exceltable/
+-rw-r--r--   0 runner    (1001) docker     (123)    18270 2023-04-23 15:49:51.000000 sphinxcontrib-exceltable-0.3.0.dev1/src/sphinxcontrib/exceltable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:50:01.745522 sphinxcontrib-exceltable-0.3.0.dev1/src/sphinxcontrib_exceltable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-23 15:50:01.000000 sphinxcontrib-exceltable-0.3.0.dev1/src/sphinxcontrib_exceltable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-23 15:50:01.000000 sphinxcontrib-exceltable-0.3.0.dev1/src/sphinxcontrib_exceltable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 15:50:01.000000 sphinxcontrib-exceltable-0.3.0.dev1/src/sphinxcontrib_exceltable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 15:50:01.000000 sphinxcontrib-exceltable-0.3.0.dev1/src/sphinxcontrib_exceltable.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-23 15:50:01.000000 sphinxcontrib-exceltable-0.3.0.dev1/src/sphinxcontrib_exceltable.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-23 15:50:01.000000 sphinxcontrib-exceltable-0.3.0.dev1/src/sphinxcontrib_exceltable.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:50:01.745522 sphinxcontrib-exceltable-0.3.0.dev1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-23 15:49:51.000000 sphinxcontrib-exceltable-0.3.0.dev1/test/test_exceltable.py
```

### Comparing `sphinxcontrib-exceltable-0.3.0.dev0/LICENSE` & `sphinxcontrib-exceltable-0.3.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-exceltable-0.3.0.dev0/PKG-INFO` & `sphinxcontrib-exceltable-0.3.0.dev1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-exceltable
-Version: 0.3.0.dev0
+Version: 0.3.0.dev1
 Summary: Support for including Excel spreadsheets into Sphinx documents
 Home-page: https://packages.python.org/sphinxcontrib-exceltable
-Download-URL: https://pypi.python.org/pypi/sphinxcontrib-exceltable
+Download-URL: http://pypi.python.org/pypi/sphinxcontrib-exceltable
 Author: Juha Mustonen
 Author-email: juha.p.mustonen@gmail.com
-License: BSD
 Project-URL: GitHub: repo, https://github.com/sphinx-contrib/exceltable
 Project-URL: GitHub: issues, https://github.com/sphinx-contrib/exceltable/issues
-Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Documentation
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
+Requires-Python: <4,>=3.8
+Provides-Extra: test
 License-File: LICENSE
 
 Module ``sphinxcontrib.exceltable`` is an extension for Sphinx_, that adds support for including Excel spreadsheets, or part
-of them, into Sphinx document. See documentation for further information. It has been tested to run on both Python 2.7 and 3.4
+of them, into Sphinx document. See documentation for further information. It works with Python >=3.7
 
 Installation::
 
     mkdir my-docs
     cd my-docs/
 
     # Install dependencies
     python3 -v venv
     source vevn/bin/activate
     pip3 install sphinx sphinxcontrib-exceltable
 
+    # Alternatively, install pre-release
+    # pip3 install sphinxcontrib-exceltable --pre
+
     # Create simple docs
     sphinx-quickstart
 
 Configuration:
 
 Enable the extension by adding ::
 
@@ -72,13 +73,13 @@
   source venv3/bin/activate
 
   # Install dependencies
   python3 -m pip install --upgrade pip
   pip3 install -r requirements.txt
 
   # Run tests
-  PYTHONPATH=$(pwd) python3 -m pytest
+  PYTHONPATH=$(pwd)/src python3 -m pytest
 
   # Run
   python3 -m tox
 
 .. _Sphinx: https://www.sphinx-doc.org/
```

### Comparing `sphinxcontrib-exceltable-0.3.0.dev0/README.rst` & `sphinxcontrib-exceltable-0.3.0.dev1/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Module ``sphinxcontrib.exceltable`` is an extension for Sphinx_, that adds support for including Excel spreadsheets, or part
-of them, into Sphinx document. See documentation for further information. It has been tested to run on both Python 2.7 and 3.4
+of them, into Sphinx document. See documentation for further information. It works with Python >=3.7
 
 Installation::
 
     mkdir my-docs
     cd my-docs/
 
     # Install dependencies
     python3 -v venv
     source vevn/bin/activate
     pip3 install sphinx sphinxcontrib-exceltable
 
+    # Alternatively, install pre-release
+    # pip3 install sphinxcontrib-exceltable --pre
+
     # Create simple docs
     sphinx-quickstart
 
 Configuration:
 
 Enable the extension by adding ::
 
@@ -45,13 +48,13 @@
   source venv3/bin/activate
 
   # Install dependencies
   python3 -m pip install --upgrade pip
   pip3 install -r requirements.txt
 
   # Run tests
-  PYTHONPATH=$(pwd) python3 -m pytest
+  PYTHONPATH=$(pwd)/src python3 -m pytest
 
   # Run
   python3 -m tox
 
 .. _Sphinx: https://www.sphinx-doc.org/
```

### Comparing `sphinxcontrib-exceltable-0.3.0.dev0/setup.cfg` & `sphinxcontrib-exceltable-0.3.0.dev1/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,48 @@
 [metadata]
 name = sphinxcontrib-exceltable
-description = Sphinx exceltable obfuscation extension
-long_description = file: README.rst
-long_description_content_type = text/x-rst
-url = https://github.com/sphinx-contrib/exceltable
+version = 0.3.0-dev1
 author = Juha Mustonen
 author_email = juha.p.mustonen@gmail.com
-license = BSD-3-Clause
-license_file = LICENSE
-license_files = LICENSE
+description = Support for including Excel spreadsheets into Sphinx documents
+long_description = file: README.rst
+url = https://packages.python.org/sphinxcontrib-exceltable
+download_url = http://pypi.python.org/pypi/sphinxcontrib-exceltable
+project_urls = 
+	GitHub: repo = https://github.com/sphinx-contrib/exceltable
+	GitHub: issues = https://github.com/sphinx-contrib/exceltable/issues
 classifiers = 
-	Development Status :: 3 - Alpha
+	Development Status :: 4 - Beta
 	Environment :: Console
 	Environment :: Web Environment
-	Framework :: Sphinx :: Extension
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
+	Programming Language :: Python
+	Programming Language :: Python :: 2
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3 :: Only
-	Topic :: Documentation :: Sphinx
+	Topic :: Documentation
 	Topic :: Utilities
-download_url = http://pypi.python.org/pypi/sphinxcontrib-exceltable
-project_urls = 
-	GitHub: repo = https://github.com/sphinx-contrib/exceltable
-	GitHub: issues = https://github.com/sphinx-contrib/exceltable/issues
 
 [options]
 packages = find_namespace:
+python_requires = >=3.8, <4
 install_requires = 
-	Sphinx>=1.8
-	Sphinx>=0.6
-	xlrd>=2.0
-	docutils>=0.19
-python_requires = >=3.7
-include_package_data = True
+	Sphinx>=5
+	xlrd
+	docutils
+include_package_data = False
+package_dir = 
+	= src
 platforms = any
 zip_safe = False
 
-[aliases]
-release = check -rs sdist bdist_wheel
-
-[nosetests]
-verbosity = 1
-detailed-errors = 1
-with-coverage = 1
-cover-package = nose
-debug = nose.loader
-pdb = 1
-pdb-failures = 1
-
-[build_sphinx]
-source-dir = doc/
-build-dir = build/doc
-all_files = 1
+[options.packages.find]
+where = src
 
-[upload_docs]
-upload_dir = build/doc/html
+[options.extras_require]
+test = pytest
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sphinxcontrib-exceltable-0.3.0.dev0/sphinxcontrib/exceltable/__init__.py` & `sphinxcontrib-exceltable-0.3.0.dev1/src/sphinxcontrib/exceltable/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-exceltable-0.3.0.dev0/sphinxcontrib_exceltable.egg-info/PKG-INFO` & `sphinxcontrib-exceltable-0.3.0.dev1/src/sphinxcontrib_exceltable.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-exceltable
-Version: 0.3.0.dev0
+Version: 0.3.0.dev1
 Summary: Support for including Excel spreadsheets into Sphinx documents
 Home-page: https://packages.python.org/sphinxcontrib-exceltable
-Download-URL: https://pypi.python.org/pypi/sphinxcontrib-exceltable
+Download-URL: http://pypi.python.org/pypi/sphinxcontrib-exceltable
 Author: Juha Mustonen
 Author-email: juha.p.mustonen@gmail.com
-License: BSD
 Project-URL: GitHub: repo, https://github.com/sphinx-contrib/exceltable
 Project-URL: GitHub: issues, https://github.com/sphinx-contrib/exceltable/issues
-Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Documentation
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
+Requires-Python: <4,>=3.8
+Provides-Extra: test
 License-File: LICENSE
 
 Module ``sphinxcontrib.exceltable`` is an extension for Sphinx_, that adds support for including Excel spreadsheets, or part
-of them, into Sphinx document. See documentation for further information. It has been tested to run on both Python 2.7 and 3.4
+of them, into Sphinx document. See documentation for further information. It works with Python >=3.7
 
 Installation::
 
     mkdir my-docs
     cd my-docs/
 
     # Install dependencies
     python3 -v venv
     source vevn/bin/activate
     pip3 install sphinx sphinxcontrib-exceltable
 
+    # Alternatively, install pre-release
+    # pip3 install sphinxcontrib-exceltable --pre
+
     # Create simple docs
     sphinx-quickstart
 
 Configuration:
 
 Enable the extension by adding ::
 
@@ -72,13 +73,13 @@
   source venv3/bin/activate
 
   # Install dependencies
   python3 -m pip install --upgrade pip
   pip3 install -r requirements.txt
 
   # Run tests
-  PYTHONPATH=$(pwd) python3 -m pytest
+  PYTHONPATH=$(pwd)/src python3 -m pytest
 
   # Run
   python3 -m tox
 
 .. _Sphinx: https://www.sphinx-doc.org/
```

### Comparing `sphinxcontrib-exceltable-0.3.0.dev0/test/test_exceltable.py` & `sphinxcontrib-exceltable-0.3.0.dev1/test/test_exceltable.py`

 * *Files identical despite different names*

