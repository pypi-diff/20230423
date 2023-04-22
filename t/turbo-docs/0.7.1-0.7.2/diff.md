# Comparing `tmp/turbo_docs-0.7.1.tar.gz` & `tmp/turbo_docs-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbo_docs-0.7.1.tar", last modified: Sat Apr 22 21:55:08 2023, max compression
+gzip compressed data, was "dist\turbo_docs-0.7.2.tar", last modified: Sat Apr 22 22:02:27 2023, max compression
```

## Comparing `turbo_docs-0.7.1.tar` & `turbo_docs-0.7.2.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 21:55:08.224864 turbo_docs-0.7.1/
--rw-rw-rw-   0        0        0     2067 2023-04-22 21:55:08.223864 turbo_docs-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0     1554 2023-04-22 21:44:40.000000 turbo_docs-0.7.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-22 21:55:08.224864 turbo_docs-0.7.1/setup.cfg
--rw-rw-rw-   0        0        0      757 2023-04-22 21:55:03.000000 turbo_docs-0.7.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-22 21:55:08.205856 turbo_docs-0.7.1/turbo_docs/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.7.1/turbo_docs/__init__.py
--rw-rw-rw-   0        0        0     2017 2023-04-22 21:54:25.000000 turbo_docs-0.7.1/turbo_docs/generate.py
-drwxrwxrwx   0        0        0        0 2023-04-22 21:55:08.221856 turbo_docs-0.7.1/turbo_docs/utils/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.7.1/turbo_docs/utils/__init__.py
--rw-rw-rw-   0        0        0     1820 2023-04-22 21:27:40.000000 turbo_docs-0.7.1/turbo_docs/utils/cli_options.py
--rw-rw-rw-   0        0        0     1928 2023-04-22 21:27:45.000000 turbo_docs-0.7.1/turbo_docs/utils/directory.py
--rw-rw-rw-   0        0        0     1415 2023-04-22 21:35:25.000000 turbo_docs-0.7.1/turbo_docs/utils/openai_api.py
-drwxrwxrwx   0        0        0        0 2023-04-22 21:55:08.215856 turbo_docs-0.7.1/turbo_docs.egg-info/
--rw-rw-rw-   0        0        0     2067 2023-04-22 21:55:07.000000 turbo_docs-0.7.1/turbo_docs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-04-22 21:55:08.000000 turbo_docs-0.7.1/turbo_docs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 21:55:07.000000 turbo_docs-0.7.1/turbo_docs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-04-22 21:55:08.000000 turbo_docs-0.7.1/turbo_docs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2023-04-22 21:55:08.000000 turbo_docs-0.7.1/turbo_docs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-22 21:55:08.000000 turbo_docs-0.7.1/turbo_docs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-22 22:02:27.424419 turbo_docs-0.7.2/
+-rw-rw-rw-   0        0        0     2010 2023-04-22 22:02:27.423420 turbo_docs-0.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1554 2023-04-22 21:44:40.000000 turbo_docs-0.7.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-22 22:02:27.424419 turbo_docs-0.7.2/setup.cfg
+-rw-rw-rw-   0        0        0      757 2023-04-22 22:02:18.000000 turbo_docs-0.7.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 22:02:27.393989 turbo_docs-0.7.2/turbo_docs/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.7.2/turbo_docs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 22:02:27.413897 turbo_docs-0.7.2/turbo_docs/commands/
+-rw-rw-rw-   0        0        0        0 2023-04-22 22:02:08.000000 turbo_docs-0.7.2/turbo_docs/commands/__init__.py
+-rw-rw-rw-   0        0        0     2078 2023-04-22 21:34:48.000000 turbo_docs-0.7.2/turbo_docs/commands/commit.py
+-rw-rw-rw-   0        0        0     2162 2023-04-22 21:34:03.000000 turbo_docs-0.7.2/turbo_docs/commands/docstring.py
+-rw-rw-rw-   0        0        0     1590 2023-04-22 21:33:13.000000 turbo_docs-0.7.2/turbo_docs/commands/readme.py
+-rw-rw-rw-   0        0        0     1133 2023-04-22 21:31:48.000000 turbo_docs-0.7.2/turbo_docs/commands/unit_tests.py
+-rw-rw-rw-   0        0        0     2017 2023-04-22 21:54:25.000000 turbo_docs-0.7.2/turbo_docs/generate.py
+drwxrwxrwx   0        0        0        0 2023-04-22 22:02:27.421428 turbo_docs-0.7.2/turbo_docs/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.7.2/turbo_docs/utils/__init__.py
+-rw-rw-rw-   0        0        0     1820 2023-04-22 21:27:40.000000 turbo_docs-0.7.2/turbo_docs/utils/cli_options.py
+-rw-rw-rw-   0        0        0     1928 2023-04-22 21:27:45.000000 turbo_docs-0.7.2/turbo_docs/utils/directory.py
+-rw-rw-rw-   0        0        0     1415 2023-04-22 21:35:25.000000 turbo_docs-0.7.2/turbo_docs/utils/openai_api.py
+drwxrwxrwx   0        0        0        0 2023-04-22 22:02:27.405518 turbo_docs-0.7.2/turbo_docs.egg-info/
+-rw-rw-rw-   0        0        0     2010 2023-04-22 22:02:27.000000 turbo_docs-0.7.2/turbo_docs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-04-22 22:02:27.000000 turbo_docs-0.7.2/turbo_docs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 22:02:27.000000 turbo_docs-0.7.2/turbo_docs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-04-22 22:02:27.000000 turbo_docs-0.7.2/turbo_docs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2023-04-22 22:02:27.000000 turbo_docs-0.7.2/turbo_docs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-22 22:02:27.000000 turbo_docs-0.7.2/turbo_docs.egg-info/top_level.txt
```

### Comparing `turbo_docs-0.7.1/PKG-INFO` & `turbo_docs-0.7.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 Metadata-Version: 2.1
 Name: turbo_docs
-Version: 0.7.1
-Summary: UNKNOWN
-License: UNKNOWN
-Platform: UNKNOWN
+Version: 0.7.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -57,8 +54,7 @@
 - `--commit`: Generate a commit message and execute the commit
 
 ## Contributing
 
 If you would like to contribute to Turbo Docs, please feel free to open a pull request
 
 Or each out to me at voynow99@gmail.com, https://www.linkedin.com/in/voynow/, or https://twitter.com/JamesVoynow!
-
```

### Comparing `turbo_docs-0.7.1/README.md` & `turbo_docs-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.7.1/setup.py` & `turbo_docs-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 	name="turbo_docs",
-	version="0.7.1",
+	version="0.7.2",
 	packages=find_packages(),
 	install_requires=[
 		"requests",
 		"openai",
 		"click",
 		"pyperclip",
 		"redbaron",
```

### Comparing `turbo_docs-0.7.1/turbo_docs/generate.py` & `turbo_docs-0.7.2/turbo_docs/generate.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.7.1/turbo_docs/utils/cli_options.py` & `turbo_docs-0.7.2/turbo_docs/utils/cli_options.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.7.1/turbo_docs/utils/directory.py` & `turbo_docs-0.7.2/turbo_docs/utils/directory.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.7.1/turbo_docs/utils/openai_api.py` & `turbo_docs-0.7.2/turbo_docs/utils/openai_api.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.7.1/turbo_docs.egg-info/PKG-INFO` & `turbo_docs-0.7.2/turbo_docs.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 Metadata-Version: 2.1
 Name: turbo-docs
-Version: 0.7.1
-Summary: UNKNOWN
-License: UNKNOWN
-Platform: UNKNOWN
+Version: 0.7.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -57,8 +54,7 @@
 - `--commit`: Generate a commit message and execute the commit
 
 ## Contributing
 
 If you would like to contribute to Turbo Docs, please feel free to open a pull request
 
 Or each out to me at voynow99@gmail.com, https://www.linkedin.com/in/voynow/, or https://twitter.com/JamesVoynow!
-
```

