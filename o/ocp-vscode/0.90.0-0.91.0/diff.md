# Comparing `tmp/ocp_vscode-0.90.0.tar.gz` & `tmp/ocp_vscode-0.91.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocp_vscode-0.90.0.tar", last modified: Sat Apr 22 16:14:51 2023, max compression
+gzip compressed data, was "ocp_vscode-0.91.0.tar", last modified: Sun Apr 23 16:11:00 2023, max compression
```

## Comparing `ocp_vscode-0.90.0.tar` & `ocp_vscode-0.91.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-04-22 16:14:51.744052 ocp_vscode-0.90.0/
--rw-r--r--   0 bernhard   (501) staff       (20)    10938 2022-10-05 06:47:11.000000 ocp_vscode-0.90.0/LICENSE
--rw-r--r--   0 bernhard   (501) staff       (20)      809 2023-04-22 16:14:51.744113 ocp_vscode-0.90.0/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)     7866 2023-04-22 14:48:14.000000 ocp_vscode-0.90.0/README.md
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-04-22 16:14:51.743304 ocp_vscode-0.90.0/ocp_vscode/
--rw-r--r--   0 bernhard   (501) staff       (20)      871 2023-04-16 10:39:54.000000 ocp_vscode-0.90.0/ocp_vscode/__init__.py
--rw-r--r--   0 bernhard   (501) staff       (20)     4750 2023-04-21 15:55:51.000000 ocp_vscode-0.90.0/ocp_vscode/animation.py
--rw-r--r--   0 bernhard   (501) staff       (20)     9445 2023-04-22 08:41:23.000000 ocp_vscode-0.90.0/ocp_vscode/config.py
--rw-r--r--   0 bernhard   (501) staff       (20)    17668 2023-04-22 14:45:29.000000 ocp_vscode-0.90.0/ocp_vscode/show.py
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-04-22 16:14:51.743956 ocp_vscode-0.90.0/ocp_vscode.egg-info/
--rw-r--r--   0 bernhard   (501) staff       (20)      809 2023-04-22 16:14:51.000000 ocp_vscode-0.90.0/ocp_vscode.egg-info/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)      325 2023-04-22 16:14:51.000000 ocp_vscode-0.90.0/ocp_vscode.egg-info/SOURCES.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-04-22 16:14:51.000000 ocp_vscode-0.90.0/ocp_vscode.egg-info/dependency_links.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-04-22 16:14:51.000000 ocp_vscode-0.90.0/ocp_vscode.egg-info/not-zip-safe
--rw-r--r--   0 bernhard   (501) staff       (20)       38 2023-04-22 16:14:51.000000 ocp_vscode-0.90.0/ocp_vscode.egg-info/requires.txt
--rw-r--r--   0 bernhard   (501) staff       (20)       11 2023-04-22 16:14:51.000000 ocp_vscode-0.90.0/ocp_vscode.egg-info/top_level.txt
--rw-r--r--   0 bernhard   (501) staff       (20)      901 2023-04-22 16:14:51.744401 ocp_vscode-0.90.0/setup.cfg
--rw-r--r--   0 bernhard   (501) staff       (20)     1137 2023-04-22 16:14:00.000000 ocp_vscode-0.90.0/setup.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-04-23 16:11:00.322681 ocp_vscode-0.91.0/
+-rw-r--r--   0 bernhard   (501) staff       (20)    10938 2022-10-05 06:47:11.000000 ocp_vscode-0.91.0/LICENSE
+-rw-r--r--   0 bernhard   (501) staff       (20)      809 2023-04-23 16:11:00.322735 ocp_vscode-0.91.0/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)     7866 2023-04-23 12:18:09.000000 ocp_vscode-0.91.0/README.md
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-04-23 16:11:00.321864 ocp_vscode-0.91.0/ocp_vscode/
+-rw-r--r--   0 bernhard   (501) staff       (20)      871 2023-04-16 10:39:54.000000 ocp_vscode-0.91.0/ocp_vscode/__init__.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     4750 2023-04-21 15:55:51.000000 ocp_vscode-0.91.0/ocp_vscode/animation.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     9445 2023-04-22 08:41:23.000000 ocp_vscode-0.91.0/ocp_vscode/config.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    17668 2023-04-22 14:45:29.000000 ocp_vscode-0.91.0/ocp_vscode/show.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-04-23 16:11:00.322595 ocp_vscode-0.91.0/ocp_vscode.egg-info/
+-rw-r--r--   0 bernhard   (501) staff       (20)      809 2023-04-23 16:11:00.000000 ocp_vscode-0.91.0/ocp_vscode.egg-info/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)      325 2023-04-23 16:11:00.000000 ocp_vscode-0.91.0/ocp_vscode.egg-info/SOURCES.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-04-23 16:11:00.000000 ocp_vscode-0.91.0/ocp_vscode.egg-info/dependency_links.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-04-23 16:11:00.000000 ocp_vscode-0.91.0/ocp_vscode.egg-info/not-zip-safe
+-rw-r--r--   0 bernhard   (501) staff       (20)       38 2023-04-23 16:11:00.000000 ocp_vscode-0.91.0/ocp_vscode.egg-info/requires.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)       11 2023-04-23 16:11:00.000000 ocp_vscode-0.91.0/ocp_vscode.egg-info/top_level.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)      901 2023-04-23 16:11:00.322997 ocp_vscode-0.91.0/setup.cfg
+-rw-r--r--   0 bernhard   (501) staff       (20)     1137 2023-04-23 12:18:09.000000 ocp_vscode-0.91.0/setup.py
```

### Comparing `ocp_vscode-0.90.0/LICENSE` & `ocp_vscode-0.91.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ocp_vscode-0.90.0/PKG-INFO` & `ocp_vscode-0.91.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp_vscode
-Version: 0.90.0
+Version: 0.91.0
 Summary: OCP CAD Viewer for VSCode
 Home-page: https://github.com/bernhard-42/vscode-ocp-cad-viewer
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: vscode,widgets,CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `ocp_vscode-0.90.0/README.md` & `ocp_vscode-0.91.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 -   A fairly recent version of VS Code, e.g. 1.76.0 or newer
 -   [Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python) installed in VS Code
 -   `pip` available in the Python enviroment that will be used for CAD development
 
 **Steps**:
 
--   Download [ocp-cad-viewer-0.90.0.vsix](https://github.com/bernhard-42/vscode-ocp-cad-viewer/releases/download/v0.90.0/ocp-cad-viewer-0.90.0.vsix)
+-   Download [ocp-cad-viewer-0.91.0.vsix](https://github.com/bernhard-42/vscode-ocp-cad-viewer/releases/download/v0.91.0/ocp-cad-viewer-0.91.0.vsix)
 -   Install it locally in VS Code (_Extensions -> "..." menu -> Install from VSIX..._)
 -   Use the OCP CAD Viewer sidebar to manage both OCP CAD Viewer and python libraries:
     -   Install ocp_vscode via the blue button in the welcome screen of the "Viewer Manager" or by pressing the green down-arrow in the "Library Manager" section of the OCP CAD Viewer sidebar
     -   Install needed CAD libraries by pressing the green down-arrow behind the library name in the "Library Manager" section of the OCP CAD Viewer sidebar
 
 ![Installation](screenshots/ocp_vscode-install.gif)
```

### Comparing `ocp_vscode-0.90.0/ocp_vscode/__init__.py` & `ocp_vscode-0.91.0/ocp_vscode/__init__.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-0.90.0/ocp_vscode/animation.py` & `ocp_vscode-0.91.0/ocp_vscode/animation.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-0.90.0/ocp_vscode/config.py` & `ocp_vscode-0.91.0/ocp_vscode/config.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-0.90.0/ocp_vscode/show.py` & `ocp_vscode-0.91.0/ocp_vscode/show.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-0.90.0/ocp_vscode.egg-info/PKG-INFO` & `ocp_vscode-0.91.0/ocp_vscode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp-vscode
-Version: 0.90.0
+Version: 0.91.0
 Summary: OCP CAD Viewer for VSCode
 Home-page: https://github.com/bernhard-42/vscode-ocp-cad-viewer
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: vscode,widgets,CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `ocp_vscode-0.90.0/setup.cfg` & `ocp_vscode-0.91.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.90.0
+current_version = 0.91.0
 commit = False
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<release>\D*)(?P<build>\d*)
 serialize = 
 	{major}.{minor}.{patch}{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `ocp_vscode-0.90.0/setup.py` & `ocp_vscode-0.91.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup_args = {
     "name": "ocp_vscode",
-    "version": "0.90.0",
+    "version": "0.91.0",
     "description": "OCP CAD Viewer for VSCode",
     "long_description": "An extension to show OCP cad CAD objects (CadQuery, build123d) in VS Code via pythreejs",
     "include_package_data": True,
     "python_requires": ">=3.9",
     "install_requires": ["ocp-tessellate>=1.0.0", "requests", "orjson"],
     "packages": find_packages(),
     "zip_safe": False,
```

