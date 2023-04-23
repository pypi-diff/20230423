# Comparing `tmp/quinten-cli-1.0.4.tar.gz` & `tmp/quinten-cli-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quinten-cli-1.0.4.tar", last modified: Sun Mar  5 20:54:16 2023, max compression
+gzip compressed data, was "quinten-cli-1.1.0.tar", last modified: Sun Apr 23 18:25:00 2023, max compression
```

## Comparing `quinten-cli-1.0.4.tar` & `quinten-cli-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-03-05 20:54:16.281652 quinten-cli-1.0.4/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1069 2023-03-05 20:15:30.000000 quinten-cli-1.0.4/LICENSE
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      269 2023-03-05 20:54:16.281652 quinten-cli-1.0.4/PKG-INFO
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      322 2023-03-05 20:15:30.000000 quinten-cli-1.0.4/README.md
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-03-05 20:54:16.277651 quinten-cli-1.0.4/cli/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      925 2023-03-05 20:18:29.000000 quinten-cli-1.0.4/cli/__init__.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      157 2023-03-05 20:15:30.000000 quinten-cli-1.0.4/cli/env.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      625 2023-03-05 20:15:30.000000 quinten-cli-1.0.4/cli/input_interface.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      741 2023-03-05 20:15:30.000000 quinten-cli-1.0.4/cli/install.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1241 2023-03-05 20:15:30.000000 quinten-cli-1.0.4/cli/output_interface.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1483 2023-03-05 20:15:30.000000 quinten-cli-1.0.4/cli/progress.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     4999 2023-03-05 20:15:30.000000 quinten-cli-1.0.4/cli/run.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      366 2023-03-05 20:15:30.000000 quinten-cli-1.0.4/cli/status.py
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-03-05 20:54:16.281652 quinten-cli-1.0.4/quinten_cli.egg-info/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      269 2023-03-05 20:54:16.000000 quinten-cli-1.0.4/quinten_cli.egg-info/PKG-INFO
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      394 2023-03-05 20:54:16.000000 quinten-cli-1.0.4/quinten_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)        1 2023-03-05 20:54:16.000000 quinten-cli-1.0.4/quinten_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       44 2023-03-05 20:54:16.000000 quinten-cli-1.0.4/quinten_cli.egg-info/entry_points.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       35 2023-03-05 20:54:16.000000 quinten-cli-1.0.4/quinten_cli.egg-info/requires.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)        4 2023-03-05 20:54:16.000000 quinten-cli-1.0.4/quinten_cli.egg-info/top_level.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      553 2023-03-05 20:54:16.281652 quinten-cli-1.0.4/setup.cfg
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       69 2023-03-05 20:15:30.000000 quinten-cli-1.0.4/setup.py
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-04-23 18:25:00.848521 quinten-cli-1.1.0/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1069 2023-04-23 18:15:22.000000 quinten-cli-1.1.0/LICENSE
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      672 2023-04-23 18:25:00.848521 quinten-cli-1.1.0/PKG-INFO
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      294 2023-04-23 18:15:22.000000 quinten-cli-1.1.0/README.md
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-04-23 18:25:00.848521 quinten-cli-1.1.0/cli/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      925 2023-04-23 18:15:22.000000 quinten-cli-1.1.0/cli/__init__.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      157 2023-04-23 18:15:22.000000 quinten-cli-1.1.0/cli/env.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      625 2023-04-23 18:15:22.000000 quinten-cli-1.1.0/cli/input_interface.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      741 2023-04-23 18:15:22.000000 quinten-cli-1.1.0/cli/install.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1241 2023-04-23 18:15:22.000000 quinten-cli-1.1.0/cli/output_interface.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1483 2023-04-23 18:15:22.000000 quinten-cli-1.1.0/cli/progress.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     5139 2023-04-23 18:19:12.000000 quinten-cli-1.1.0/cli/run.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      366 2023-04-23 18:15:22.000000 quinten-cli-1.1.0/cli/status.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      586 2023-04-23 18:23:25.000000 quinten-cli-1.1.0/pyproject.toml
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-04-23 18:25:00.848521 quinten-cli-1.1.0/quinten_cli.egg-info/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      672 2023-04-23 18:25:00.000000 quinten-cli-1.1.0/quinten_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      453 2023-04-23 18:25:00.000000 quinten-cli-1.1.0/quinten_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)        1 2023-04-23 18:25:00.000000 quinten-cli-1.1.0/quinten_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)       44 2023-04-23 18:25:00.000000 quinten-cli-1.1.0/quinten_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)       74 2023-04-23 18:25:00.000000 quinten-cli-1.1.0/quinten_cli.egg-info/requires.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)        4 2023-04-23 18:25:00.000000 quinten-cli-1.1.0/quinten_cli.egg-info/top_level.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      553 2023-04-23 18:25:00.848521 quinten-cli-1.1.0/setup.cfg
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)       69 2023-04-23 18:24:58.000000 quinten-cli-1.1.0/setup.py
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-04-23 18:25:00.848521 quinten-cli-1.1.0/tests/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      322 2023-04-23 18:15:22.000000 quinten-cli-1.1.0/tests/test_api.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      937 2023-04-23 18:15:22.000000 quinten-cli-1.1.0/tests/test_progress_ui.py
```

### Comparing `quinten-cli-1.0.4/LICENSE` & `quinten-cli-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quinten-cli-1.0.4/cli/__init__.py` & `quinten-cli-1.1.0/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `quinten-cli-1.0.4/cli/input_interface.py` & `quinten-cli-1.1.0/cli/input_interface.py`

 * *Files identical despite different names*

### Comparing `quinten-cli-1.0.4/cli/install.py` & `quinten-cli-1.1.0/cli/install.py`

 * *Files identical despite different names*

### Comparing `quinten-cli-1.0.4/cli/output_interface.py` & `quinten-cli-1.1.0/cli/output_interface.py`

 * *Files identical despite different names*

### Comparing `quinten-cli-1.0.4/cli/progress.py` & `quinten-cli-1.1.0/cli/progress.py`

 * *Files identical despite different names*

### Comparing `quinten-cli-1.0.4/cli/run.py` & `quinten-cli-1.1.0/cli/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 import shlex
 import subprocess
 import sys
 import types
 
+from plib import Path
+
 
 def sh(*cmds, **kwargs):
     return run_commands(*cmds, shell=True, **kwargs)
 
 
 def run_commands(*cmds, **kwargs):
     for cmd in cmds:
@@ -142,15 +144,17 @@
                 if auto_pw():
                     args.insert(1, "-A")
 
     return args
 
 
 def auto_pw() -> bool:
-    return "SUDO_ASKPASS" in os.environ
+    askpass_key = "SUDO_ASKPASS"
+    askpass_program = os.environ.get(askpass_key)
+    return askpass_program is not None and Path(askpass_program).exists()
 
 
 def iterate_args(args, command):
     """
     arg can be:
 
     - command string
```

### Comparing `quinten-cli-1.0.4/setup.cfg` & `quinten-cli-1.1.0/setup.cfg`

 * *Files identical despite different names*

