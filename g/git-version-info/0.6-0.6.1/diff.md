# Comparing `tmp/git_version_info-0.6.tar.gz` & `tmp/git_version_info-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_version_info-0.6.tar", last modified: Sun Apr 23 19:00:01 2023, max compression
+gzip compressed data, was "git_version_info-0.6.1.tar", last modified: Sun Apr 23 19:03:58 2023, max compression
```

## Comparing `git_version_info-0.6.tar` & `git_version_info-0.6.1.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 19:00:01.895173 git_version_info-0.6/
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-04-23 18:59:50.000000 git_version_info-0.6/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-04-23 18:59:50.000000 git_version_info-0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      961 2023-04-23 19:00:01.895173 git_version_info-0.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      390 2023-04-23 18:59:50.000000 git_version_info-0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 19:00:01.893173 git_version_info-0.6/git_version_info.egg-info/
--rw-r--r--   0 root         (0) root         (0)      961 2023-04-23 19:00:01.000000 git_version_info-0.6/git_version_info.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      352 2023-04-23 19:00:01.000000 git_version_info-0.6/git_version_info.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 19:00:01.000000 git_version_info-0.6/git_version_info.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-04-23 19:00:01.000000 git_version_info-0.6/git_version_info.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-23 19:00:01.000000 git_version_info-0.6/git_version_info.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      712 2023-04-23 19:00:01.896173 git_version_info-0.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      545 2023-04-23 18:59:50.000000 git_version_info-0.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 19:00:01.893173 git_version_info-0.6/test/
--rw-rw-rw-   0 root         (0) root         (0)      242 2023-04-23 18:59:50.000000 git_version_info-0.6/test/test_basics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 19:00:01.896173 git_version_info-0.6/version_info/
--rw-rw-rw-   0 root         (0) root         (0)      207 2023-04-23 18:59:50.000000 git_version_info-0.6/version_info/__init__.py
--rw-r--r--   0 root         (0) root         (0)      496 2023-04-23 19:00:01.896173 git_version_info-0.6/version_info/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     3106 2023-04-23 18:59:50.000000 git_version_info-0.6/version_info/main.py
--rw-rw-rw-   0 root         (0) root         (0)    68749 2023-04-23 18:59:50.000000 git_version_info-0.6/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 19:03:58.466489 git_version_info-0.6.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-04-23 19:03:46.000000 git_version_info-0.6.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-23 19:03:46.000000 git_version_info-0.6.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      963 2023-04-23 19:03:58.466489 git_version_info-0.6.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      390 2023-04-23 19:03:46.000000 git_version_info-0.6.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 19:03:58.464489 git_version_info-0.6.1/git_version_info.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      963 2023-04-23 19:03:58.000000 git_version_info-0.6.1/git_version_info.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      387 2023-04-23 19:03:58.000000 git_version_info-0.6.1/git_version_info.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 19:03:58.000000 git_version_info-0.6.1/git_version_info.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-04-23 19:03:58.000000 git_version_info-0.6.1/git_version_info.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-23 19:03:58.000000 git_version_info-0.6.1/git_version_info.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-04-23 19:03:46.000000 git_version_info-0.6.1/requirements.in
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-04-23 19:03:46.000000 git_version_info-0.6.1/requirementsDev.in
+-rw-rw-rw-   0 root         (0) root         (0)      712 2023-04-23 19:03:58.467489 git_version_info-0.6.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      545 2023-04-23 19:03:46.000000 git_version_info-0.6.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 19:03:58.465489 git_version_info-0.6.1/test/
+-rw-rw-rw-   0 root         (0) root         (0)      242 2023-04-23 19:03:46.000000 git_version_info-0.6.1/test/test_basics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 19:03:58.468489 git_version_info-0.6.1/version_info/
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-04-23 19:03:46.000000 git_version_info-0.6.1/version_info/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      498 2023-04-23 19:03:58.468489 git_version_info-0.6.1/version_info/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     3106 2023-04-23 19:03:46.000000 git_version_info-0.6.1/version_info/main.py
+-rw-rw-rw-   0 root         (0) root         (0)    68749 2023-04-23 19:03:46.000000 git_version_info-0.6.1/versioneer.py
```

### Comparing `git_version_info-0.6/LICENSE` & `git_version_info-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `git_version_info-0.6/PKG-INFO` & `git_version_info-0.6.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git_version_info
-Version: 0.6
+Version: 0.6.1
 Summary: Basic version tagging for python scripts and plots
 Home-page: https://gitlab.com/charlesbaynham/version_info
 Author: Charles Baynham
 License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.com/charlesbaynham/version_info/-/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `git_version_info-0.6/git_version_info.egg-info/PKG-INFO` & `git_version_info-0.6.1/git_version_info.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-version-info
-Version: 0.6
+Version: 0.6.1
 Summary: Basic version tagging for python scripts and plots
 Home-page: https://gitlab.com/charlesbaynham/version_info
 Author: Charles Baynham
 License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.com/charlesbaynham/version_info/-/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `git_version_info-0.6/setup.cfg` & `git_version_info-0.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `git_version_info-0.6/setup.py` & `git_version_info-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `git_version_info-0.6/version_info/main.py` & `git_version_info-0.6.1/version_info/main.py`

 * *Files identical despite different names*

### Comparing `git_version_info-0.6/versioneer.py` & `git_version_info-0.6.1/versioneer.py`

 * *Files identical despite different names*

