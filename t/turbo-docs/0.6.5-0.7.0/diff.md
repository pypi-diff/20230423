# Comparing `tmp/turbo_docs-0.6.5.tar.gz` & `tmp/turbo_docs-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbo_docs-0.6.5.tar", last modified: Sun Apr 16 16:10:30 2023, max compression
+gzip compressed data, was "dist\turbo_docs-0.7.0.tar", last modified: Sat Apr 22 21:46:40 2023, max compression
```

## Comparing `turbo_docs-0.6.5.tar` & `turbo_docs-0.7.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 16:10:30.741118 turbo_docs-0.6.5/
--rw-rw-rw-   0        0        0     1862 2023-04-16 16:10:30.740124 turbo_docs-0.6.5/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2023-04-16 15:34:04.000000 turbo_docs-0.6.5/README.md
--rw-rw-rw-   0        0        0       42 2023-04-16 16:10:30.742119 turbo_docs-0.6.5/setup.cfg
--rw-rw-rw-   0        0        0      726 2023-04-16 16:09:43.000000 turbo_docs-0.6.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 16:10:30.721076 turbo_docs-0.6.5/turbo_docs/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.6.5/turbo_docs/__init__.py
--rw-rw-rw-   0        0        0     6057 2023-04-16 16:08:18.000000 turbo_docs-0.6.5/turbo_docs/generate.py
-drwxrwxrwx   0        0        0        0 2023-04-16 16:10:30.738120 turbo_docs-0.6.5/turbo_docs/utils/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.6.5/turbo_docs/utils/__init__.py
--rw-rw-rw-   0        0        0     1471 2023-04-16 15:13:12.000000 turbo_docs-0.6.5/turbo_docs/utils/cli_options.py
--rw-rw-rw-   0        0        0     1624 2023-04-16 15:18:24.000000 turbo_docs-0.6.5/turbo_docs/utils/directory.py
--rw-rw-rw-   0        0        0      763 2023-04-16 15:13:17.000000 turbo_docs-0.6.5/turbo_docs/utils/openai_api.py
-drwxrwxrwx   0        0        0        0 2023-04-16 16:10:30.731078 turbo_docs-0.6.5/turbo_docs.egg-info/
--rw-rw-rw-   0        0        0     1862 2023-04-16 16:10:30.000000 turbo_docs-0.6.5/turbo_docs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-04-16 16:10:30.000000 turbo_docs-0.6.5/turbo_docs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 16:10:30.000000 turbo_docs-0.6.5/turbo_docs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-04-16 16:10:30.000000 turbo_docs-0.6.5/turbo_docs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-04-16 16:10:30.000000 turbo_docs-0.6.5/turbo_docs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-16 16:10:30.000000 turbo_docs-0.6.5/turbo_docs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-22 21:46:40.407364 turbo_docs-0.7.0/
+-rw-rw-rw-   0        0        0     2010 2023-04-22 21:46:40.406364 turbo_docs-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1554 2023-04-22 21:44:40.000000 turbo_docs-0.7.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-22 21:46:40.408363 turbo_docs-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0      757 2023-04-22 21:45:22.000000 turbo_docs-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 21:46:40.386762 turbo_docs-0.7.0/turbo_docs/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.7.0/turbo_docs/__init__.py
+-rw-rw-rw-   0        0        0     1993 2023-04-22 21:31:08.000000 turbo_docs-0.7.0/turbo_docs/generate.py
+drwxrwxrwx   0        0        0        0 2023-04-22 21:46:40.404364 turbo_docs-0.7.0/turbo_docs/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.7.0/turbo_docs/utils/__init__.py
+-rw-rw-rw-   0        0        0     1820 2023-04-22 21:27:40.000000 turbo_docs-0.7.0/turbo_docs/utils/cli_options.py
+-rw-rw-rw-   0        0        0     1928 2023-04-22 21:27:45.000000 turbo_docs-0.7.0/turbo_docs/utils/directory.py
+-rw-rw-rw-   0        0        0     1415 2023-04-22 21:35:25.000000 turbo_docs-0.7.0/turbo_docs/utils/openai_api.py
+drwxrwxrwx   0        0        0        0 2023-04-22 21:46:40.394726 turbo_docs-0.7.0/turbo_docs.egg-info/
+-rw-rw-rw-   0        0        0     2010 2023-04-22 21:46:40.000000 turbo_docs-0.7.0/turbo_docs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-04-22 21:46:40.000000 turbo_docs-0.7.0/turbo_docs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 21:46:40.000000 turbo_docs-0.7.0/turbo_docs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-04-22 21:46:40.000000 turbo_docs-0.7.0/turbo_docs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2023-04-22 21:46:40.000000 turbo_docs-0.7.0/turbo_docs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-22 21:46:40.000000 turbo_docs-0.7.0/turbo_docs.egg-info/top_level.txt
```

### Comparing `turbo_docs-0.6.5/setup.py` & `turbo_docs-0.7.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
 	name="turbo_docs",
-	version="0.6.5",
+	version="0.7.0",
 	packages=find_packages(),
 	install_requires=[
 		"requests",
 		"openai",
 		"click",
 		"pyperclip",
+		"redbaron",
+		"gitpython",
 	],
 	entry_points={
 		"console_scripts": [
 			"turbo_docs=turbo_docs.generate:driver"
 		],
 	},
 	classifiers=[
```

### Comparing `turbo_docs-0.6.5/turbo_docs/utils/cli_options.py` & `turbo_docs-0.7.0/turbo_docs/utils/cli_options.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,58 +1,68 @@
 import click
 from typing import Callable
 
 def copy(func: Callable) -> Callable:
-	"""
-    Create a click option to support copying directory text to the clipboard.
     """
-	return click.option(
-		'--copy',
-		default=False,
-		is_flag=True,
-		help='Copy the directory text to clipboard'
-	)(func)
-
-def create_readme(func: Callable) -> Callable:
-	"""
-    Add a --create_readme flag for a function, which when set to true, will generate
-    a README.md file
-    """
-	return click.option(
-		'--create_readme',
-		default=False,
-		is_flag=True,
-		help='Generate README.md file'
-	)(func)
-
-def create_readme_plus(func: Callable) -> Callable:
-	"""
-    Wrap a function to provide flag to generate readme for larger repositories.
-    """
-	return click.option(
-		'--create_readme_plus',
-		default=False,
-		is_flag=True,
-		help='Generate readme for larger repositories'
-	)(func)
-
-def create_tests(func: Callable) -> Callable:
-	"""
-    Create a command line flag to generate unit tests for each code file.
-    """
-	return click.option(
-		'--create_tests',
-		default=False,
-		is_flag=True,
-		help='Generate unit tests for each code file'
-	)(func)
-
-def create_docstring(func: Callable) -> Callable:
-	"""
-    Generate and insert docstrings for each function using GPT.
-    """
-	return click.option(
-		'--create_docstring',
-		default=False,
-		is_flag=True,
-		help='Generate and insert docstrings for each function using GPT'
-	)(func)
+    Create a click option to enable the user to copy directory text to clipboard
+    """
+    return click.option(
+        '--copy',
+        default=False,
+        is_flag=True,
+        help='Copy the directory text to clipboard'
+    )(func)
+
+def readme(func: Callable) -> Callable:
+    """
+    Decorate a function with the `--readme` option to generate a README.md file.
+    """
+    return click.option(
+        '--readme',
+        default=False,
+        is_flag=True,
+        help='Generate README.md file'
+    )(func)
+
+def readme_large_repo(func: Callable) -> Callable:
+    """
+    Run function to generate README for larger repositories.
+    """
+    return click.option(
+        '--readme_large_repo',
+        default=False,
+        is_flag=True,
+        help='Generate readme for larger repositories'
+    )(func)
+
+def unit_tests(func: Callable) -> Callable:
+    """
+    Enable generation of unit tests for each code file.
+    """
+    return click.option(
+        '--unit_tests',
+        default=False,
+        is_flag=True,
+        help='Generate unit tests for each code file'
+    )(func)
+
+def docstring(func: Callable) -> Callable:
+    """
+    Autogenerate docstrings for functions.
+    """
+    return click.option(
+        '--docstring',
+        default=False,
+        is_flag=True,
+        help='Generate and insert docstrings for each function'
+    )(func)
+
+def commit(func: Callable) -> Callable:
+    """
+    Decorate a function to generate a commit message and execute a commit.
+    """
+    return click.option(
+        '--commit',
+        default=False,
+        is_flag=True,
+        help='Generate a commit message and execute the commit'
+    )(func)
```

### Comparing `turbo_docs-0.6.5/turbo_docs/utils/directory.py` & `turbo_docs-0.7.0/turbo_docs/utils/directory.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,64 @@
 import json
 import os
 from pathlib import Path
 from typing import List, Dict
 
+
 def ignored_files_init() -> List[str]:
-	"""
-    Initialize the list of files to be ignored.
     """
-	ignored_files = ["README.md", "tests", "setup.py"]
-	for file in os.listdir():
-		if file[0] == ".":
-			ignored_files.append(file)
-	return ignored_files
+    Initializes a list of ignored files from current directory.
+    """
+    ignored_files = ["README.md", "tests", "setup.py"]
+    for file in os.listdir():
+        if file[0] == ".":
+            ignored_files.append(file)
+    return ignored_files
+
 
 def read_gitignore() -> List[str]:
-	"""
-    Read .gitignore file and return a list of ignored files.
     """
-	ignore_files = ignored_files_init()
-	try:
-		with open(".gitignore", "r") as gitignore:
-			for line in gitignore:
-				ignore_files.append(line.strip())
-	except FileNotFoundError:
-		raise ValueError(".gitignore file required for excluding files from documentation generation")
-	return ignore_files
+    Read '.gitignore' file and return a list of files to be excluded from
+    documentation generation.
+    """
+    ignore_files = ignored_files_init()
+    try:
+        with open(".gitignore", "r") as gitignore:
+            for line in gitignore:
+                ignore_files.append(line.strip())
+    except FileNotFoundError:
+        raise ValueError(
+            ".gitignore file required for excluding files from documentation generation")
+    return ignore_files
+
 
 def ignore_filepath(filepath: str, ignore_files: List[str]) -> bool:
-	"""
-    Checks if a filepath includes a particular file or folder to ignore.
     """
-	for part in Path(filepath).parts:
-		if part in ignore_files:
-			return True
-	return False
+    Check a file path to see if it should be ignored
+    """
+    for part in Path(filepath).parts:
+        if part in ignore_files:
+            return True
+    return False
+
 
 def get_files() -> Dict:
-	"""
-    Retrieve files from directory ignoring items from .gitignore and formatting tab
-    indentation.
-    """
-	files_dict = {}
-	ignore_files = read_gitignore()
-
-	# Iterate over files
-	for root, _, files in os.walk("."):
-		for file in files:
-			filepath = os.path.join(root, file).replace(".\\", "")
-
-			# If not in ignore, collect file text
-			if not ignore_filepath(filepath, ignore_files):
-				with open(filepath, "r") as f:
-					content = f.read()
-				if content:
-					files_dict[filepath] = content.replace(" " * 4, "\t").strip()
-	return files_dict
+    """
+    Retrieve and return all files in the working directory, ignoring those specified
+    in the .gitignore file.
+    """
+    files_dict = {}
+    ignore_files = read_gitignore()
+
+    # Iterate over files
+    for root, _, files in os.walk("."):
+        for file in files:
+            filepath = os.path.join(root, file).replace(".\\", "")
+
+            # If not in ignore, collect file text
+            if not ignore_filepath(filepath, ignore_files):
+                with open(filepath, "r") as f:
+                    content = f.read()
+                if content:
+                    files_dict[filepath] = content.replace(
+                        " " * 4, "\t").strip()
+    return files_dict
```

