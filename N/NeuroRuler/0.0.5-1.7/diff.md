# Comparing `tmp/NeuroRuler-0.0.5.tar.gz` & `tmp/NeuroRuler-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NeuroRuler-0.0.5.tar", last modified: Sun Apr 23 15:08:53 2023, max compression
+gzip compressed data, was "NeuroRuler-1.7.tar", last modified: Sat Apr 15 15:33:02 2023, max compression
```

## Comparing `NeuroRuler-0.0.5.tar` & `NeuroRuler-1.7.tar`

### file list

```diff
@@ -1,70 +1,21 @@
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-23 15:08:53.031606 NeuroRuler-0.0.5/
--rw-r--r--   0 jesse      (501) staff       (20)     1105 2023-04-20 15:32:55.000000 NeuroRuler-0.0.5/LICENSE
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-23 15:08:53.002872 NeuroRuler-0.0.5/NeuroRuler/
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-23 15:08:53.005428 NeuroRuler-0.0.5/NeuroRuler/GUI/
--rw-r--r--   0 jesse      (501) staff       (20)     1613 2023-04-23 15:04:05.000000 NeuroRuler-0.0.5/NeuroRuler/GUI/__init__.py
--rw-r--r--   0 jesse      (501) staff       (20)     6022 2023-04-20 16:07:04.000000 NeuroRuler-0.0.5/NeuroRuler/GUI/helpers.py
--rw-r--r--   0 jesse      (501) staff       (20)    40276 2023-04-23 14:31:54.000000 NeuroRuler-0.0.5/NeuroRuler/GUI/main.py
--rw-r--r--   0 jesse      (501) staff       (20)    47653 2023-04-20 15:32:55.000000 NeuroRuler-0.0.5/NeuroRuler/GUI/mainwindow.ui
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-23 15:08:53.005922 NeuroRuler-0.0.5/NeuroRuler/GUI/static/
--rw-r--r--   0 jesse      (501) staff       (20)     1587 2023-04-20 15:32:55.000000 NeuroRuler-0.0.5/NeuroRuler/GUI/static/hct_logo.png
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-23 15:08:53.001860 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-23 15:08:53.007361 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/dark/
--rw-r--r--   0 jesse      (501) staff       (20)     1530 2023-04-20 15:32:55.000000 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/dark/dark.json
--rw-r--r--   0 jesse      (501) staff       (20)   295673 2023-04-20 15:32:55.000000 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/dark/resources.py
--rw-r--r--   0 jesse      (501) staff       (20)    61516 2023-04-20 15:32:55.000000 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/dark/stylesheet.qss
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-23 15:08:53.009121 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/dark-green/
--rw-r--r--   0 jesse      (501) staff       (20)     1529 2023-04-20 15:32:55.000000 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/dark-green/dark-green.json
--rw-r--r--   0 jesse      (501) staff       (20)   295809 2023-04-20 15:32:55.000000 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/dark-green/resources.py
--rw-r--r--   0 jesse      (501) staff       (20)    62538 2023-04-20 15:32:55.000000 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/dark-green/stylesheet.qss
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-23 15:08:53.010331 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/dark-hct/
--rw-r--r--   0 jesse      (501) staff       (20)     1529 2023-04-20 15:32:55.000000 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/dark-hct/dark-hct.json
--rw-r--r--   0 jesse      (501) staff       (20)   295771 2023-04-20 15:32:55.000000 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/dark-hct/resources.py
--rw-r--r--   0 jesse      (501) staff       (20)    62194 2023-04-20 15:32:55.000000 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/dark-hct/stylesheet.qss
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-23 15:08:53.011261 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/dark-purple/
--rw-r--r--   0 jesse      (501) staff       (20)     1530 2023-04-20 15:32:55.000000 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/dark-purple/dark-purple.json
--rw-r--r--   0 jesse      (501) staff       (20)   295869 2023-04-20 15:32:55.000000 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/dark-purple/resources.py
--rw-r--r--   0 jesse      (501) staff       (20)    62720 2023-04-20 15:32:55.000000 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/dark-purple/stylesheet.qss
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-23 15:08:53.013848 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/light/
--rw-r--r--   0 jesse      (501) staff       (20)     1611 2023-04-20 15:32:55.000000 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/light/light.json
--rw-r--r--   0 jesse      (501) staff       (20)   296029 2023-04-20 15:32:55.000000 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/light/resources.py
--rw-r--r--   0 jesse      (501) staff       (20)    62445 2023-04-20 15:32:55.000000 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/light/stylesheet.qss
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-23 15:08:53.019081 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/light-green/
--rw-r--r--   0 jesse      (501) staff       (20)     1606 2023-04-20 15:32:55.000000 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/light-green/light-green.json
--rw-r--r--   0 jesse      (501) staff       (20)   296171 2023-04-20 15:32:55.000000 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/light-green/resources.py
--rw-r--r--   0 jesse      (501) staff       (20)    63425 2023-04-20 15:32:55.000000 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/light-green/stylesheet.qss
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-23 15:08:53.021262 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/light-hct/
--rw-r--r--   0 jesse      (501) staff       (20)     1606 2023-04-20 15:32:55.000000 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/light-hct/light-hct.json
--rw-r--r--   0 jesse      (501) staff       (20)   296123 2023-04-20 15:32:55.000000 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/light-hct/resources.py
--rw-r--r--   0 jesse      (501) staff       (20)    63081 2023-04-20 15:32:55.000000 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/light-hct/stylesheet.qss
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-23 15:08:53.022597 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/light-purple/
--rw-r--r--   0 jesse      (501) staff       (20)     1610 2023-04-20 15:32:55.000000 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/light-purple/light-purple.json
--rw-r--r--   0 jesse      (501) staff       (20)   296221 2023-04-20 15:32:55.000000 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/light-purple/resources.py
--rw-r--r--   0 jesse      (501) staff       (20)    63647 2023-04-20 15:32:55.000000 NeuroRuler-0.0.5/NeuroRuler/GUI/themes/light-purple/stylesheet.qss
--rw-r--r--   0 jesse      (501) staff       (20)        0 2023-04-20 16:07:04.000000 NeuroRuler-0.0.5/NeuroRuler/__init__.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-23 15:08:53.029919 NeuroRuler-0.0.5/NeuroRuler/utils/
--rw-r--r--   0 jesse      (501) staff       (20)        0 2023-04-20 16:07:04.000000 NeuroRuler-0.0.5/NeuroRuler/utils/__init__.py
--rw-r--r--   0 jesse      (501) staff       (20)     6166 2023-04-23 15:06:12.000000 NeuroRuler-0.0.5/NeuroRuler/utils/constants.py
--rw-r--r--   0 jesse      (501) staff       (20)     2333 2023-04-20 16:07:04.000000 NeuroRuler-0.0.5/NeuroRuler/utils/exceptions.py
--rw-r--r--   0 jesse      (501) staff       (20)     3510 2023-04-20 16:07:04.000000 NeuroRuler-0.0.5/NeuroRuler/utils/global_vars.py
--rw-r--r--   0 jesse      (501) staff       (20)    14569 2023-04-20 16:07:04.000000 NeuroRuler-0.0.5/NeuroRuler/utils/img_helpers.py
--rw-r--r--   0 jesse      (501) staff       (20)     8449 2023-04-20 16:07:04.000000 NeuroRuler-0.0.5/NeuroRuler/utils/imgproc.py
--rw-r--r--   0 jesse      (501) staff       (20)     7801 2023-04-23 15:03:35.000000 NeuroRuler-0.0.5/NeuroRuler/utils/parser.py
--rw-r--r--   0 jesse      (501) staff       (20)     1926 2023-04-23 15:02:30.000000 NeuroRuler-0.0.5/NeuroRuler/utils/user_settings.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-23 15:08:53.003583 NeuroRuler-0.0.5/NeuroRuler.egg-info/
--rw-r--r--   0 jesse      (501) staff       (20)     4598 2023-04-23 15:08:52.000000 NeuroRuler-0.0.5/NeuroRuler.egg-info/PKG-INFO
--rw-r--r--   0 jesse      (501) staff       (20)     1835 2023-04-23 15:08:53.000000 NeuroRuler-0.0.5/NeuroRuler.egg-info/SOURCES.txt
--rw-r--r--   0 jesse      (501) staff       (20)        1 2023-04-23 15:08:52.000000 NeuroRuler-0.0.5/NeuroRuler.egg-info/dependency_links.txt
--rw-r--r--   0 jesse      (501) staff       (20)       89 2023-04-23 15:08:52.000000 NeuroRuler-0.0.5/NeuroRuler.egg-info/requires.txt
--rw-r--r--   0 jesse      (501) staff       (20)       17 2023-04-23 15:08:52.000000 NeuroRuler-0.0.5/NeuroRuler.egg-info/top_level.txt
--rw-r--r--   0 jesse      (501) staff       (20)     4598 2023-04-23 15:08:53.031411 NeuroRuler-0.0.5/PKG-INFO
--rw-r--r--   0 jesse      (501) staff       (20)     3502 2023-04-20 18:58:54.000000 NeuroRuler-0.0.5/README.md
--rw-r--r--   0 jesse      (501) staff       (20)     1341 2023-04-23 14:44:07.000000 NeuroRuler-0.0.5/config.json
--rw-r--r--   0 jesse      (501) staff       (20)     1226 2023-04-20 15:32:55.000000 NeuroRuler-0.0.5/pyproject.toml
--rw-r--r--   0 jesse      (501) staff       (20)       38 2023-04-23 15:08:53.031651 NeuroRuler-0.0.5/setup.cfg
--rw-r--r--   0 jesse      (501) staff       (20)     1978 2023-04-23 14:53:51.000000 NeuroRuler-0.0.5/setup.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-23 15:08:53.031045 NeuroRuler-0.0.5/tests/
--rw-r--r--   0 jesse      (501) staff       (20)      135 2023-04-20 15:32:55.000000 NeuroRuler-0.0.5/tests/__init__.py
--rw-r--r--   0 jesse      (501) staff       (20)     2721 2023-04-20 16:07:04.000000 NeuroRuler-0.0.5/tests/test_img_helpers.py
--rw-r--r--   0 jesse      (501) staff       (20)    12471 2023-04-20 16:07:04.000000 NeuroRuler-0.0.5/tests/test_imgproc.py
--rw-r--r--   0 jesse      (501) staff       (20)      330 2023-04-20 15:32:55.000000 NeuroRuler-0.0.5/tests/test_unittest.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-15 15:33:02.396332 NeuroRuler-1.7/
+-rw-r--r--   0 jesse      (501) staff       (20)     1105 2023-04-03 23:13:14.000000 NeuroRuler-1.7/LICENSE
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-15 15:33:02.394270 NeuroRuler-1.7/NeuroRuler.egg-info/
+-rw-r--r--   0 jesse      (501) staff       (20)     3910 2023-04-15 15:33:02.000000 NeuroRuler-1.7/NeuroRuler.egg-info/PKG-INFO
+-rw-r--r--   0 jesse      (501) staff       (20)      313 2023-04-15 15:33:02.000000 NeuroRuler-1.7/NeuroRuler.egg-info/SOURCES.txt
+-rw-r--r--   0 jesse      (501) staff       (20)        1 2023-04-15 15:33:02.000000 NeuroRuler-1.7/NeuroRuler.egg-info/dependency_links.txt
+-rw-r--r--   0 jesse      (501) staff       (20)      142 2023-04-15 15:33:02.000000 NeuroRuler-1.7/NeuroRuler.egg-info/requires.txt
+-rw-r--r--   0 jesse      (501) staff       (20)        4 2023-04-15 15:33:02.000000 NeuroRuler-1.7/NeuroRuler.egg-info/top_level.txt
+-rw-r--r--   0 jesse      (501) staff       (20)     3910 2023-04-15 15:33:02.396123 NeuroRuler-1.7/PKG-INFO
+-rw-r--r--   0 jesse      (501) staff       (20)     2794 2023-04-15 13:56:33.000000 NeuroRuler-1.7/README.md
+-rw-r--r--   0 jesse      (501) staff       (20)     1445 2023-04-15 15:03:14.000000 NeuroRuler-1.7/pyproject.toml
+-rw-r--r--   0 jesse      (501) staff       (20)       38 2023-04-15 15:33:02.396397 NeuroRuler-1.7/setup.cfg
+-rw-r--r--   0 jesse      (501) staff       (20)     2114 2023-04-15 15:26:51.000000 NeuroRuler-1.7/setup.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-15 15:33:02.392259 NeuroRuler-1.7/src/
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-15 15:33:02.395072 NeuroRuler-1.7/src/GUI/
+-rw-r--r--   0 jesse      (501) staff       (20)     1622 2023-04-15 15:27:32.000000 NeuroRuler-1.7/src/GUI/__init__.py
+-rw-r--r--   0 jesse      (501) staff       (20)     6001 2023-04-15 13:24:15.000000 NeuroRuler-1.7/src/GUI/helpers.py
+-rw-r--r--   0 jesse      (501) staff       (20)    39894 2023-04-15 13:38:34.000000 NeuroRuler-1.7/src/GUI/main.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-15 15:33:02.395671 NeuroRuler-1.7/tests/
+-rw-r--r--   0 jesse      (501) staff       (20)     2707 2023-04-15 13:24:15.000000 NeuroRuler-1.7/tests/test_img_helpers.py
+-rw-r--r--   0 jesse      (501) staff       (20)    12447 2023-04-15 13:38:34.000000 NeuroRuler-1.7/tests/test_imgproc.py
```

### Comparing `NeuroRuler-0.0.5/LICENSE` & `NeuroRuler-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `NeuroRuler-0.0.5/NeuroRuler/GUI/__init__.py` & `NeuroRuler-1.7/src/GUI/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """After installing NeuroRuler via pip, the functions here are importable like so
 
-from NeuroRuler.GUI import {function}
+from {package_name} import gui
 
-where NeuroRuler.GUI is the name of the package this __init__.py file is in."""
+Currently, the package name is GUI (TODO: Change this)"""
 
 import sys
 import os
-import NeuroRuler.GUI.main as main
-import NeuroRuler.utils.parser as parser
+import src.GUI.main as main
+import src.utils.parser as parser
 
+# TODO: Modify when refactoring
+__version__ = "1.7"
 
 def gui() -> None:
     """Start GUI."""
     # Source: https://stackoverflow.com/questions/5047734/in-osx-change-application-name-from-python
     if sys.platform.startswith("darwin"):
         # Set app name, if PyObjC is installed
         # Python 2 has PyObjC preinstalled
```

### Comparing `NeuroRuler-0.0.5/NeuroRuler/GUI/helpers.py` & `NeuroRuler-1.7/src/GUI/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,17 +23,17 @@
     QMessageBox,
 )
 from PyQt6.QtCore import QSize
 from PyQt6.QtCore import Qt
 
 import qimage2ndarray
 
-import NeuroRuler.utils.exceptions as exceptions
-import NeuroRuler.utils.user_settings as user_settings
-from NeuroRuler.utils.constants import deprecated
+import src.utils.exceptions as exceptions
+import src.utils.user_settings as user_settings
+from src.utils.constants import deprecated
 
 MACOS: bool = "macOS" in platform.platform()
 WINDOW_TITLE_PADDING: int = 12
 """Used in InformationDialog to add width to the dialog to prevent the window title from being truncated."""
 
 
 # tl;dr QColor can have alpha (e.g., if we wanted contour color to be transparent)
```

### Comparing `NeuroRuler-0.0.5/NeuroRuler/GUI/main.py` & `NeuroRuler-1.7/src/GUI/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Defines MainWindow and main(), the entrypoint of the GUI.
 
-Loads `NeuroRuler/GUI/mainwindow.ui`, made in QtDesigner.
+Loads `src/GUI/mainwindow.ui`, made in QtDesigner.
 
 Loads `.qss` stylesheets and `resources.py` (icons) files, generated
 by BreezeStyleSheets. Our fork of the repo: https://github.com/COMP523TeamD/BreezeStyleSheets.
 
 If adding a new GUI element (in the GUI or in the menubar, whatever), you'll have to modify
 modify __init__ and settings_view_toggle.
 
@@ -35,34 +35,33 @@
     QWidget,
     QMessageBox,
 )
 from PyQt6.uic.load_ui import loadUi
 from PyQt6.QtCore import Qt, QSize
 
 import pprint
-import pkg_resources
-from NeuroRuler.utils.constants import View, ThresholdFilter
-import NeuroRuler.utils.constants as constants
+from src.utils.constants import View, ThresholdFilter
+import src.utils.constants as constants
 
 # Note, do not use imports like
-# from NeuroRuler.utils.global_vars import IMAGE_DICT
+# from src.utils.global_vars import IMAGE_DICT
 # This would make the global variables not work
-import NeuroRuler.utils.global_vars as global_vars
-import NeuroRuler.utils.imgproc as imgproc
-import NeuroRuler.utils.user_settings as user_settings
-from NeuroRuler.GUI.helpers import (
+import src.utils.global_vars as global_vars
+import src.utils.imgproc as imgproc
+import src.utils.user_settings as user_settings
+from src.GUI.helpers import (
     string_to_QColor,
     mask_QImage,
     sitk_slice_to_qimage,
     ErrorMessageBox,
     InformationMessageBox,
     InformationDialog,
 )
 
-from NeuroRuler.utils.img_helpers import (
+from src.utils.img_helpers import (
     initialize_globals,
     update_images,
     get_curr_image,
     get_curr_image_size,
     get_curr_rotated_slice,
     get_curr_smooth_slice,
     get_curr_metadata,
@@ -70,38 +69,34 @@
     get_curr_otsu_slice,
     get_curr_physical_units,
     get_curr_path,
     get_curr_properties_tuple,
     get_middle_dimension,
 )
 
-import NeuroRuler.utils.img_helpers as img_helpers
+import src.utils.img_helpers as img_helpers
 
 
-PATH_TO_UI_FILE: Path = Path("NeuroRuler") / "GUI" / "mainwindow.ui"
-if not PATH_TO_UI_FILE.exists():
-    PATH_TO_UI_FILE = Path(pkg_resources.resource_filename("NeuroRuler.GUI", "mainwindow.ui"))
-PATH_TO_HCT_LOGO: Path = Path("NeuroRuler") / "GUI" / "static" / "hct_logo.png"
-if not PATH_TO_HCT_LOGO.exists():
-    PATH_TO_HCT_LOGO = Path(pkg_resources.resource_filename("NeuroRuler.GUI", "static/hct_logo.png"))
+PATH_TO_UI_FILE: Path = Path("src") / "GUI" / "mainwindow.ui"
+PATH_TO_HCT_LOGO: Path = Path("src") / "GUI" / "static" / "hct_logo.png"
 
 SETTINGS_VIEW_ENABLED: bool = True
 """Whether the user is able to adjust settings (settings screen) or not
 (circumference and contoured image screen)."""
 
 DEFAULT_CIRCUMFERENCE_LABEL_TEXT: str = "Calculated Circumference: N/A"
 DEFAULT_IMAGE_PATH_LABEL_TEXT: str = "Image path"
-GITHUB_LINK: str = "https://github.com/COMP523TeamD/NeuroRuler"
-DOCUMENTATION_LINK: str = "https://NeuroRuler.readthedocs.io/en/latest/"
+GITHUB_LINK: str = "https://github.com/COMP523TeamD/HeadCircumferenceTool"
+DOCUMENTATION_LINK: str = "https://headcircumferencetool.readthedocs.io/en/latest/"
 DEFAULT_IMAGE_TEXT: str = "Select images using File > Open!"
 DEFAULT_IMAGE_NUM_LABEL_TEXT: str = "Image 0 of 0"
 DEFAULT_IMAGE_STATUS_TEXT: str = "Image path is displayed here."
 
+# We assume units are millimeters if we can't find units in metadata
 MESSAGE_TO_SHOW_IF_UNITS_NOT_FOUND: str = "millimeters (mm)"
-"""We assume units are millimeters if we can't find units in metadata"""
 
 UNSCALED_QPIXMAP: QPixmap
 """Unscaled QPixmap from which the scaled version is rendered in the GUI.
 
 When any slice (rotated, smoothed, previewed) is rendered from an unscaled QImage, this variable is set to the
 QPixmap generated from that unscaled QImage.
 
@@ -888,15 +883,15 @@
     if not len(global_vars.IMAGE_DICT):
         print("No loaded image!")
         return
     curr_properties: tuple = get_curr_properties_tuple()
     fields: tuple = ("center of rotation", "dimensions", "spacing")
     if len(fields) != len(curr_properties):
         print(
-            "Update NeuroRuler/GUI/main.print_properties() !\nNumber of fields and number of properties don't match."
+            "Update src/GUI/main.print_properties() !\nNumber of fields and number of properties don't match."
         )
         exit(1)
     # Pretty sure the dict(zip(...)) goes through fields in alphabetical order
     message: str = pprint.pformat(dict(zip(fields, curr_properties)))
     if user_settings.DISPLAY_ADVANCED_MENU_MESSAGES_IN_TERMINAL:
         print(message)
     else:
@@ -932,18 +927,16 @@
 
 
 def main() -> None:
     """Main entrypoint of GUI."""
     # This import can't go at the top of the file
     # because gui.py.parse_gui_cli() has to set THEME_NAME before the import occurs
     # This imports globally
-    # For example, NeuroRuler/GUI/helpers.py can access resource files without having to import there
-    importlib.import_module(
-        f"NeuroRuler.GUI.themes.{user_settings.THEME_NAME}.resources"
-    )
+    # For example, src/GUI/helpers.py can access resource files without having to import there
+    importlib.import_module(f"src.GUI.themes.{user_settings.THEME_NAME}.resources")
 
     app = QApplication(sys.argv)
 
     # On macOS, sets the application logo in the dock (but no window icon on macOS)
     # TODO
     # On Windows, sets the window icon at the top left of the window (but no dock icon on Windows)
     app.setWindowIcon(QIcon(str(PATH_TO_HCT_LOGO)))
@@ -960,15 +953,15 @@
 
     with open(
         constants.THEME_DIR / user_settings.THEME_NAME / "stylesheet.qss", "r"
     ) as f:
         MAIN_WINDOW.setStyleSheet(f.read())
 
     # Non-zero min width and height is needed to prevent
-    # this bug https://github.com/COMP523TeamD/NeuroRuler/issues/42
+    # this bug https://github.com/COMP523TeamD/HeadCircumferenceTool/issues/42
     # However, this also seems to affect startup GUI size or at least GUI element spacing
     MAIN_WINDOW.setMinimumSize(QSize(1, 1))
     MAIN_WINDOW.resize(
         int(
             user_settings.STARTUP_WIDTH_RATIO * constants.PRIMARY_MONITOR_DIMENSIONS[0]
         ),
         int(
@@ -986,12 +979,12 @@
         os._exit(app.exec())
     except:
         if user_settings.DEBUG:
             print("Exiting")
 
 
 if __name__ == "__main__":
-    import NeuroRuler.utils.parser as parser
+    import src.utils.parser as parser
 
     parser.parse_config_json()
     parser.parse_gui_cli()
     main()
```

### Comparing `NeuroRuler-0.0.5/NeuroRuler.egg-info/PKG-INFO` & `NeuroRuler-1.7/NeuroRuler.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: NeuroRuler
-Version: 0.0.5
+Version: 1.7
 Summary: A program that calculates head circumference from MRI data (.nii, .nii.gz, .nrrd).
-Home-page: https://github.com/COMP523TeamD/NeuroRuler
-Download-URL: https://github.com/COMP523TeamD/NeuroRuler/releases
+Home-page: https://github.com/COMP523TeamD/HeadCircumferenceTool
+Download-URL: https://github.com/COMP523TeamD/HeadCircumferenceTool/releases
 Author: COMP523 Team D
 Author-email: Peifeng He <hankhe@ad.unc.edu>, Madison Lester <madiali@email.unc.edu>, Eric Schneider <eric@cs.unc.edu>, Jesse Wei <jesse@cs.unc.edu>
 Project-URL: Homepage, https://github.com/COMP523TeamD/HeadCircumferenceTool
 Project-URL: Bug Tracker, https://github.com/COMP523TeamD/HeadCircumferenceTool/issues
 Keywords: MRI,NIfTI,NRRD,brain,circumference,PyQt6
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NeuroRuler
 
-![Tests](https://github.com/COMP523TeamD/NeuroRuler/actions/workflows/tests.yml/badge.svg)
+![Tests](https://github.com/COMP523TeamD/HeadCircumferenceTool/actions/workflows/tests.yml/badge.svg)
 ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
 ![Python](https://img.shields.io/badge/python-3670A0?style=plastic&logo=python&logoColor=ffdd54)
 
 > A program that calculates head circumference from MRI data (`.nii`, `.nii.gz`, `.nrrd`).
 
 <p align="center">
   <img src="https://i.imgur.com/nqwqHq8.gif" alt="GUI demo"/>
@@ -36,43 +36,42 @@
 
 If you want 😉 format is bibtex.
 
 ```bibtex
 @misc{neuroruler,
   title={NeuroRuler},
   author={Wei, Jesse and Lester, Madison and He, Peifeng and Schneider, Eric and Styner, Martin},
-  howpublished={\url{https://github.com/COMP523TeamD/NeuroRuler}},
+  howpublished={\url{https://github.com/COMP523TeamD/HeadCircumferenceTool}},
   year={2023}
 }
 ```
 
 ## Install
 
-Your Python version needs to be 3.8+. Check with `python --version`. Install via pip.
+Your Python version needs to be 3.8+. Check with `python --version`. Clone this repo, and install the Python dependencies.
 
 ```sh
-pip install NeuroRuler
+pip install -r requirements.txt
+pip install -i https://test.pypi.org/simple/ NeuroRuler
 ```
 
-If `pip` doesn't work, try `pip3`.
+If `pip` doesn't work, try `pip3` or `python3 -m pip`.
 
-If contributing to this repo, please fork and run `pip install -r requirements.txt` to install additional development dependencies (for code formatting, documentation, etc.). After installing additional dependencies, run `pre-commit install` to enable pre-commit actions.
+If contributing to this repo, please also run `pre-commit install` to run pre-commit actions (i.e., autoformat) on your code before commits.
 
-## Run GUI
+## Start GUI
 
 Run these commands in a Python terminal:
 
 ```py
-from NeuroRuler.GUI import gui
+from GUI import gui
 gui()
 ```
 
-Note: If you make changes to the repo, then use the [`gui.py`](gui.py) script to run the GUI. Changes you make will not be reflected in the package from pip until uploaded to PyPI.
-
-See [release](#release) for how to upload to PyPI or Test PyPI.
+Note: If you make changes to the repo, then use the [`gui.py`](https://github.com/COMP523TeamD/HeadCircumferenceTool/blob/main/gui.py) script to run the GUI. Changes you make will not be reflected in the package from pip until uploaded to PyPi.
 
 ## Configure settings
 
 Edit [`config.json`](config.json).
 
 You can also supply CLI arguments, which override settings in `config.json`.
 
@@ -90,31 +89,18 @@
                         contour color as name (e.g. red) or hex color code rrggbb
 ```
 
 ## Run tests
 
 `pytest`
 
-Our unit tests run on GitHub Actions on push and PR. The results are on GitHub.
-
 ## Documentation
 
-[https://NeuroRuler.readthedocs.io](https://NeuroRuler.readthedocs.io)
+[https://headcircumferencetool.readthedocs.io](https://headcircumferencetool.readthedocs.io)
 
 See [`.readthedocs.yaml`](.readthedocs.yaml) and [`docs/`](docs/).
 
 ## Pre-commit actions
 
 Run `pre-commit install` to enable pre-commit actions.
 
 Before each commit, the actions in [`.pre-commit-config.yaml`](.pre-commit-config.yaml) will be run. Specifically, code will be reformatted with `black`. Note that some file names are excluded, so don't name any source code files those names.
-
-## Release
-
-* [PyPI page](https://pypi.org/project/NeuroRuler/)
-* [TestPyPI page](https://test.pypi.org/project/NeuroRuler/)
-
-To publish to [PyPI](https://pypi.org/project/NeuroRuler/), edit the version number in [`setup.py`](setup.py). Push a **tagged (use the version number) commit** to the `main` branch (can be done through PR) to publish to PyPI (these actions cause the [`pypi.yml`](.github/workflows/pypi.yml) action to run).
-
-The version number on PyPI will be the one in `setup.py`, so make sure it's correct!
-
-To publish on Test PyPI, edit the version number, and push to a branch called `release-testpypi` (create it if it doesn't exist).
```

### Comparing `NeuroRuler-0.0.5/PKG-INFO` & `NeuroRuler-1.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: NeuroRuler
-Version: 0.0.5
+Version: 1.7
 Summary: A program that calculates head circumference from MRI data (.nii, .nii.gz, .nrrd).
-Home-page: https://github.com/COMP523TeamD/NeuroRuler
-Download-URL: https://github.com/COMP523TeamD/NeuroRuler/releases
+Home-page: https://github.com/COMP523TeamD/HeadCircumferenceTool
+Download-URL: https://github.com/COMP523TeamD/HeadCircumferenceTool/releases
 Author: COMP523 Team D
 Author-email: Peifeng He <hankhe@ad.unc.edu>, Madison Lester <madiali@email.unc.edu>, Eric Schneider <eric@cs.unc.edu>, Jesse Wei <jesse@cs.unc.edu>
 Project-URL: Homepage, https://github.com/COMP523TeamD/HeadCircumferenceTool
 Project-URL: Bug Tracker, https://github.com/COMP523TeamD/HeadCircumferenceTool/issues
 Keywords: MRI,NIfTI,NRRD,brain,circumference,PyQt6
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NeuroRuler
 
-![Tests](https://github.com/COMP523TeamD/NeuroRuler/actions/workflows/tests.yml/badge.svg)
+![Tests](https://github.com/COMP523TeamD/HeadCircumferenceTool/actions/workflows/tests.yml/badge.svg)
 ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
 ![Python](https://img.shields.io/badge/python-3670A0?style=plastic&logo=python&logoColor=ffdd54)
 
 > A program that calculates head circumference from MRI data (`.nii`, `.nii.gz`, `.nrrd`).
 
 <p align="center">
   <img src="https://i.imgur.com/nqwqHq8.gif" alt="GUI demo"/>
@@ -36,43 +36,42 @@
 
 If you want 😉 format is bibtex.
 
 ```bibtex
 @misc{neuroruler,
   title={NeuroRuler},
   author={Wei, Jesse and Lester, Madison and He, Peifeng and Schneider, Eric and Styner, Martin},
-  howpublished={\url{https://github.com/COMP523TeamD/NeuroRuler}},
+  howpublished={\url{https://github.com/COMP523TeamD/HeadCircumferenceTool}},
   year={2023}
 }
 ```
 
 ## Install
 
-Your Python version needs to be 3.8+. Check with `python --version`. Install via pip.
+Your Python version needs to be 3.8+. Check with `python --version`. Clone this repo, and install the Python dependencies.
 
 ```sh
-pip install NeuroRuler
+pip install -r requirements.txt
+pip install -i https://test.pypi.org/simple/ NeuroRuler
 ```
 
-If `pip` doesn't work, try `pip3`.
+If `pip` doesn't work, try `pip3` or `python3 -m pip`.
 
-If contributing to this repo, please fork and run `pip install -r requirements.txt` to install additional development dependencies (for code formatting, documentation, etc.). After installing additional dependencies, run `pre-commit install` to enable pre-commit actions.
+If contributing to this repo, please also run `pre-commit install` to run pre-commit actions (i.e., autoformat) on your code before commits.
 
-## Run GUI
+## Start GUI
 
 Run these commands in a Python terminal:
 
 ```py
-from NeuroRuler.GUI import gui
+from GUI import gui
 gui()
 ```
 
-Note: If you make changes to the repo, then use the [`gui.py`](gui.py) script to run the GUI. Changes you make will not be reflected in the package from pip until uploaded to PyPI.
-
-See [release](#release) for how to upload to PyPI or Test PyPI.
+Note: If you make changes to the repo, then use the [`gui.py`](https://github.com/COMP523TeamD/HeadCircumferenceTool/blob/main/gui.py) script to run the GUI. Changes you make will not be reflected in the package from pip until uploaded to PyPi.
 
 ## Configure settings
 
 Edit [`config.json`](config.json).
 
 You can also supply CLI arguments, which override settings in `config.json`.
 
@@ -90,31 +89,18 @@
                         contour color as name (e.g. red) or hex color code rrggbb
 ```
 
 ## Run tests
 
 `pytest`
 
-Our unit tests run on GitHub Actions on push and PR. The results are on GitHub.
-
 ## Documentation
 
-[https://NeuroRuler.readthedocs.io](https://NeuroRuler.readthedocs.io)
+[https://headcircumferencetool.readthedocs.io](https://headcircumferencetool.readthedocs.io)
 
 See [`.readthedocs.yaml`](.readthedocs.yaml) and [`docs/`](docs/).
 
 ## Pre-commit actions
 
 Run `pre-commit install` to enable pre-commit actions.
 
 Before each commit, the actions in [`.pre-commit-config.yaml`](.pre-commit-config.yaml) will be run. Specifically, code will be reformatted with `black`. Note that some file names are excluded, so don't name any source code files those names.
-
-## Release
-
-* [PyPI page](https://pypi.org/project/NeuroRuler/)
-* [TestPyPI page](https://test.pypi.org/project/NeuroRuler/)
-
-To publish to [PyPI](https://pypi.org/project/NeuroRuler/), edit the version number in [`setup.py`](setup.py). Push a **tagged (use the version number) commit** to the `main` branch (can be done through PR) to publish to PyPI (these actions cause the [`pypi.yml`](.github/workflows/pypi.yml) action to run).
-
-The version number on PyPI will be the one in `setup.py`, so make sure it's correct!
-
-To publish on Test PyPI, edit the version number, and push to a branch called `release-testpypi` (create it if it doesn't exist).
```

### Comparing `NeuroRuler-0.0.5/README.md` & `NeuroRuler-1.7/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # NeuroRuler
 
-![Tests](https://github.com/COMP523TeamD/NeuroRuler/actions/workflows/tests.yml/badge.svg)
+![Tests](https://github.com/COMP523TeamD/HeadCircumferenceTool/actions/workflows/tests.yml/badge.svg)
 ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
 ![Python](https://img.shields.io/badge/python-3670A0?style=plastic&logo=python&logoColor=ffdd54)
 
 > A program that calculates head circumference from MRI data (`.nii`, `.nii.gz`, `.nrrd`).
 
 <p align="center">
   <img src="https://i.imgur.com/nqwqHq8.gif" alt="GUI demo"/>
@@ -14,43 +14,42 @@
 
 If you want 😉 format is bibtex.
 
 ```bibtex
 @misc{neuroruler,
   title={NeuroRuler},
   author={Wei, Jesse and Lester, Madison and He, Peifeng and Schneider, Eric and Styner, Martin},
-  howpublished={\url{https://github.com/COMP523TeamD/NeuroRuler}},
+  howpublished={\url{https://github.com/COMP523TeamD/HeadCircumferenceTool}},
   year={2023}
 }
 ```
 
 ## Install
 
-Your Python version needs to be 3.8+. Check with `python --version`. Install via pip.
+Your Python version needs to be 3.8+. Check with `python --version`. Clone this repo, and install the Python dependencies.
 
 ```sh
-pip install NeuroRuler
+pip install -r requirements.txt
+pip install -i https://test.pypi.org/simple/ NeuroRuler
 ```
 
-If `pip` doesn't work, try `pip3`.
+If `pip` doesn't work, try `pip3` or `python3 -m pip`.
 
-If contributing to this repo, please fork and run `pip install -r requirements.txt` to install additional development dependencies (for code formatting, documentation, etc.). After installing additional dependencies, run `pre-commit install` to enable pre-commit actions.
+If contributing to this repo, please also run `pre-commit install` to run pre-commit actions (i.e., autoformat) on your code before commits.
 
-## Run GUI
+## Start GUI
 
 Run these commands in a Python terminal:
 
 ```py
-from NeuroRuler.GUI import gui
+from GUI import gui
 gui()
 ```
 
-Note: If you make changes to the repo, then use the [`gui.py`](gui.py) script to run the GUI. Changes you make will not be reflected in the package from pip until uploaded to PyPI.
-
-See [release](#release) for how to upload to PyPI or Test PyPI.
+Note: If you make changes to the repo, then use the [`gui.py`](https://github.com/COMP523TeamD/HeadCircumferenceTool/blob/main/gui.py) script to run the GUI. Changes you make will not be reflected in the package from pip until uploaded to PyPi.
 
 ## Configure settings
 
 Edit [`config.json`](config.json).
 
 You can also supply CLI arguments, which override settings in `config.json`.
 
@@ -68,31 +67,18 @@
                         contour color as name (e.g. red) or hex color code rrggbb
 ```
 
 ## Run tests
 
 `pytest`
 
-Our unit tests run on GitHub Actions on push and PR. The results are on GitHub.
-
 ## Documentation
 
-[https://NeuroRuler.readthedocs.io](https://NeuroRuler.readthedocs.io)
+[https://headcircumferencetool.readthedocs.io](https://headcircumferencetool.readthedocs.io)
 
 See [`.readthedocs.yaml`](.readthedocs.yaml) and [`docs/`](docs/).
 
 ## Pre-commit actions
 
 Run `pre-commit install` to enable pre-commit actions.
 
 Before each commit, the actions in [`.pre-commit-config.yaml`](.pre-commit-config.yaml) will be run. Specifically, code will be reformatted with `black`. Note that some file names are excluded, so don't name any source code files those names.
-
-## Release
-
-* [PyPI page](https://pypi.org/project/NeuroRuler/)
-* [TestPyPI page](https://test.pypi.org/project/NeuroRuler/)
-
-To publish to [PyPI](https://pypi.org/project/NeuroRuler/), edit the version number in [`setup.py`](setup.py). Push a **tagged (use the version number) commit** to the `main` branch (can be done through PR) to publish to PyPI (these actions cause the [`pypi.yml`](.github/workflows/pypi.yml) action to run).
-
-The version number on PyPI will be the one in `setup.py`, so make sure it's correct!
-
-To publish on Test PyPI, edit the version number, and push to a branch called `release-testpypi` (create it if it doesn't exist).
```

### Comparing `NeuroRuler-0.0.5/pyproject.toml` & `NeuroRuler-1.7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -15,24 +15,35 @@
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Topic :: Multimedia :: Graphics",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
-# dependencies set in setup.py
-# version set in NeuroRuler/GUI/__init__.py
-# keywords set in setup.py
 dynamic = ["dependencies", "version", "keywords"]
 
 [project.urls]
 "Homepage" = "https://github.com/COMP523TeamD/HeadCircumferenceTool"
 "Bug Tracker" = "https://github.com/COMP523TeamD/HeadCircumferenceTool/issues"
 
 [build-system]
 requires = ["setuptools>=67.6.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
 testpaths = [
     "tests",
 ]
+
+[tool.mypy]
+mypy_path = "src"
+check_untyped_defs = true
+disallow_any_generics = true
+ignore_missing_imports = true
+no_implicit_optional = true
+show_error_codes = true
+strict_equality = true
+warn_redundant_casts = true
+warn_return_any = true
+warn_unreachable = true
+warn_unused_configs = true
+no_implicit_reexport = true
```

### Comparing `NeuroRuler-0.0.5/setup.py` & `NeuroRuler-1.7/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,71 @@
 # Source: https://github.com/hmeine/qimage2ndarray/blob/master/setup.py
 
 try:
-    from setuptools import setup, find_packages
+    from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
+from pathlib import Path
+
+# TODO: Modify path when refactoring
+for line in open(Path("src") / "GUI" / "__init__.py"):
+    if line.startswith("__version__"):
+        exec(line)
+
+install_requires: list[str]
+
+print(f"cwd: {Path().cwd()}")
+
+# with open(Path("requirements.txt")) as f:
+#     install_requires = f.read().splitlines()
+
 install_requires: list[str] = [
     "setuptools",
+    "sphinx",
+    "sphinx_rtd_theme",
     "SimpleITK",
     "numpy",
     "argparse",
     "opencv-python",
     "pytest",
     "PyQt6",
     "qimage2ndarray",
     "screeninfo",
+    "black",
+    "pre-commit",
+    "build",
+    "twine",
 ]
-"""All required (i.e., for functionality) dependencies that are installed when running `pip install NeuroRuler`.
-
-Non-functional (e.g., formatting, documentation) dependencies listed in requirements.txt."""
 
 setup(
     name="NeuroRuler",
-    # Version number that appears on PyPI and Test PyPI
-    version="0.0.5",
+    version=__version__,
     description="A program that calculates head circumference from MRI data (`.nii`, `.nii.gz`, `.nrrd`).",
     # Cannot use multiple authors
     # https://stackoverflow.com/questions/9999829/how-to-specify-multiple-authors-emails-in-setup-py
     author="COMP523 Team D",
     author_email="comp523d@gmail.com",
-    url="https://github.com/COMP523TeamD/NeuroRuler",
-    download_url="https://github.com/COMP523TeamD/NeuroRuler/releases",
+    url="https://github.com/COMP523TeamD/HeadCircumferenceTool",
+    download_url="https://github.com/COMP523TeamD/HeadCircumferenceTool/releases",
     keywords=[
         "MRI",
         "NIfTI",
         "NRRD",
         "brain",
         "circumference",
         "PyQt6",
     ],
     install_requires=install_requires,
-    tests_require=install_requires + ["tox", "pytest", "pytest-cov"],
-    # See https://setuptools.pypa.io/en/latest/userguide/package_discovery.html
-    package_dir={"NeuroRuler": "NeuroRuler"},
-    packages=find_packages(),
-    package_data={"NeuroRuler":["GUI/*.ui", "GUI/static/*", "GUI/themes/*/*", "../*.json"]},
+    # We don't need extras_require
+    # See https://stackoverflow.com/questions/41268863/what-is-the-difference-between-extras-require-and-install-requires-in-se
+    # extras_require=dict(),
+    tests_require="pytest",
+    # TODO: Change after refactoring
+    packages=["src.GUI"],
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Operating System :: OS Independent",
         "Topic :: Multimedia :: Graphics",
```

### Comparing `NeuroRuler-0.0.5/tests/test_img_helpers.py` & `NeuroRuler-1.7/tests/test_img_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from NeuroRuler.utils.img_helpers import *
-import NeuroRuler.utils.global_vars as global_vars
+from src.utils.img_helpers import *
+import src.utils.global_vars as global_vars
 
 IMAGE_NAMES: list[str] = [
     "BCP_Dataset_2month_T1w.nrrd",
     "IBIS_Case1_V06_t1w_RAI.nrrd",
     "IBIS_Case2_V12_t1w_RAI.nrrd",
     "IBIS_Case3_V24_t1w_RAI.nrrd",
     "IBIS_Dataset_12month_T1w.nrrd",  # Group 1: 0-4
```

### Comparing `NeuroRuler-0.0.5/tests/test_imgproc.py` & `NeuroRuler-1.7/tests/test_imgproc.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 We use == for float comparison instead of |a-b|<epsilon when the numbers should be *exactly* the same."""
 
 import SimpleITK as sitk
 import numpy as np
 import cv2
 import pytest
 from pathlib import Path
-from NeuroRuler.utils.imgproc import contour, length_of_contour
-import NeuroRuler.utils.exceptions as exceptions
-from NeuroRuler.utils.constants import (
+from src.utils.imgproc import contour, length_of_contour
+import src.utils.exceptions as exceptions
+from src.utils.constants import (
     DATA_DIR,
     NUM_CONTOURS_IN_INVALID_SLICE,
     SUPPORTED_EXTENSIONS,
 )
-from NeuroRuler.utils.global_vars import READER
-from NeuroRuler.utils.img_helpers import get_rotated_slice_hardcoded
+from src.utils.global_vars import READER
+from src.utils.img_helpers import get_rotated_slice_hardcoded
 
 EPSILON: float = 0.001
 """Used for `float` comparisons."""
 
 EXAMPLE_IMAGES: dict[Path, sitk.Image] = dict()
 for extension in SUPPORTED_EXTENSIONS:
     for path in DATA_DIR.glob(extension):
@@ -175,15 +175,15 @@
                         assert length_of_not_copied == length_of_copied
 
 
 @pytest.mark.skip(
     reason="User can see in the GUI the contour generated to confirm its accuracy. Also, this won't matter except for edge cases where the slice is invalid"
 )
 def test_arc_length_of_transposed_matrix_is_same_except_for_invalid_slice():
-    """Per discussion here https://github.com/COMP523TeamD/NeuroRuler/commit/a230a6b57dc34ec433e311d760cc53841ddd6a49,
+    """Per discussion here https://github.com/COMP523TeamD/HeadCircumferenceTool/commit/a230a6b57dc34ec433e311d760cc53841ddd6a49,
 
     Test that the arc length of a contour and its transpose is the same in a specific case. It probably generalizes to the general case.
 
     Specifically, for a matrix and its transpose, cv2.findContours will return [ [[x0 y0]] [[x1 y1]] [[x2 y2]] ... ] and [ [[y0 x0]], [[y1 x1]] [[y2 x2]] ... ]
 
     But cv2.arcLength will apply the distance formula to these contours and that will return the same result.
```

