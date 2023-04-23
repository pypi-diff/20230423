# Comparing `tmp/edgetest-pip-tools-2022.4.1.tar.gz` & `tmp/edgetest-pip-tools-2023.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgetest-pip-tools-2022.4.1.tar", last modified: Tue Apr 19 15:35:15 2022, max compression
+gzip compressed data, was "edgetest-pip-tools-2023.4.0.tar", last modified: Sun Apr 23 17:54:42 2023, max compression
```

## Comparing `edgetest-pip-tools-2022.4.1.tar` & `edgetest-pip-tools-2023.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 15:35:15.284051 edgetest-pip-tools-2022.4.1/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-04-19 15:34:34.000000 edgetest-pip-tools-2022.4.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-04-19 15:34:34.000000 edgetest-pip-tools-2022.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-04-19 15:34:34.000000 edgetest-pip-tools-2022.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3058 2022-04-19 15:35:15.284051 edgetest-pip-tools-2022.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1862 2022-04-19 15:34:34.000000 edgetest-pip-tools-2022.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 15:35:15.280051 edgetest-pip-tools-2022.4.1/edgetest_pip_tools/
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-04-19 15:34:34.000000 edgetest-pip-tools-2022.4.1/edgetest_pip_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2808 2022-04-19 15:34:34.000000 edgetest-pip-tools-2022.4.1/edgetest_pip_tools/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 15:35:15.284051 edgetest-pip-tools-2022.4.1/edgetest_pip_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3058 2022-04-19 15:35:14.000000 edgetest-pip-tools-2022.4.1/edgetest_pip_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      468 2022-04-19 15:35:15.000000 edgetest-pip-tools-2022.4.1/edgetest_pip_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-19 15:35:14.000000 edgetest-pip-tools-2022.4.1/edgetest_pip_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-04-19 15:35:15.000000 edgetest-pip-tools-2022.4.1/edgetest_pip_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-19 15:35:07.000000 edgetest-pip-tools-2022.4.1/edgetest_pip_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      413 2022-04-19 15:35:15.000000 edgetest-pip-tools-2022.4.1/edgetest_pip_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-04-19 15:35:15.000000 edgetest-pip-tools-2022.4.1/edgetest_pip_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      689 2022-04-19 15:34:34.000000 edgetest-pip-tools-2022.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2754 2022-04-19 15:35:15.284051 edgetest-pip-tools-2022.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-04-19 15:34:34.000000 edgetest-pip-tools-2022.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 15:35:15.284051 edgetest-pip-tools-2022.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-19 15:34:34.000000 edgetest-pip-tools-2022.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3909 2022-04-19 15:34:34.000000 edgetest-pip-tools-2022.4.1/tests/test_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:54:42.641824 edgetest-pip-tools-2023.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-23 17:54:09.000000 edgetest-pip-tools-2023.4.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-23 17:54:09.000000 edgetest-pip-tools-2023.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-23 17:54:09.000000 edgetest-pip-tools-2023.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-23 17:54:42.641824 edgetest-pip-tools-2023.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-23 17:54:09.000000 edgetest-pip-tools-2023.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:54:42.637824 edgetest-pip-tools-2023.4.0/edgetest_pip_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-23 17:54:09.000000 edgetest-pip-tools-2023.4.0/edgetest_pip_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-23 17:54:09.000000 edgetest-pip-tools-2023.4.0/edgetest_pip_tools/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:54:42.641824 edgetest-pip-tools-2023.4.0/edgetest_pip_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-23 17:54:42.000000 edgetest-pip-tools-2023.4.0/edgetest_pip_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-23 17:54:42.000000 edgetest-pip-tools-2023.4.0/edgetest_pip_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 17:54:42.000000 edgetest-pip-tools-2023.4.0/edgetest_pip_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-23 17:54:42.000000 edgetest-pip-tools-2023.4.0/edgetest_pip_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 17:54:12.000000 edgetest-pip-tools-2023.4.0/edgetest_pip_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-23 17:54:42.000000 edgetest-pip-tools-2023.4.0/edgetest_pip_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-23 17:54:42.000000 edgetest-pip-tools-2023.4.0/edgetest_pip_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-23 17:54:09.000000 edgetest-pip-tools-2023.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-23 17:54:42.645824 edgetest-pip-tools-2023.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-23 17:54:09.000000 edgetest-pip-tools-2023.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:54:42.641824 edgetest-pip-tools-2023.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 17:54:09.000000 edgetest-pip-tools-2023.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-04-23 17:54:09.000000 edgetest-pip-tools-2023.4.0/tests/test_hook.py
```

### Comparing `edgetest-pip-tools-2022.4.1/LICENSE` & `edgetest-pip-tools-2023.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgetest-pip-tools-2022.4.1/PKG-INFO` & `edgetest-pip-tools-2023.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: edgetest-pip-tools
-Version: 2022.4.1
+Version: 2023.4.0
 Summary: pip-tools integration for edgetest
 Home-page: https://github.com/capitalone/edgetest-pip-tools
 Author: Akshay Gupta
 Author-email: akshay.gupta2@capitalone.com
 Maintainer: Akshay Gupta
 Maintainer-email: akshay.gupta2@capitalone.com
-License: UNKNOWN
 Project-URL: Documentation, https://capitalone.github.io/edgetest-pip-tools/
 Project-URL: Bug Tracker, https://github.com/capitalone/edgetest-pip-tools/issues
 Project-URL: Source Code, https://github.com/capitalone/edgetest-pip-tools
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: qa
 Provides-Extra: build
 Provides-Extra: dev
 License-File: LICENSE
@@ -101,9 +100,7 @@
 By participating, you are expected to honor this code.
 
 License
 -------
 
 Apache-2.0
 
-
-
```

### Comparing `edgetest-pip-tools-2022.4.1/README.md` & `edgetest-pip-tools-2023.4.0/README.md`

 * *Files identical despite different names*

### Comparing `edgetest-pip-tools-2022.4.1/edgetest_pip_tools/plugin.py` & `edgetest-pip-tools-2023.4.0/edgetest_pip_tools/plugin.py`

 * *Files identical despite different names*

### Comparing `edgetest-pip-tools-2022.4.1/edgetest_pip_tools.egg-info/PKG-INFO` & `edgetest-pip-tools-2023.4.0/edgetest_pip_tools.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: edgetest-pip-tools
-Version: 2022.4.1
+Version: 2023.4.0
 Summary: pip-tools integration for edgetest
 Home-page: https://github.com/capitalone/edgetest-pip-tools
 Author: Akshay Gupta
 Author-email: akshay.gupta2@capitalone.com
 Maintainer: Akshay Gupta
 Maintainer-email: akshay.gupta2@capitalone.com
-License: UNKNOWN
 Project-URL: Documentation, https://capitalone.github.io/edgetest-pip-tools/
 Project-URL: Bug Tracker, https://github.com/capitalone/edgetest-pip-tools/issues
 Project-URL: Source Code, https://github.com/capitalone/edgetest-pip-tools
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: qa
 Provides-Extra: build
 Provides-Extra: dev
 License-File: LICENSE
@@ -101,9 +100,7 @@
 By participating, you are expected to honor this code.
 
 License
 -------
 
 Apache-2.0
 
-
-
```

### Comparing `edgetest-pip-tools-2022.4.1/requirements.txt` & `edgetest-pip-tools-2023.4.0/requirements.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 #
-# This file is autogenerated by pip-compile with python 3.9
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.9
+# by the following command:
 #
 #    pip-compile --output-file=requirements.txt setup.cfg
 #
+build==0.10.0
+    # via pip-tools
 cerberus==1.3.4
     # via edgetest
-click==8.0.4
+click==8.1.3
     # via
     #   edgetest
     #   pip-tools
-edgetest==2022.3.1
+edgetest==2023.4.0
     # via edgetest-pip-tools (setup.cfg)
-packaging==21.3
-    # via edgetest
-pep517==0.12.0
-    # via pip-tools
-pip-tools==6.6.0
+packaging==23.0
+    # via
+    #   build
+    #   edgetest
+pip-tools==6.13.0
     # via edgetest-pip-tools (setup.cfg)
 pluggy==1.0.0
     # via edgetest
-pyparsing==3.0.8
-    # via packaging
-tabulate==0.8.9
+pyproject-hooks==1.0.0
+    # via build
+tabulate==0.9.0
     # via edgetest
 tomli==2.0.1
-    # via pep517
-wheel==0.37.1
+    # via build
+tomlkit==0.11.4
+    # via edgetest
+wheel==0.40.0
     # via pip-tools
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `edgetest-pip-tools-2022.4.1/setup.cfg` & `edgetest-pip-tools-2023.4.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -21,22 +21,23 @@
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
 	edgetest
-	pip-tools<=6.6.0,>=6.0.0
+	pip-tools<=6.13.0,>=6.0.0
 
 [options.extras_require]
 docs = 
 	furo
 	sphinx
 	sphinx-copybutton
 	sphinx-tabs
@@ -82,15 +83,15 @@
 	bumpver
 
 [options.entry_points]
 edgetest = 
 	piptools = edgetest_pip_tools.plugin
 
 [bumpver]
-current_version = "2022.4.1"
+current_version = "2023.4.0"
 version_pattern = "YYYY.MM.INC0"
 commit_message = "Bump {old_version} to {new_version}"
 commit = True
 
 [bumpver:file_patterns]
 docs/source/conf.py = 
 	version = "{version}"
```

### Comparing `edgetest-pip-tools-2022.4.1/tests/test_hook.py` & `edgetest-pip-tools-2023.4.0/tests/test_hook.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 """
 
 
 @pytest.mark.parametrize("config", [CFG, CFG_ART, CFG_EXTRAS])
 def test_addoption(config, tmpdir):
     """Test the addoption hook."""
     location = tmpdir.mkdir("mylocation")
-    conf_loc = Path(str(location), "myconfig.ini")
+    conf_loc = Path(str(location), "myconfig.cfg")
     with open(conf_loc, "w") as outfile:
         outfile.write(config)
 
     schema = Schema()
     addoption(schema=schema)
 
     cfg = parse_cfg(filename=conf_loc)
```

