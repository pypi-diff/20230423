# Comparing `tmp/supadef-0.0.8.tar.gz` & `tmp/supadef-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supadef-0.0.8.tar", last modified: Sat Feb  4 22:39:08 2023, max compression
+gzip compressed data, was "supadef-0.0.9.tar", last modified: Fri Feb 17 22:28:56 2023, max compression
```

## Comparing `supadef-0.0.8.tar` & `supadef-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 connormclaughlin   (501) staff       (20)        0 2023-02-04 22:39:08.300890 supadef-0.0.8/
--rw-r--r--   0 connormclaughlin   (501) staff       (20)     1069 2023-01-08 01:05:32.000000 supadef-0.0.8/LICENSE
--rw-r--r--   0 connormclaughlin   (501) staff       (20)      512 2023-02-04 22:39:08.300764 supadef-0.0.8/PKG-INFO
--rw-r--r--   0 connormclaughlin   (501) staff       (20)       74 2023-01-08 01:00:10.000000 supadef-0.0.8/README.md
--rw-r--r--   0 connormclaughlin   (501) staff       (20)      898 2023-02-04 22:38:30.000000 supadef-0.0.8/pyproject.toml
--rw-r--r--   0 connormclaughlin   (501) staff       (20)       38 2023-02-04 22:39:08.300926 supadef-0.0.8/setup.cfg
-drwxr-xr-x   0 connormclaughlin   (501) staff       (20)        0 2023-02-04 22:39:08.299769 supadef-0.0.8/supadef/
--rw-r--r--   0 connormclaughlin   (501) staff       (20)      210 2023-02-02 19:24:07.000000 supadef-0.0.8/supadef/__init__.py
--rw-r--r--   0 connormclaughlin   (501) staff       (20)     2365 2023-02-04 22:38:20.000000 supadef-0.0.8/supadef/cli.py
--rw-r--r--   0 connormclaughlin   (501) staff       (20)      123 2023-02-02 20:28:19.000000 supadef-0.0.8/supadef/credentials.py
-drwxr-xr-x   0 connormclaughlin   (501) staff       (20)        0 2023-02-04 22:39:08.300625 supadef-0.0.8/supadef.egg-info/
--rw-r--r--   0 connormclaughlin   (501) staff       (20)      512 2023-02-04 22:39:08.000000 supadef-0.0.8/supadef.egg-info/PKG-INFO
--rw-r--r--   0 connormclaughlin   (501) staff       (20)      278 2023-02-04 22:39:08.000000 supadef-0.0.8/supadef.egg-info/SOURCES.txt
--rw-r--r--   0 connormclaughlin   (501) staff       (20)        1 2023-02-04 22:39:08.000000 supadef-0.0.8/supadef.egg-info/dependency_links.txt
--rw-r--r--   0 connormclaughlin   (501) staff       (20)       44 2023-02-04 22:39:08.000000 supadef-0.0.8/supadef.egg-info/entry_points.txt
--rw-r--r--   0 connormclaughlin   (501) staff       (20)       55 2023-02-04 22:39:08.000000 supadef-0.0.8/supadef.egg-info/requires.txt
--rw-r--r--   0 connormclaughlin   (501) staff       (20)        8 2023-02-04 22:39:08.000000 supadef-0.0.8/supadef.egg-info/top_level.txt
+drwxr-xr-x   0 connormclaughlin   (501) staff       (20)        0 2023-02-17 22:28:56.625726 supadef-0.0.9/
+-rw-r--r--   0 connormclaughlin   (501) staff       (20)     1069 2023-01-08 01:05:32.000000 supadef-0.0.9/LICENSE
+-rw-r--r--   0 connormclaughlin   (501) staff       (20)      512 2023-02-17 22:28:56.625590 supadef-0.0.9/PKG-INFO
+-rw-r--r--   0 connormclaughlin   (501) staff       (20)       74 2023-01-08 01:00:10.000000 supadef-0.0.9/README.md
+-rw-r--r--   0 connormclaughlin   (501) staff       (20)      898 2023-02-17 22:28:37.000000 supadef-0.0.9/pyproject.toml
+-rw-r--r--   0 connormclaughlin   (501) staff       (20)       38 2023-02-17 22:28:56.625774 supadef-0.0.9/setup.cfg
+drwxr-xr-x   0 connormclaughlin   (501) staff       (20)        0 2023-02-17 22:28:56.624178 supadef-0.0.9/supadef/
+-rw-r--r--   0 connormclaughlin   (501) staff       (20)      210 2023-02-02 19:24:07.000000 supadef-0.0.9/supadef/__init__.py
+-rw-r--r--   0 connormclaughlin   (501) staff       (20)     2442 2023-02-17 16:55:10.000000 supadef-0.0.9/supadef/cli.py
+-rw-r--r--   0 connormclaughlin   (501) staff       (20)      123 2023-02-02 20:28:19.000000 supadef-0.0.9/supadef/credentials.py
+drwxr-xr-x   0 connormclaughlin   (501) staff       (20)        0 2023-02-17 22:28:56.625166 supadef-0.0.9/supadef.egg-info/
+-rw-r--r--   0 connormclaughlin   (501) staff       (20)      512 2023-02-17 22:28:56.000000 supadef-0.0.9/supadef.egg-info/PKG-INFO
+-rw-r--r--   0 connormclaughlin   (501) staff       (20)      310 2023-02-17 22:28:56.000000 supadef-0.0.9/supadef.egg-info/SOURCES.txt
+-rw-r--r--   0 connormclaughlin   (501) staff       (20)        1 2023-02-17 22:28:56.000000 supadef-0.0.9/supadef.egg-info/dependency_links.txt
+-rw-r--r--   0 connormclaughlin   (501) staff       (20)       44 2023-02-17 22:28:56.000000 supadef-0.0.9/supadef.egg-info/entry_points.txt
+-rw-r--r--   0 connormclaughlin   (501) staff       (20)       55 2023-02-17 22:28:56.000000 supadef-0.0.9/supadef.egg-info/requires.txt
+-rw-r--r--   0 connormclaughlin   (501) staff       (20)        8 2023-02-17 22:28:56.000000 supadef-0.0.9/supadef.egg-info/top_level.txt
+drwxr-xr-x   0 connormclaughlin   (501) staff       (20)        0 2023-02-17 22:28:56.625304 supadef-0.0.9/tests/
+-rw-r--r--   0 connormclaughlin   (501) staff       (20)      215 2023-02-02 20:16:10.000000 supadef-0.0.9/tests/test_parse_credentials.py
```

### Comparing `supadef-0.0.8/LICENSE` & `supadef-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `supadef-0.0.8/PKG-INFO` & `supadef-0.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supadef
-Version: 0.0.8
+Version: 0.0.9
 Summary: Official command-line interface for supadef ⚡️
 Author-email: Connor McLaughlin <connor@fractall.com>
 Project-URL: Homepage, https://github.com/connormcl/supadef_cli
 Project-URL: Bug Tracker, https://github.com/connormcl/supadef_cli/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `supadef-0.0.8/pyproject.toml` & `supadef-0.0.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "supadef"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Connor McLaughlin", email="connor@fractall.com" },
 ]
 description = "Official command-line interface for supadef ⚡️"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `supadef-0.0.8/supadef/cli.py` & `supadef-0.0.9/supadef/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import os
 import subprocess
 import requests
 from typer import Typer
 from .credentials import parse_credentials
 
 
+TIMEOUT_SECONDS = 3 * 60
+
+
 def execute_bash_command(cmd):
     print(cmd)
     process = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     stdout, stderr = process.communicate()
     if process.returncode != 0:
         raise subprocess.CalledProcessError(process.returncode, cmd, output=stdout, stderr=stderr)
     return stdout.decode().strip()
@@ -53,26 +56,26 @@
     """create a new project"""
     # 1.
     execute_bash_command(f'mkdir -p {project_name}')
     execute_bash_command(f'touch {project_name}/supadef.yml')
     body = {
         'name': project_name
     }
-    response = requests.post("https://supadef.com/project", headers=get_auth_headers(), json=body)
+    response = requests.post("https://supadef.com/project", headers=get_auth_headers(), json=body, timeout=TIMEOUT_SECONDS)
     print(response.status_code)
     print(response.json())
 
 
 @app.command()
 def destroy(project_name: str):
     """destroy a project"""
     body = {
         'name': project_name
     }
-    response = requests.delete("https://supadef.com/project", headers=get_auth_headers(), json=body)
+    response = requests.delete("https://supadef.com/project", headers=get_auth_headers(), json=body, timeout=TIMEOUT_SECONDS)
     print(response.status_code)
     print(response.json())
 
 
 @app.command()
 def projects():
     """list your projects"""
```

### Comparing `supadef-0.0.8/supadef.egg-info/PKG-INFO` & `supadef-0.0.9/supadef.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supadef
-Version: 0.0.8
+Version: 0.0.9
 Summary: Official command-line interface for supadef ⚡️
 Author-email: Connor McLaughlin <connor@fractall.com>
 Project-URL: Homepage, https://github.com/connormcl/supadef_cli
 Project-URL: Bug Tracker, https://github.com/connormcl/supadef_cli/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

