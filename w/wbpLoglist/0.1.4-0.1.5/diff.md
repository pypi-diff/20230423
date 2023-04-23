# Comparing `tmp/wbpLoglist-0.1.4.tar.gz` & `tmp/wbpLoglist-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbpLoglist-0.1.4.tar", last modified: Tue Feb  7 14:41:36 2023, max compression
+gzip compressed data, was "wbpLoglist-0.1.5.tar", last modified: Sun Apr 23 01:37:11 2023, max compression
```

## Comparing `wbpLoglist-0.1.4.tar` & `wbpLoglist-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 14:41:36.039551 wbpLoglist-0.1.4/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-02-07 14:41:34.000000 wbpLoglist-0.1.4/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 14:41:36.034550 wbpLoglist-0.1.4/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 14:41:36.036550 wbpLoglist-0.1.4/Lib/wbpLoglist/
--rw-rw-rw-   0 root         (0) root         (0)     1467 2023-02-07 14:41:34.000000 wbpLoglist-0.1.4/Lib/wbpLoglist/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5217 2023-02-07 14:41:34.000000 wbpLoglist-0.1.4/Lib/wbpLoglist/loglistwin.py
--rw-rw-rw-   0 root         (0) root         (0)     1244 2023-02-07 14:41:34.000000 wbpLoglist-0.1.4/Lib/wbpLoglist/preferences.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 14:41:36.038551 wbpLoglist-0.1.4/Lib/wbpLoglist.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1543 2023-02-07 14:41:36.000000 wbpLoglist-0.1.4/Lib/wbpLoglist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      352 2023-02-07 14:41:36.000000 wbpLoglist-0.1.4/Lib/wbpLoglist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-07 14:41:36.000000 wbpLoglist-0.1.4/Lib/wbpLoglist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-02-07 14:41:36.000000 wbpLoglist-0.1.4/Lib/wbpLoglist.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-02-07 14:41:36.000000 wbpLoglist-0.1.4/Lib/wbpLoglist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-02-07 14:41:36.000000 wbpLoglist-0.1.4/Lib/wbpLoglist.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1543 2023-02-07 14:41:36.039551 wbpLoglist-0.1.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-02-07 14:41:34.000000 wbpLoglist-0.1.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2072 2023-02-07 14:41:36.040551 wbpLoglist-0.1.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-02-07 14:41:34.000000 wbpLoglist-0.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:37:11.957045 wbpLoglist-0.1.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-04-23 01:37:10.000000 wbpLoglist-0.1.5/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:37:11.952045 wbpLoglist-0.1.5/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:37:11.955045 wbpLoglist-0.1.5/Lib/wbpLoglist/
+-rw-rw-rw-   0 root         (0) root         (0)     1555 2023-04-23 01:37:10.000000 wbpLoglist-0.1.5/Lib/wbpLoglist/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5700 2023-04-23 01:37:10.000000 wbpLoglist-0.1.5/Lib/wbpLoglist/loglistwin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2023-04-23 01:37:10.000000 wbpLoglist-0.1.5/Lib/wbpLoglist/preferences.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:37:11.957045 wbpLoglist-0.1.5/Lib/wbpLoglist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1967 2023-04-23 01:37:11.000000 wbpLoglist-0.1.5/Lib/wbpLoglist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      352 2023-04-23 01:37:11.000000 wbpLoglist-0.1.5/Lib/wbpLoglist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 01:37:11.000000 wbpLoglist-0.1.5/Lib/wbpLoglist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-04-23 01:37:11.000000 wbpLoglist-0.1.5/Lib/wbpLoglist.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-23 01:37:11.000000 wbpLoglist-0.1.5/Lib/wbpLoglist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-23 01:37:11.000000 wbpLoglist-0.1.5/Lib/wbpLoglist.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1967 2023-04-23 01:37:11.957045 wbpLoglist-0.1.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-04-23 01:37:10.000000 wbpLoglist-0.1.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2094 2023-04-23 01:37:11.958045 wbpLoglist-0.1.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-04-23 01:37:10.000000 wbpLoglist-0.1.5/setup.py
```

### Comparing `wbpLoglist-0.1.4/LICENSE` & `wbpLoglist-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wbpLoglist-0.1.4/Lib/wbpLoglist/loglistwin.py` & `wbpLoglist-0.1.5/Lib/wbpLoglist/loglistwin.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,16 +5,19 @@
 Panel to show logging output in a list control
 """
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
 from datetime import datetime
 import wx
+from wx import aui
 import wx.lib.mixins.listctrl as listmix
 
+from .preferences import name
+
 if TYPE_CHECKING:
     from wbBase.application import App
 
 
 class ListLog(wx.Log):
     """
     Log target to show logging info in a list control.
@@ -145,12 +148,29 @@
             wx.FD_SAVE | wx.FD_OVERWRITE_PROMPT,
             self,
         )
         if fileName:
             self.saveLog(fileName)
 
     def saveLog(self, fileName:str) -> None:
-        logFile = open(fileName, "w")
-        logFile.write("LEVEL      TIMESTAMP             MESSAGE\n")
-        for i in range(self.ItemCount):
-            logFile.write(self.GetItem(i, 0).Text.strip() + "\n")
-        logFile.close()
+        with open(fileName, "w") as logFile:
+            logFile.write("LEVEL      TIMESTAMP             MESSAGE\n")
+            for i in range(self.ItemCount):
+                logFile.write(self.GetItem(i, 0).Text.strip() + "\n")
+
+
+logListInfo = aui.AuiPaneInfo()
+logListInfo.Name(name)
+logListInfo.Caption(name)
+logListInfo.Dock()
+logListInfo.Bottom()
+logListInfo.Resizable()
+logListInfo.Hide()
+logListInfo.MaximizeButton(True)
+logListInfo.MinimizeButton(True)
+logListInfo.CloseButton(False)
+logListInfo.MinSize(150, 100)
+logListInfo.BestSize(250, 200)
+logListInfo.Icon(wx.ArtProvider.GetBitmap("LOG", wx.ART_FRAME_ICON))
+
+
+logListPanel = (LogListWindow, logListInfo)
```

### Comparing `wbpLoglist-0.1.4/Lib/wbpLoglist/preferences.py` & `wbpLoglist-0.1.5/Lib/wbpLoglist/preferences.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 ===============================================================================
 """
 import wx
 import wx.propgrid as pg
 
 from wbBase.dialog.preferences import PreferencesPageBase
 
+name = "LogList"
+
 
 class LogListPreferences(PreferencesPageBase):
     def __init__(self, parent) -> None:
         PreferencesPageBase.__init__(self, parent)
         logLabels = [
             "FatalError",
             "Error",
```

### Comparing `wbpLoglist-0.1.4/setup.cfg` & `wbpLoglist-0.1.5/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.4
+current_version = 0.1.5
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
 
@@ -36,44 +36,43 @@
 	Operating System :: MacOS
 	Operating System :: Microsoft :: Windows
 	Operating System :: POSIX
 	Environment :: MacOS X :: Cocoa
 	Environment :: Win32 (MS Windows)
 	Environment :: X11 Applications :: GTK
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: Implementation :: CPython
 	Intended Audience :: Developers
 	Topic :: Software Development :: Libraries
 	Topic :: Software Development :: User Interfaces
 
 [options]
 package_dir = 
 	=Lib
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8,<3.11
 install_requires = 
-	wbBase>=0.1.46
+	wbBase>=0.1.54
 
 [options.packages.find]
 where = Lib
 
 [options.entry_points]
 wbbase.plugin = loglist = wbpLoglist
 
 [bumpversion:file:Lib/wbpLoglist/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
 
 [tox:tox]
-min_version = 4.3
+min_version = 4.4
 env_list = 
-	py37
 	py38
 	py39
 	py310
 
 [testenv]
 deps = 
 	pytest
```

