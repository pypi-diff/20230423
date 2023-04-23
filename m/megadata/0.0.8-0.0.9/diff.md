# Comparing `tmp/megadata-0.0.8.tar.gz` & `tmp/megadata-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "megadata-0.0.8.tar", last modified: Mon Oct 10 02:16:05 2022, max compression
+gzip compressed data, was "megadata-0.0.9.tar", last modified: Fri Oct 21 05:19:04 2022, max compression
```

## Comparing `megadata-0.0.8.tar` & `megadata-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-10-10 02:16:05.405559 megadata-0.0.8/
--rw-rw-rw-   0        0        0     1088 2022-09-27 07:15:24.000000 megadata-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      631 2022-10-10 02:16:05.404547 megadata-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      124 2022-09-27 07:55:17.000000 megadata-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-10-10 02:16:05.393781 megadata-0.0.8/megadata/
--rw-rw-rw-   0        0        0        0 2022-09-27 07:41:06.000000 megadata-0.0.8/megadata/__init__.py
--rw-rw-rw-   0        0        0     1643 2022-09-28 03:46:05.000000 megadata-0.0.8/megadata/__main__.py
--rw-rw-rw-   0        0        0     1363 2022-09-27 13:55:17.000000 megadata-0.0.8/megadata/clt_ipc.py
--rw-rw-rw-   0        0        0     4018 2022-09-27 05:21:27.000000 megadata-0.0.8/megadata/myeval.py
--rw-rw-rw-   0        0        0    11588 2022-10-10 02:11:35.000000 megadata-0.0.8/megadata/mypy.py
--rw-rw-rw-   0        0        0     3402 2022-10-10 02:05:06.000000 megadata-0.0.8/megadata/mypyx.py
-drwxrwxrwx   0        0        0        0 2022-10-10 02:16:05.402574 megadata-0.0.8/megadata.egg-info/
--rw-rw-rw-   0        0        0      631 2022-10-10 02:16:05.000000 megadata-0.0.8/megadata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2022-10-10 02:16:05.000000 megadata-0.0.8/megadata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-10 02:16:05.000000 megadata-0.0.8/megadata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-10-10 02:16:05.000000 megadata-0.0.8/megadata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      497 2022-10-08 23:22:15.000000 megadata-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-10-10 02:16:05.406467 megadata-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-10-21 05:19:04.409903 megadata-0.0.9/
+-rw-rw-rw-   0        0        0     1088 2022-09-27 07:15:24.000000 megadata-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      700 2022-10-21 05:19:04.408927 megadata-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2022-10-19 14:45:26.000000 megadata-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-10-21 05:19:04.397230 megadata-0.0.9/megadata/
+-rw-rw-rw-   0        0        0        0 2022-09-27 07:41:06.000000 megadata-0.0.9/megadata/__init__.py
+-rw-rw-rw-   0        0        0     1643 2022-09-28 03:46:05.000000 megadata-0.0.9/megadata/__main__.py
+-rw-rw-rw-   0        0        0     1363 2022-09-27 13:55:17.000000 megadata-0.0.9/megadata/clt_ipc.py
+-rw-rw-rw-   0        0        0     4018 2022-09-27 05:21:27.000000 megadata-0.0.9/megadata/myeval.py
+-rw-rw-rw-   0        0        0    11588 2022-10-10 02:11:35.000000 megadata-0.0.9/megadata/mypy.py
+-rw-rw-rw-   0        0        0     5072 2022-10-21 05:13:10.000000 megadata-0.0.9/megadata/mypyx.py
+drwxrwxrwx   0        0        0        0 2022-10-21 05:19:04.406985 megadata-0.0.9/megadata.egg-info/
+-rw-rw-rw-   0        0        0      700 2022-10-21 05:19:04.000000 megadata-0.0.9/megadata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2022-10-21 05:19:04.000000 megadata-0.0.9/megadata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-21 05:19:04.000000 megadata-0.0.9/megadata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2022-10-21 05:19:04.000000 megadata-0.0.9/megadata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      497 2022-10-21 05:18:27.000000 megadata-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2022-10-21 05:19:04.409903 megadata-0.0.9/setup.cfg
```

### Comparing `megadata-0.0.8/LICENSE` & `megadata-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `megadata-0.0.8/megadata/__main__.py` & `megadata-0.0.9/megadata/__main__.py`

 * *Files identical despite different names*

### Comparing `megadata-0.0.8/megadata/clt_ipc.py` & `megadata-0.0.9/megadata/clt_ipc.py`

 * *Files identical despite different names*

### Comparing `megadata-0.0.8/megadata/myeval.py` & `megadata-0.0.9/megadata/myeval.py`

 * *Files identical despite different names*

### Comparing `megadata-0.0.8/megadata/mypy.py` & `megadata-0.0.9/megadata/mypy.py`

 * *Files identical despite different names*

