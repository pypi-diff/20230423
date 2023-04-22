# Comparing `tmp/fhs-iptv-tools-0.8.8.tar.gz` & `tmp/fhs-iptv-tools-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fhs-iptv-tools-0.8.8.tar", last modified: Thu Nov 10 22:22:26 2022, max compression
+gzip compressed data, was "fhs-iptv-tools-0.8.9.tar", last modified: Sat Nov 12 22:53:54 2022, max compression
```

## Comparing `fhs-iptv-tools-0.8.8.tar` & `fhs-iptv-tools-0.8.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 richard   (1000) richard   (1000)        0 2022-11-10 22:22:26.848406 fhs-iptv-tools-0.8.8/
--rw-r--r--   0 richard   (1000) richard   (1000)      149 2022-11-10 22:20:56.000000 fhs-iptv-tools-0.8.8/.bumpversion.cfg
-drwxr-xr-x   0 richard   (1000) richard   (1000)        0 2022-11-10 22:22:26.848406 fhs-iptv-tools-0.8.8/.githooks/
--rwxr-xr-x   0 richard   (1000) richard   (1000)     1611 2022-10-24 15:34:54.000000 fhs-iptv-tools-0.8.8/.githooks/prepare-commit-msg
--rw-r--r--   0 richard   (1000) richard   (1000)      391 2022-10-24 15:34:54.000000 fhs-iptv-tools-0.8.8/.gitignore
--rw-r--r--   0 richard   (1000) richard   (1000)      855 2022-11-10 22:21:18.000000 fhs-iptv-tools-0.8.8/CHANGELOG.md
--rw-r--r--   0 richard   (1000) richard   (1000)       25 2022-10-24 15:34:54.000000 fhs-iptv-tools-0.8.8/MANIFEST.in
--rw-r--r--   0 richard   (1000) richard   (1000)     3947 2022-11-10 22:22:26.848406 fhs-iptv-tools-0.8.8/PKG-INFO
--rw-r--r--   0 richard   (1000) richard   (1000)     3274 2022-11-10 22:20:56.000000 fhs-iptv-tools-0.8.8/README.md
--rw-r--r--   0 richard   (1000) richard   (1000)     2700 2022-11-01 22:15:59.000000 fhs-iptv-tools-0.8.8/justfile
--rw-r--r--   0 richard   (1000) richard   (1000)       16 2022-10-24 15:34:54.000000 fhs-iptv-tools-0.8.8/requirements-dev.txt
--rw-r--r--   0 richard   (1000) richard   (1000)      174 2022-10-24 15:34:54.000000 fhs-iptv-tools-0.8.8/requirements-flake8.txt
--rw-r--r--   0 richard   (1000) richard   (1000)       38 2022-11-07 22:09:02.000000 fhs-iptv-tools-0.8.8/requirements.txt
--rw-r--r--   0 richard   (1000) richard   (1000)       38 2022-11-10 22:22:26.848406 fhs-iptv-tools-0.8.8/setup.cfg
--rw-r--r--   0 richard   (1000) richard   (1000)     1726 2022-11-05 16:05:20.000000 fhs-iptv-tools-0.8.8/setup.py
-drwxr-xr-x   0 richard   (1000) richard   (1000)        0 2022-11-10 22:22:26.845072 fhs-iptv-tools-0.8.8/src/
-drwxr-xr-x   0 richard   (1000) richard   (1000)        0 2022-11-10 22:22:26.848406 fhs-iptv-tools-0.8.8/src/fhs_iptv_tools/
--rw-r--r--   0 richard   (1000) richard   (1000)      120 2022-10-24 16:06:03.000000 fhs-iptv-tools-0.8.8/src/fhs_iptv_tools/__init__.py
--rw-r--r--   0 richard   (1000) richard   (1000)      311 2022-11-10 22:20:56.000000 fhs-iptv-tools-0.8.8/src/fhs_iptv_tools/__version__.py
--rw-r--r--   0 richard   (1000) richard   (1000)     2555 2022-11-01 21:01:59.000000 fhs-iptv-tools-0.8.8/src/fhs_iptv_tools/cli.py
--rw-r--r--   0 richard   (1000) richard   (1000)       87 2022-10-29 22:42:49.000000 fhs-iptv-tools-0.8.8/src/fhs_iptv_tools/config.py
--rw-r--r--   0 richard   (1000) richard   (1000)      723 2022-11-01 16:03:30.000000 fhs-iptv-tools-0.8.8/src/fhs_iptv_tools/directories.py
--rw-r--r--   0 richard   (1000) richard   (1000)       19 2022-10-24 15:34:54.000000 fhs-iptv-tools-0.8.8/src/fhs_iptv_tools/fhs_iptv_tools.py
--rw-r--r--   0 richard   (1000) richard   (1000)     5702 2022-11-04 21:52:48.000000 fhs-iptv-tools-0.8.8/src/fhs_iptv_tools/import_m3u.py
--rw-r--r--   0 richard   (1000) richard   (1000)     4188 2022-11-09 22:35:58.000000 fhs-iptv-tools-0.8.8/src/fhs_iptv_tools/interactive_cmd2.py
--rw-r--r--   0 richard   (1000) richard   (1000)    20880 2022-11-09 21:31:13.000000 fhs-iptv-tools-0.8.8/src/fhs_iptv_tools/playyaml.py
--rw-r--r--   0 richard   (1000) richard   (1000)     6094 2022-11-08 22:27:44.000000 fhs-iptv-tools-0.8.8/src/fhs_iptv_tools/playyaml_lib.py
--rw-r--r--   0 richard   (1000) richard   (1000)     5842 2022-11-01 21:45:09.000000 fhs-iptv-tools-0.8.8/src/fhs_iptv_tools/probe.py
--rw-r--r--   0 richard   (1000) richard   (1000)    13890 2022-11-09 21:58:35.000000 fhs-iptv-tools-0.8.8/src/fhs_iptv_tools/probe_list.py
--rw-r--r--   0 richard   (1000) richard   (1000)      343 2022-05-28 20:02:12.000000 fhs-iptv-tools-0.8.8/src/fhs_iptv_tools/subgroup.py
--rw-r--r--   0 richard   (1000) richard   (1000)      447 2022-11-03 21:46:35.000000 fhs-iptv-tools-0.8.8/src/fhs_iptv_tools/utils.py
-drwxr-xr-x   0 richard   (1000) richard   (1000)        0 2022-11-10 22:22:26.848406 fhs-iptv-tools-0.8.8/src/fhs_iptv_tools.egg-info/
--rw-r--r--   0 richard   (1000) richard   (1000)     3947 2022-11-10 22:22:26.000000 fhs-iptv-tools-0.8.8/src/fhs_iptv_tools.egg-info/PKG-INFO
--rw-r--r--   0 richard   (1000) richard   (1000)      924 2022-11-10 22:22:26.000000 fhs-iptv-tools-0.8.8/src/fhs_iptv_tools.egg-info/SOURCES.txt
--rw-r--r--   0 richard   (1000) richard   (1000)        1 2022-11-10 22:22:26.000000 fhs-iptv-tools-0.8.8/src/fhs_iptv_tools.egg-info/dependency_links.txt
--rw-r--r--   0 richard   (1000) richard   (1000)       59 2022-11-10 22:22:26.000000 fhs-iptv-tools-0.8.8/src/fhs_iptv_tools.egg-info/entry_points.txt
--rw-r--r--   0 richard   (1000) richard   (1000)       38 2022-11-10 22:22:26.000000 fhs-iptv-tools-0.8.8/src/fhs_iptv_tools.egg-info/requires.txt
--rw-r--r--   0 richard   (1000) richard   (1000)       15 2022-11-10 22:22:26.000000 fhs-iptv-tools-0.8.8/src/fhs_iptv_tools.egg-info/top_level.txt
--rw-r--r--   0 richard   (1000) richard   (1000)      152 2022-10-24 15:34:54.000000 fhs-iptv-tools-0.8.8/template-version.txt
-drwxr-xr-x   0 richard   (1000) richard   (1000)        0 2022-11-10 22:22:26.848406 fhs-iptv-tools-0.8.8/tests/
--rw-r--r--   0 richard   (1000) richard   (1000)       98 2022-10-24 15:34:54.000000 fhs-iptv-tools-0.8.8/tests/test_sample.py
--rw-r--r--   0 richard   (1000) richard   (1000)      579 2022-11-01 22:29:06.000000 fhs-iptv-tools-0.8.8/tox.ini
+drwxr-xr-x   0 richard   (1000) richard   (1000)        0 2022-11-12 22:53:54.632660 fhs-iptv-tools-0.8.9/
+-rw-r--r--   0 richard   (1000) richard   (1000)      149 2022-11-12 21:11:05.000000 fhs-iptv-tools-0.8.9/.bumpversion.cfg
+drwxr-xr-x   0 richard   (1000) richard   (1000)        0 2022-11-12 22:53:54.629327 fhs-iptv-tools-0.8.9/.githooks/
+-rwxr-xr-x   0 richard   (1000) richard   (1000)     1611 2022-10-24 15:34:54.000000 fhs-iptv-tools-0.8.9/.githooks/prepare-commit-msg
+-rw-r--r--   0 richard   (1000) richard   (1000)      391 2022-10-24 15:34:54.000000 fhs-iptv-tools-0.8.9/.gitignore
+-rw-r--r--   0 richard   (1000) richard   (1000)      991 2022-11-12 22:51:30.000000 fhs-iptv-tools-0.8.9/CHANGELOG.md
+-rw-r--r--   0 richard   (1000) richard   (1000)       25 2022-10-24 15:34:54.000000 fhs-iptv-tools-0.8.9/MANIFEST.in
+-rw-r--r--   0 richard   (1000) richard   (1000)     3947 2022-11-12 22:53:54.632660 fhs-iptv-tools-0.8.9/PKG-INFO
+-rw-r--r--   0 richard   (1000) richard   (1000)     3274 2022-11-12 21:11:05.000000 fhs-iptv-tools-0.8.9/README.md
+-rw-r--r--   0 richard   (1000) richard   (1000)     2806 2022-11-12 20:46:34.000000 fhs-iptv-tools-0.8.9/justfile
+-rw-r--r--   0 richard   (1000) richard   (1000)       16 2022-10-24 15:34:54.000000 fhs-iptv-tools-0.8.9/requirements-dev.txt
+-rw-r--r--   0 richard   (1000) richard   (1000)      174 2022-10-24 15:34:54.000000 fhs-iptv-tools-0.8.9/requirements-flake8.txt
+-rw-r--r--   0 richard   (1000) richard   (1000)       38 2022-11-07 22:09:02.000000 fhs-iptv-tools-0.8.9/requirements.txt
+-rw-r--r--   0 richard   (1000) richard   (1000)       38 2022-11-12 22:53:54.632660 fhs-iptv-tools-0.8.9/setup.cfg
+-rw-r--r--   0 richard   (1000) richard   (1000)     1726 2022-11-05 16:05:20.000000 fhs-iptv-tools-0.8.9/setup.py
+drwxr-xr-x   0 richard   (1000) richard   (1000)        0 2022-11-12 22:53:54.629327 fhs-iptv-tools-0.8.9/src/
+drwxr-xr-x   0 richard   (1000) richard   (1000)        0 2022-11-12 22:53:54.629327 fhs-iptv-tools-0.8.9/src/fhs_iptv_tools/
+-rw-r--r--   0 richard   (1000) richard   (1000)      120 2022-10-24 16:06:03.000000 fhs-iptv-tools-0.8.9/src/fhs_iptv_tools/__init__.py
+-rw-r--r--   0 richard   (1000) richard   (1000)      311 2022-11-12 21:11:05.000000 fhs-iptv-tools-0.8.9/src/fhs_iptv_tools/__version__.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     2555 2022-11-01 21:01:59.000000 fhs-iptv-tools-0.8.9/src/fhs_iptv_tools/cli.py
+-rw-r--r--   0 richard   (1000) richard   (1000)       87 2022-10-29 22:42:49.000000 fhs-iptv-tools-0.8.9/src/fhs_iptv_tools/config.py
+-rw-r--r--   0 richard   (1000) richard   (1000)      723 2022-11-01 16:03:30.000000 fhs-iptv-tools-0.8.9/src/fhs_iptv_tools/directories.py
+-rw-r--r--   0 richard   (1000) richard   (1000)       19 2022-10-24 15:34:54.000000 fhs-iptv-tools-0.8.9/src/fhs_iptv_tools/fhs_iptv_tools.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     5702 2022-11-04 21:52:48.000000 fhs-iptv-tools-0.8.9/src/fhs_iptv_tools/import_m3u.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     4188 2022-11-09 22:35:58.000000 fhs-iptv-tools-0.8.9/src/fhs_iptv_tools/interactive_cmd2.py
+-rw-r--r--   0 richard   (1000) richard   (1000)    22308 2022-11-12 22:49:24.000000 fhs-iptv-tools-0.8.9/src/fhs_iptv_tools/playyaml.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     6094 2022-11-08 22:27:44.000000 fhs-iptv-tools-0.8.9/src/fhs_iptv_tools/playyaml_lib.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     6175 2022-11-11 21:27:33.000000 fhs-iptv-tools-0.8.9/src/fhs_iptv_tools/probe.py
+-rw-r--r--   0 richard   (1000) richard   (1000)    14863 2022-11-12 21:07:03.000000 fhs-iptv-tools-0.8.9/src/fhs_iptv_tools/probe_list.py
+-rw-r--r--   0 richard   (1000) richard   (1000)      343 2022-05-28 20:02:12.000000 fhs-iptv-tools-0.8.9/src/fhs_iptv_tools/subgroup.py
+-rw-r--r--   0 richard   (1000) richard   (1000)      447 2022-11-03 21:46:35.000000 fhs-iptv-tools-0.8.9/src/fhs_iptv_tools/utils.py
+drwxr-xr-x   0 richard   (1000) richard   (1000)        0 2022-11-12 22:53:54.632660 fhs-iptv-tools-0.8.9/src/fhs_iptv_tools.egg-info/
+-rw-r--r--   0 richard   (1000) richard   (1000)     3947 2022-11-12 22:53:54.000000 fhs-iptv-tools-0.8.9/src/fhs_iptv_tools.egg-info/PKG-INFO
+-rw-r--r--   0 richard   (1000) richard   (1000)      924 2022-11-12 22:53:54.000000 fhs-iptv-tools-0.8.9/src/fhs_iptv_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 richard   (1000) richard   (1000)        1 2022-11-12 22:53:54.000000 fhs-iptv-tools-0.8.9/src/fhs_iptv_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 richard   (1000) richard   (1000)       59 2022-11-12 22:53:54.000000 fhs-iptv-tools-0.8.9/src/fhs_iptv_tools.egg-info/entry_points.txt
+-rw-r--r--   0 richard   (1000) richard   (1000)       38 2022-11-12 22:53:54.000000 fhs-iptv-tools-0.8.9/src/fhs_iptv_tools.egg-info/requires.txt
+-rw-r--r--   0 richard   (1000) richard   (1000)       15 2022-11-12 22:53:54.000000 fhs-iptv-tools-0.8.9/src/fhs_iptv_tools.egg-info/top_level.txt
+-rw-r--r--   0 richard   (1000) richard   (1000)      152 2022-10-24 15:34:54.000000 fhs-iptv-tools-0.8.9/template-version.txt
+drwxr-xr-x   0 richard   (1000) richard   (1000)        0 2022-11-12 22:53:54.632660 fhs-iptv-tools-0.8.9/tests/
+-rw-r--r--   0 richard   (1000) richard   (1000)       98 2022-10-24 15:34:54.000000 fhs-iptv-tools-0.8.9/tests/test_sample.py
+-rw-r--r--   0 richard   (1000) richard   (1000)      579 2022-11-01 22:29:06.000000 fhs-iptv-tools-0.8.9/tox.ini
```

### Comparing `fhs-iptv-tools-0.8.8/.githooks/prepare-commit-msg` & `fhs-iptv-tools-0.8.9/.githooks/prepare-commit-msg`

 * *Files identical despite different names*

### Comparing `fhs-iptv-tools-0.8.8/CHANGELOG.md` & `fhs-iptv-tools-0.8.9/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -16,7 +16,8 @@
 - 0.8.2: add save_m3u (so now this program is usable)
 - 0.8.3: add modify_channel, change channel id, name, group_title, and logo and small bug in display channel
 - 0.8.4: add copy_channels to copy channels and list_stores to list current stores.
 - 0.8.5: fix missing dependancy (pyyaml), add clear tag and change add copy of dataclass struct on copy_channel function
 - 0.8.6: add move, select_and_copy, select_and_move options
 - 0.8.7: add sorted options and add cleanup of save_tasks command.
 - 0.8.8: change documentation
+- 0.8.9: some small changes and add a run_tasks command, to load and use a task file from interactive mode, changed some default values
```

### Comparing `fhs-iptv-tools-0.8.8/PKG-INFO` & `fhs-iptv-tools-0.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fhs-iptv-tools
-Version: 0.8.8
+Version: 0.8.9
 Summary: foxhunt software iptv tools, making iptv easier
 Home-page: https://github.com/foxhunt72/fhs-iptv-tools
 Author: Richard de Vos
 Author-email: rdevos72@gmail.com
 License: MIT license
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 
 fhs\_iptv\_tools
 ================
 
-Iptv Tools Version: 0.8.8
+Iptv Tools Version: 0.8.9
 --------
 #### ** For changes see** [changelog](https://github.com/foxhunt72/fhs-iptv-tools/blob/main/CHANGELOG.md).
 
 ## Foxhunt Software IPTV Tools
 
 Making iptv easier
```

### Comparing `fhs-iptv-tools-0.8.8/README.md` & `fhs-iptv-tools-0.8.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 fhs\_iptv\_tools
 ================
 
-Iptv Tools Version: 0.8.8
+Iptv Tools Version: 0.8.9
 --------
 #### ** For changes see** [changelog](https://github.com/foxhunt72/fhs-iptv-tools/blob/main/CHANGELOG.md).
 
 ## Foxhunt Software IPTV Tools
 
 Making iptv easier
```

### Comparing `fhs-iptv-tools-0.8.8/justfile` & `fhs-iptv-tools-0.8.9/justfile`

 * *Files 4% similar despite different names*

```diff
@@ -98,13 +98,15 @@
 pytest-failure:
   tox -e py310 -- --lf --trace
 
 # bump version number
 bumppatch:
   #!/usr/bin/env sh
   bumpversion --allow-dirty --verbose patch
+  # bumpversion --allow-dirty --verbose --new-version 1.0.0
+  # bumpversion --allow-dirty --verbose major
 
 # edit README.rst
 readme:
   #!/usr/bin/env sh
   formiko README.rst
```

### Comparing `fhs-iptv-tools-0.8.8/setup.py` & `fhs-iptv-tools-0.8.9/setup.py`

 * *Files identical despite different names*

### Comparing `fhs-iptv-tools-0.8.8/src/fhs_iptv_tools/cli.py` & `fhs-iptv-tools-0.8.9/src/fhs_iptv_tools/cli.py`

 * *Files identical despite different names*

### Comparing `fhs-iptv-tools-0.8.8/src/fhs_iptv_tools/directories.py` & `fhs-iptv-tools-0.8.9/src/fhs_iptv_tools/directories.py`

 * *Files identical despite different names*

### Comparing `fhs-iptv-tools-0.8.8/src/fhs_iptv_tools/import_m3u.py` & `fhs-iptv-tools-0.8.9/src/fhs_iptv_tools/import_m3u.py`

 * *Files identical despite different names*

### Comparing `fhs-iptv-tools-0.8.8/src/fhs_iptv_tools/interactive_cmd2.py` & `fhs-iptv-tools-0.8.9/src/fhs_iptv_tools/interactive_cmd2.py`

 * *Files identical despite different names*

### Comparing `fhs-iptv-tools-0.8.8/src/fhs_iptv_tools/playyaml.py` & `fhs-iptv-tools-0.8.9/src/fhs_iptv_tools/playyaml.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,35 @@
 
 
 import sys
 from . import config
 from .playyaml_lib import func_dict_parse, play as play_lib
 
 
+def play_command_run_tasks(task):
+    """Play command load_m3u_file.
+
+    Args:
+        task: task array
+
+    Returns:
+        Good: boolean
+    """
+    from .probe_list import ProbeInfoList
+
+    task_file = task["file"]
+    include_tag = task['include_tag']
+    if include_tag == "":
+        include_tag = None
+    exclude_tag = task['exclude_tag']
+    if exclude_tag == "":
+        exclude_tag = None
+    play(task_file, include_tag, exclude_tag)
+    return True
+
 def play_command_load_m3u_file(task):
     """Play command load_m3u_file.
 
     Args:
         task: task array
 
     Returns:
@@ -146,15 +167,15 @@
         Good: boolean
     """
     from .probe_list import ProbeInfoList
 
     task_store = task['store']
     if task_store not in config.STORE:
         config.STORE[task_store] = ProbeInfoList()
-    count = config.STORE[task_store].list_channels(with_tag=task['with_tag'], without_tag=task['without_tag'])
+    count = config.STORE[task_store].list_channels(with_tag=task['with_tag'], without_tag=task['without_tag'], verbose=task['verbose'])
     print(f"list {count} channels.")
     return True
 
 
 def play_command_sort_channels(task):
     """Play command sort channels.
 
@@ -170,15 +191,15 @@
     if task_store not in config.STORE:
         config.STORE[task_store] = ProbeInfoList()
     result = config.STORE[task_store].sort_channels(
         sort_key1=task['sort_key1'],
         sort_key2=task['sort_key2']
     )
     if result:
-        print("sorted channels.")
+        print(f"sorted channels with key1: {task['sort_key1']}, key2: {task['sort_key2']}.")
     else:
         print("ERROR: sorted channels failed.")
     return True
 
 
 def play_command_modify_channels(task):
     """Play command modify channels.
@@ -409,15 +430,21 @@
     from .probe_list import ProbeInfoList
 
     task_store = task['store']
     delay = int(task['delay'])
     if task_store not in config.STORE:
         config.STORE[task_store] = ProbeInfoList()
     with config.CONSOLE.status(f"Probe scan channel list from store: {task_store} with delay {delay}", spinner="dots"):
-        config.STORE[task_store].probe_scan(delay)
+        config.STORE[task_store].probe_scan(
+            with_tag=task['with_tag'],
+            without_tag=task['without_tag'],
+            with_id=task['with_id'],
+            with_name=task['with_name'],
+            delay=delay
+        )
     return True
 
 
 def play_command_list_groups(task):
     """Play command list groups.
 
     Args:
@@ -500,14 +527,23 @@
             config.STORE[task_store].filter_lijst(LoadType.VOD)
         return True
     sys.stderr.write(f"ERROR: unknown filter options '{task_type}' and not channels or vod")
     return True
 
 
 funcdict = {
+    "run_tasks": {
+        "args": [
+            {"name": "file"},
+            {"name": "include_tag", "default": ""},
+            {"name": "exclude_tag", "default": ""}
+        ],
+        "func": play_command_run_tasks,
+        "help": "run tasks from yaml task file."
+    },
     "load_m3u": {
         "args": [{"name": "file"}, {"name": "store", "help": "store name", "default": "default"}],
         "func": play_command_load_m3u_file,
         "help": "loading m3u file from disk."
     },
     "count_channels": {
         "args": [{"name": "store", "help": "store name", "default": "default"}],
@@ -531,15 +567,22 @@
     },
     "group_channels": {
         "args": [{"name": "store", "help": "store name", "default": "default"},{"name": "group"}],
         "func": play_command_group_channels,
         "help": "list channels for a group."
     },
     "probe_scan": {
-        "args": [{"name": "store", "help": "store name", "default": "default"},{"name": "delay", "help": "delay between probing channels", "default": "5"}],
+        "args": [
+            {"name": "store", "help": "store name", "default": "default"},
+            {"name": "delay", "help": "delay between probing channels", "default": "5"},
+            {"name": "with_tag", "default": ""},
+            {"name": "without_tag", "default": ""},
+            {"name": "with_id", "default": ""},
+            {"name": "with_name", "default": ""}
+        ],
         "func": play_command_probe_scan,
         "help": "probe scanning the list of channels."
     },
     "filter_channels": {
         "args": [{"name": 'type', "help": "type to filter, channels or vod"}, {"name": "store", "help": "store name", "default": "default"}],
         "func": play_command_filter_channels,
         "help": "filter channels."
@@ -596,47 +639,48 @@
     "copy_channels": {
         "args": [
             {"name": "store", "help": "store name", "default": "default"},
             {"name": "with_tag", "default": ""},
             {"name": "without_tag", "default": ""},
             {"name": "with_id", "default": ""},
             {"name": "with_name", "default": ""},
-            {"name": "to_store", "default": ""},
+            {"name": "to_store"},
         ],
         "func": play_command_copy_channels,
         "loop": "channels",
         "help": "copy channels to other store (create store if not exists)."
     },
     "move_channels": {
         "args": [
             {"name": "store", "help": "store name", "default": "default"},
             {"name": "with_tag", "default": ""},
             {"name": "without_tag", "default": ""},
             {"name": "with_id", "default": ""},
             {"name": "with_name", "default": ""},
-            {"name": "to_store", "default": ""},
+            {"name": "to_store"},
         ],
         "func": play_command_move_channels,
         "loop": "channels",
         "help": "move channels to other store (create store if not exists)."
     },
     "list_channels": {
         "args": [
             {"name": "store", "help": "store name", "default": "default"},
             {"name": "with_tag", "default": ""},
             {"name": "without_tag", "default": ""},
+            {"name": "verbose", "default": "no", "help": "verbose: no or yes"},
         ],
         "func": play_command_list_channels,
         "help": "list channels."
     },
     "sort_channels": {
         "args": [
             {"name": "store", "help": "store name", "default": "default"},
-            {"name": "sort_key1", "default": ""},
-            {"name": "sort_key2", "default": ""},
+            {"name": "sort_key1", "default": "tvg_group_title", 'help': "sort key 1: tvg_id, tvg_name, tvg_logo, tvg_group_title"},
+            {"name": "sort_key2", "default": "tvg_name", 'help': "sort key 2: tvg_id, tvg_name, tvg_logo, tvg_group_title"},
         ],
         "func": play_command_sort_channels,
         "help": "sort channels."
     },
     "save_m3u": {
         "args": [
             {"name": "store", "help": "store name", "default": "default"},
@@ -667,29 +711,29 @@
             {"name": "store", "help": "store name", "default": "default"},
             {"name": "with_tag", "default": ""},
             {"name": "without_tag", "default": ""},
             {"name": "group_title", "default": ""},
             {"name": "name", "default": ""},
             {"name": "id", "default": ""},
             {"name": "source", "default": ""},
-            {"name": "to_store", "default": ""},
+            {"name": "to_store"},
         ],
         "func": play_command_select_copy,
         "help": "select and copy channels."
     },
     "select_and_move": {
         "args": [
             {"name": "store", "help": "store name", "default": "default"},
             {"name": "with_tag", "default": ""},
             {"name": "without_tag", "default": ""},
             {"name": "group_title", "default": ""},
             {"name": "name", "default": ""},
             {"name": "id", "default": ""},
             {"name": "source", "default": ""},
-            {"name": "to_store", "default": ""},
+            {"name": "to_store"},
         ],
         "func": play_command_select_move,
         "help": "select and move channels."
     }
 }
```

### Comparing `fhs-iptv-tools-0.8.8/src/fhs_iptv_tools/playyaml_lib.py` & `fhs-iptv-tools-0.8.9/src/fhs_iptv_tools/playyaml_lib.py`

 * *Files identical despite different names*

### Comparing `fhs-iptv-tools-0.8.8/src/fhs_iptv_tools/probe.py` & `fhs-iptv-tools-0.8.9/src/fhs_iptv_tools/probe.py`

 * *Files 6% similar despite different names*

```diff
@@ -158,16 +158,16 @@
             if packet['stream_index'] != stream:
                 continue
             total_size += int(packet['size'])
             total_time += float(packet.get('duration_time', 0))
         try:
             bitrate = int(((total_size * 8) / total_time))
         except ZeroDivisionError:
-            return "unknown"
-        return f"{bitrate} calculated"
+            return -1
+        return bitrate
 
     def swap_video_and_audio_in_list(self, result):
         """Reverse list is list consist of audio / video and not video / auto.
 
         Args:
             result: list of results
 
@@ -176,29 +176,36 @@
         """
         if len(result) != 2:
             return result  # more or less than 2 entries
         if 'audio' in result[0] and 'video' in result[1]:
             result.reverse()
         return result
 
-    def info2str(self, media_info):
+    def info2str_and_dict(self, media_info):
         """Convert media info to info str.
 
         Args:
             media_info: ffprobe info
 
         Returns:
             media_str
         """
         result = []
+        dict_result = {}
         for idx, p in enumerate(media_info['streams']):
             codec_type = p.get('codec_type', 'unknown')
             if 'bit_rate' in p:
                 bit_rate = p['bit_rate']
             else:
                 bit_rate = self.calculate_bitrate(media_info, idx)
+            dict_result[codec_type]={
+                'codec': p.get('codec_name','codec unknown'),
+                'bit_rate': int(bit_rate)
+            }
             if codec_type == 'video':
                 result.append(f"video: {p.get('codec_name','codec unknown')} bit_rate: {bit_rate} / width: {p.get('width', 'unknown')} / height: {p.get('height', 'unknown')}")  # noqa: E501
+                dict_result[codec_type]['with'] = int(p.get('width', -1))
+                dict_result[codec_type]['height'] = int(p.get('height', -1))
             if codec_type == 'audio':
                 result.append(f"audio: {p.get('codec_name','codec unknown')} bit_rate: {bit_rate}")  # noqa: E501
         result = self.swap_video_and_audio_in_list(result)
-        return ", ".join(result)
+        return (", ".join(result), dict_result)
```

### Comparing `fhs-iptv-tools-0.8.8/src/fhs_iptv_tools/probe_list.py` & `fhs-iptv-tools-0.8.9/src/fhs_iptv_tools/probe_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # probe source
 
 from .probe import ProbeInfo
 from .import_m3u import import_m3u_file, return_tvg_group_titles, M3uChannel
 from enum import Enum
 import time
 import copy
+from pprint import pprint
 
 
 class LoadType(Enum):
     """LoadTypes from loading m3u channels."""
 
     ALL = 0
     CHANNELS = 1
@@ -66,49 +67,69 @@
             self.write_error(f"unknown type: {filter_type=}")
             return None
 
         result = list(filter(lambda d: d.vod is include_vod, self.__m3u_channels))
         self.__m3u_channels = result
         return self.__m3u_channels
 
-    def probe_scan(self, delay=5, status_output=None):
+    def probe_channel(self, *, channel, status_output, max_len=40, delay=5):
+        """Probe a channel.
+
+        Args:
+            channel: channel array
+            status_output: function to output status
+            max_len: max len for tvg_name
+            delay: sleep delay after scan
+        """
+        if status_output is not None:
+            status_output(f"starting scanning: {channel.tvg_name}")
+        if type(channel.tvg_sources) == list:
+            for source in channel.tvg_sources:
+                result = self.__probe.probe_with_cache(source)
+        else:
+            result = self.__probe.probe_with_cache(channel.tvg_sources)
+        if result is None:
+            if status_output is not None:
+                status_output(f"no result for: {channel.tvg_name}")
+            return
+
+        if status_output is not None:
+            status_output(f"ready scanning: {channel.tvg_name}")
+        (channel.fhs_info, channel.fhs_dict) = self.__probe.info2str_and_dict(result)
+        print(f"{channel.tvg_name:{max_len}}:\t{channel.fhs_info}")
+        if result.get('fhs_source', 'unknown') != 'cache':
+            time.sleep(delay)
+        return
+
+
+
+    def probe_scan(self, *, delay=5, status_output=None, with_tag="", without_tag="", with_id="", with_name=""):
         """Probe a m3u file.
 
-        Args: 
+        Args:
             delay: delay between channels.
             status_output: function to output status
+            with_tag: select on tag set
+            without_tag: select on tag not set
+            with_id: change only on id
+            with_name: change only when name is the same
 
         Returns:
             Status: None
         """
         max_len = 10
-        for ch in self.__m3u_channels:
+        channels = list(self.get_channels(
+            with_tag=with_tag, without_tag=without_tag, with_id=with_id, with_name=with_name))
+        print(f"channels: {len(channels)}")
+        for ch in channels:
             if len(ch.tvg_name) > max_len:
                 max_len = len(ch.tvg_name)
         max_len += 3
-        for ch in self.__m3u_channels:
-            if status_output is not None:
-                status_output(f"starting scanning: {ch.tvg_name}")
-            if type(ch.tvg_sources) == list:
-                for source in ch.tvg_sources:
-                    result = self.__probe.probe_with_cache(source)
-            else:
-                result = self.__probe.probe_with_cache(ch.tvg_sources)
-            if result is None:
-                if status_output is not None:
-                    status_output(f"no result for: {ch.tvg_name}")
-                continue
-
-            if status_output is not None:
-                status_output(f"ready scanning: {ch.tvg_name}")
-            ch.fhs_info = self.__probe.info2str(result)
-            print(f"{ch.tvg_name:{max_len}}:\t{ch.fhs_info}")
-            if result.get('fhs_source', 'unknown') != 'cache':
-                time.sleep(delay)
-
+        for ch in channels:
+            self.probe_channel(channel=ch, status_output=status_output, max_len=max_len, delay=delay)
         return None
 
     def count_channels(self):
         """Count the channels.
 
         Returns:
             count of channels
@@ -322,31 +343,34 @@
         tags = ", ".join(channel.fhs_tags)
         if tags != "":
             display_tags = f" tags: {tags}"
         else:
             display_tags = ""
         return f"<{channel.tvg_id}> {channel.tvg_name}   /   {channel.tvg_group_title}{display_tags}"
 
-    def list_channels(self, *, with_tag="", without_tag=""):
+    def list_channels(self, *, with_tag="", without_tag="", verbose="no"):
         """List channels.
 
         List channels
 
         Args:
             with_tag: select on tag set
             without_tag: select on tag not set
+            verbose: verbose output no or yes
 
         Returns:
             yield of channels
         """
 
         count = 0
         for ch in self.get_channels(with_tag=with_tag, without_tag=without_tag):
             count += 1
             print(f"{count}: {self.display_channel(ch)}")
+            if verbose == 'yes':
+                pprint(ch)
         return count
 
     def save_m3u_file(self, *, file, with_tag="", without_tag=""):
         """List channels.
 
         List channels
```

### Comparing `fhs-iptv-tools-0.8.8/src/fhs_iptv_tools.egg-info/PKG-INFO` & `fhs-iptv-tools-0.8.9/src/fhs_iptv_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fhs-iptv-tools
-Version: 0.8.8
+Version: 0.8.9
 Summary: foxhunt software iptv tools, making iptv easier
 Home-page: https://github.com/foxhunt72/fhs-iptv-tools
 Author: Richard de Vos
 Author-email: rdevos72@gmail.com
 License: MIT license
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 
 fhs\_iptv\_tools
 ================
 
-Iptv Tools Version: 0.8.8
+Iptv Tools Version: 0.8.9
 --------
 #### ** For changes see** [changelog](https://github.com/foxhunt72/fhs-iptv-tools/blob/main/CHANGELOG.md).
 
 ## Foxhunt Software IPTV Tools
 
 Making iptv easier
```

### Comparing `fhs-iptv-tools-0.8.8/src/fhs_iptv_tools.egg-info/SOURCES.txt` & `fhs-iptv-tools-0.8.9/src/fhs_iptv_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fhs-iptv-tools-0.8.8/tox.ini` & `fhs-iptv-tools-0.8.9/tox.ini`

 * *Files identical despite different names*

