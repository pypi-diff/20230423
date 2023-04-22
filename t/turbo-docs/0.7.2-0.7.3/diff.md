# Comparing `tmp/turbo_docs-0.7.2.tar.gz` & `tmp/turbo_docs-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\turbo_docs-0.7.2.tar", last modified: Sat Apr 22 22:02:27 2023, max compression
+gzip compressed data, was "dist\turbo_docs-0.7.3.tar", last modified: Sat Apr 22 22:59:11 2023, max compression
```

## Comparing `turbo_docs-0.7.2.tar` & `turbo_docs-0.7.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 22:02:27.424419 turbo_docs-0.7.2/
--rw-rw-rw-   0        0        0     2010 2023-04-22 22:02:27.423420 turbo_docs-0.7.2/PKG-INFO
--rw-rw-rw-   0        0        0     1554 2023-04-22 21:44:40.000000 turbo_docs-0.7.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-22 22:02:27.424419 turbo_docs-0.7.2/setup.cfg
--rw-rw-rw-   0        0        0      757 2023-04-22 22:02:18.000000 turbo_docs-0.7.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-22 22:02:27.393989 turbo_docs-0.7.2/turbo_docs/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.7.2/turbo_docs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 22:02:27.413897 turbo_docs-0.7.2/turbo_docs/commands/
--rw-rw-rw-   0        0        0        0 2023-04-22 22:02:08.000000 turbo_docs-0.7.2/turbo_docs/commands/__init__.py
--rw-rw-rw-   0        0        0     2078 2023-04-22 21:34:48.000000 turbo_docs-0.7.2/turbo_docs/commands/commit.py
--rw-rw-rw-   0        0        0     2162 2023-04-22 21:34:03.000000 turbo_docs-0.7.2/turbo_docs/commands/docstring.py
--rw-rw-rw-   0        0        0     1590 2023-04-22 21:33:13.000000 turbo_docs-0.7.2/turbo_docs/commands/readme.py
--rw-rw-rw-   0        0        0     1133 2023-04-22 21:31:48.000000 turbo_docs-0.7.2/turbo_docs/commands/unit_tests.py
--rw-rw-rw-   0        0        0     2017 2023-04-22 21:54:25.000000 turbo_docs-0.7.2/turbo_docs/generate.py
-drwxrwxrwx   0        0        0        0 2023-04-22 22:02:27.421428 turbo_docs-0.7.2/turbo_docs/utils/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.7.2/turbo_docs/utils/__init__.py
--rw-rw-rw-   0        0        0     1820 2023-04-22 21:27:40.000000 turbo_docs-0.7.2/turbo_docs/utils/cli_options.py
--rw-rw-rw-   0        0        0     1928 2023-04-22 21:27:45.000000 turbo_docs-0.7.2/turbo_docs/utils/directory.py
--rw-rw-rw-   0        0        0     1415 2023-04-22 21:35:25.000000 turbo_docs-0.7.2/turbo_docs/utils/openai_api.py
-drwxrwxrwx   0        0        0        0 2023-04-22 22:02:27.405518 turbo_docs-0.7.2/turbo_docs.egg-info/
--rw-rw-rw-   0        0        0     2010 2023-04-22 22:02:27.000000 turbo_docs-0.7.2/turbo_docs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2023-04-22 22:02:27.000000 turbo_docs-0.7.2/turbo_docs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 22:02:27.000000 turbo_docs-0.7.2/turbo_docs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-04-22 22:02:27.000000 turbo_docs-0.7.2/turbo_docs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2023-04-22 22:02:27.000000 turbo_docs-0.7.2/turbo_docs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-22 22:02:27.000000 turbo_docs-0.7.2/turbo_docs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-22 22:59:11.092223 turbo_docs-0.7.3/
+-rw-rw-rw-   0        0        0     2010 2023-04-22 22:59:11.091223 turbo_docs-0.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1554 2023-04-22 21:44:40.000000 turbo_docs-0.7.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-22 22:59:11.092223 turbo_docs-0.7.3/setup.cfg
+-rw-rw-rw-   0        0        0      757 2023-04-22 22:58:57.000000 turbo_docs-0.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 22:59:11.065692 turbo_docs-0.7.3/turbo_docs/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.7.3/turbo_docs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 22:59:11.084221 turbo_docs-0.7.3/turbo_docs/commands/
+-rw-rw-rw-   0        0        0        0 2023-04-22 22:02:08.000000 turbo_docs-0.7.3/turbo_docs/commands/__init__.py
+-rw-rw-rw-   0        0        0     2078 2023-04-22 21:34:48.000000 turbo_docs-0.7.3/turbo_docs/commands/commit.py
+-rw-rw-rw-   0        0        0     2162 2023-04-22 21:34:03.000000 turbo_docs-0.7.3/turbo_docs/commands/docstring.py
+-rw-rw-rw-   0        0        0     1590 2023-04-22 21:33:13.000000 turbo_docs-0.7.3/turbo_docs/commands/readme.py
+-rw-rw-rw-   0        0        0     1133 2023-04-22 21:31:48.000000 turbo_docs-0.7.3/turbo_docs/commands/unit_tests.py
+-rw-rw-rw-   0        0        0     1993 2023-04-22 22:58:45.000000 turbo_docs-0.7.3/turbo_docs/generate.py
+drwxrwxrwx   0        0        0        0 2023-04-22 22:59:11.089219 turbo_docs-0.7.3/turbo_docs/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.7.3/turbo_docs/utils/__init__.py
+-rw-rw-rw-   0        0        0     1820 2023-04-22 21:27:40.000000 turbo_docs-0.7.3/turbo_docs/utils/cli_options.py
+-rw-rw-rw-   0        0        0     1928 2023-04-22 21:27:45.000000 turbo_docs-0.7.3/turbo_docs/utils/directory.py
+-rw-rw-rw-   0        0        0     1415 2023-04-22 21:35:25.000000 turbo_docs-0.7.3/turbo_docs/utils/openai_api.py
+drwxrwxrwx   0        0        0        0 2023-04-22 22:59:11.074707 turbo_docs-0.7.3/turbo_docs.egg-info/
+-rw-rw-rw-   0        0        0     2010 2023-04-22 22:59:10.000000 turbo_docs-0.7.3/turbo_docs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-04-22 22:59:11.000000 turbo_docs-0.7.3/turbo_docs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 22:59:10.000000 turbo_docs-0.7.3/turbo_docs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-04-22 22:59:10.000000 turbo_docs-0.7.3/turbo_docs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2023-04-22 22:59:10.000000 turbo_docs-0.7.3/turbo_docs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-22 22:59:10.000000 turbo_docs-0.7.3/turbo_docs.egg-info/top_level.txt
```

### Comparing `turbo_docs-0.7.2/PKG-INFO` & `turbo_docs-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbo_docs
-Version: 0.7.2
+Version: 0.7.3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `turbo_docs-0.7.2/README.md` & `turbo_docs-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.7.2/setup.py` & `turbo_docs-0.7.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 	name="turbo_docs",
-	version="0.7.2",
+	version="0.7.3",
 	packages=find_packages(),
 	install_requires=[
 		"requests",
 		"openai",
 		"click",
 		"pyperclip",
 		"redbaron",
```

### Comparing `turbo_docs-0.7.2/turbo_docs/commands/commit.py` & `turbo_docs-0.7.3/turbo_docs/commands/commit.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.7.2/turbo_docs/commands/docstring.py` & `turbo_docs-0.7.3/turbo_docs/commands/docstring.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.7.2/turbo_docs/commands/readme.py` & `turbo_docs-0.7.3/turbo_docs/commands/readme.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.7.2/turbo_docs/commands/unit_tests.py` & `turbo_docs-0.7.3/turbo_docs/commands/unit_tests.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.7.2/turbo_docs/generate.py` & `turbo_docs-0.7.3/turbo_docs/generate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import click
 import pyperclip
-from turbo_docs.utils.commands import commit as commit_module
-from turbo_docs.utils.commands import docstring as docstring_module
-from turbo_docs.utils.commands import readme as readme_module
-from turbo_docs.utils.commands import unit_tests as unit_tests_module
+from turbo_docs.commands import commit as commit_module
+from turbo_docs.commands import docstring as docstring_module
+from turbo_docs.commands import readme as readme_module
+from turbo_docs.commands import unit_tests as unit_tests_module
 from turbo_docs.utils import directory, cli_options
 
 
 @click.command()
 @cli_options.copy
 @cli_options.readme
 @cli_options.readme_large_repo
```

### Comparing `turbo_docs-0.7.2/turbo_docs/utils/cli_options.py` & `turbo_docs-0.7.3/turbo_docs/utils/cli_options.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.7.2/turbo_docs/utils/directory.py` & `turbo_docs-0.7.3/turbo_docs/utils/directory.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.7.2/turbo_docs/utils/openai_api.py` & `turbo_docs-0.7.3/turbo_docs/utils/openai_api.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.7.2/turbo_docs.egg-info/PKG-INFO` & `turbo_docs-0.7.3/turbo_docs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbo-docs
-Version: 0.7.2
+Version: 0.7.3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `turbo_docs-0.7.2/turbo_docs.egg-info/SOURCES.txt` & `turbo_docs-0.7.3/turbo_docs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

