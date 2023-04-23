# Comparing `tmp/gpush-3.0.1.tar.gz` & `tmp/gpush-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpush-3.0.1.tar", last modified: Wed Apr 19 07:50:27 2023, max compression
+gzip compressed data, was "gpush-3.1.0.tar", last modified: Sun Apr 23 12:16:39 2023, max compression
```

## Comparing `gpush-3.0.1.tar` & `gpush-3.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:50:27.566666 gpush-3.0.1/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-04-19 07:50:24.000000 gpush-3.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1718 2023-04-19 07:50:27.566666 gpush-3.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1606 2023-04-19 07:50:24.000000 gpush-3.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-19 07:50:25.000000 gpush-3.0.1/_version.py
--rw-r--r--   0 root         (0) root         (0)     3875 2023-04-19 07:50:27.000000 gpush-3.0.1/gpush
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:50:27.566666 gpush-3.0.1/gpush.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1718 2023-04-19 07:50:27.000000 gpush-3.0.1/gpush.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      212 2023-04-19 07:50:27.000000 gpush-3.0.1/gpush.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 07:50:27.000000 gpush-3.0.1/gpush.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-04-19 07:50:27.000000 gpush-3.0.1/gpush.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-19 07:50:27.000000 gpush-3.0.1/gpush.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) root         (0)     3875 2023-04-19 07:50:24.000000 gpush-3.0.1/gpush.py
--rw-r--r--   0 root         (0) root         (0)      227 2023-04-19 07:50:24.000000 gpush-3.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 07:50:27.566666 gpush-3.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      774 2023-04-19 07:50:24.000000 gpush-3.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 12:16:39.270067 gpush-3.1.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-04-23 12:16:35.000000 gpush-3.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1718 2023-04-23 12:16:39.266066 gpush-3.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1606 2023-04-23 12:16:35.000000 gpush-3.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-23 12:16:36.000000 gpush-3.1.0/_version.py
+-rw-r--r--   0 root         (0) root         (0)     4282 2023-04-23 12:16:39.000000 gpush-3.1.0/gpush
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 12:16:39.266066 gpush-3.1.0/gpush.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1718 2023-04-23 12:16:39.000000 gpush-3.1.0/gpush.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      212 2023-04-23 12:16:39.000000 gpush-3.1.0/gpush.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 12:16:39.000000 gpush-3.1.0/gpush.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-04-23 12:16:39.000000 gpush-3.1.0/gpush.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-23 12:16:39.000000 gpush-3.1.0/gpush.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)     4282 2023-04-23 12:16:35.000000 gpush-3.1.0/gpush.py
+-rw-r--r--   0 root         (0) root         (0)      227 2023-04-23 12:16:35.000000 gpush-3.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 12:16:39.270067 gpush-3.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      774 2023-04-23 12:16:35.000000 gpush-3.1.0/setup.py
```

### Comparing `gpush-3.0.1/LICENSE` & `gpush-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gpush-3.0.1/PKG-INFO` & `gpush-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpush
-Version: 3.0.1
+Version: 3.1.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gpush
 
 `gpush` is a command line utility for standardising commit messages using [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/).
```

### Comparing `gpush-3.0.1/README.md` & `gpush-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `gpush-3.0.1/gpush` & `gpush-3.1.0/gpush`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,21 @@
     help="[Default: False] Option to enable git push",
 )
 parser.add_argument(
     "--message",
     action="store",
     help="[Default: None] Override message prompt and use the provided message",
 )
+parser.add_argument(
+    "--branch",
+    action="store",
+    default="current",
+    help="[Default: current] Override using the current branch and use the provided branch",
+)
+
 
 args = parser.parse_args()
 
 
 def get_version():
     """
     Function to return the current version of gpush.py
@@ -76,16 +83,22 @@
 def git_push():
     """
     Function to push commit up to Git on the current branch for the repository
 
     :return: True/False
     """
     try:
+        if str(args.branch) != "current":
+            branch_name = str(args.branch)
+        else:
+            repo = Repo(search_parent_directories=True)
+            branch_name = repo.active_branch
         repo = Repo(search_parent_directories=True)
-        repo.git.push("--set-upstream", "origin", repo.active_branch)
+        repo.create_head(branch_name)
+        repo.git.push("--set-upstream", "origin", branch_name)
         print("Pushed successfully")
     except Exception as error_message:
         print("Some error occurred while pushing the code:")
         print(str(error_message))
         raise
 
     return True
```

### Comparing `gpush-3.0.1/gpush.egg-info/PKG-INFO` & `gpush-3.1.0/gpush.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpush
-Version: 3.0.1
+Version: 3.1.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gpush
 
 `gpush` is a command line utility for standardising commit messages using [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/).
```

### Comparing `gpush-3.0.1/gpush.py` & `gpush-3.1.0/gpush.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,21 @@
     help="[Default: False] Option to enable git push",
 )
 parser.add_argument(
     "--message",
     action="store",
     help="[Default: None] Override message prompt and use the provided message",
 )
+parser.add_argument(
+    "--branch",
+    action="store",
+    default="current",
+    help="[Default: current] Override using the current branch and use the provided branch",
+)
+
 
 args = parser.parse_args()
 
 
 def get_version():
     """
     Function to return the current version of gpush.py
@@ -76,16 +83,22 @@
 def git_push():
     """
     Function to push commit up to Git on the current branch for the repository
 
     :return: True/False
     """
     try:
+        if str(args.branch) != "current":
+            branch_name = str(args.branch)
+        else:
+            repo = Repo(search_parent_directories=True)
+            branch_name = repo.active_branch
         repo = Repo(search_parent_directories=True)
-        repo.git.push("--set-upstream", "origin", repo.active_branch)
+        repo.create_head(branch_name)
+        repo.git.push("--set-upstream", "origin", branch_name)
         print("Pushed successfully")
     except Exception as error_message:
         print("Some error occurred while pushing the code:")
         print(str(error_message))
         raise
 
     return True
```

### Comparing `gpush-3.0.1/setup.py` & `gpush-3.1.0/setup.py`

 * *Files identical despite different names*

