# Comparing `tmp/wbpShell-0.1.6.tar.gz` & `tmp/wbpShell-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbpShell-0.1.6.tar", last modified: Sun Jan 29 10:25:50 2023, max compression
+gzip compressed data, was "wbpShell-0.1.7.tar", last modified: Sun Apr 23 04:07:30 2023, max compression
```

## Comparing `wbpShell-0.1.6.tar` & `wbpShell-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 10:25:50.477369 wbpShell-0.1.6/
--rw-rw-rw-   0 root         (0) root         (0)     1080 2023-01-29 10:25:48.000000 wbpShell-0.1.6/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 10:25:50.473369 wbpShell-0.1.6/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 10:25:50.475369 wbpShell-0.1.6/Lib/wbpShell/
--rw-rw-rw-   0 root         (0) root         (0)      564 2023-01-29 10:25:48.000000 wbpShell-0.1.6/Lib/wbpShell/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1323 2023-01-29 10:25:48.000000 wbpShell-0.1.6/Lib/wbpShell/preferences.py
--rw-rw-rw-   0 root         (0) root         (0)     1529 2023-01-29 10:25:48.000000 wbpShell-0.1.6/Lib/wbpShell/shellwin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 10:25:50.477369 wbpShell-0.1.6/Lib/wbpShell.egg-info/
--rw-r--r--   0 root         (0) root         (0)      945 2023-01-29 10:25:50.000000 wbpShell-0.1.6/Lib/wbpShell.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      332 2023-01-29 10:25:50.000000 wbpShell-0.1.6/Lib/wbpShell.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-29 10:25:50.000000 wbpShell-0.1.6/Lib/wbpShell.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-01-29 10:25:50.000000 wbpShell-0.1.6/Lib/wbpShell.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-01-29 10:25:50.000000 wbpShell-0.1.6/Lib/wbpShell.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-01-29 10:25:50.000000 wbpShell-0.1.6/Lib/wbpShell.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      945 2023-01-29 10:25:50.477369 wbpShell-0.1.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-01-29 10:25:48.000000 wbpShell-0.1.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1548 2023-01-29 10:25:50.478370 wbpShell-0.1.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-01-29 10:25:48.000000 wbpShell-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 04:07:30.874070 wbpShell-0.1.7/
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2023-04-23 04:07:28.000000 wbpShell-0.1.7/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 04:07:30.870070 wbpShell-0.1.7/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 04:07:30.873070 wbpShell-0.1.7/Lib/wbpShell/
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-04-23 04:07:28.000000 wbpShell-0.1.7/Lib/wbpShell/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1336 2023-04-23 04:07:28.000000 wbpShell-0.1.7/Lib/wbpShell/preferences.py
+-rw-rw-rw-   0 root         (0) root         (0)     2029 2023-04-23 04:07:28.000000 wbpShell-0.1.7/Lib/wbpShell/shellwin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 04:07:30.874070 wbpShell-0.1.7/Lib/wbpShell.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1935 2023-04-23 04:07:30.000000 wbpShell-0.1.7/Lib/wbpShell.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      332 2023-04-23 04:07:30.000000 wbpShell-0.1.7/Lib/wbpShell.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 04:07:30.000000 wbpShell-0.1.7/Lib/wbpShell.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-04-23 04:07:30.000000 wbpShell-0.1.7/Lib/wbpShell.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-23 04:07:30.000000 wbpShell-0.1.7/Lib/wbpShell.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-23 04:07:30.000000 wbpShell-0.1.7/Lib/wbpShell.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1935 2023-04-23 04:07:30.875070 wbpShell-0.1.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      493 2023-04-23 04:07:28.000000 wbpShell-0.1.7/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2063 2023-04-23 04:07:30.876070 wbpShell-0.1.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-04-23 04:07:28.000000 wbpShell-0.1.7/setup.py
```

### Comparing `wbpShell-0.1.6/LICENSE` & `wbpShell-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wbpShell-0.1.6/Lib/wbpShell/preferences.py` & `wbpShell-0.1.7/Lib/wbpShell/preferences.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 """
 preferences
 ===============================================================================
 
 Manage persistent configuration of the shell window.
 """
 import wx.stc as stc
-
 from wbBase.control.textEditControl import PyTextEditConfig
 from wbBase.dialog.preferences import PreferencesPageBase
 
 name = "Shell"
 
 
 class ShellEditConfig(PyTextEditConfig):
-    def __init__(self):
-        PyTextEditConfig.__init__(self)
+    def __init__(self, parent):
+        super().__init__(parent)
         self.ShowLineNumbers = False
         self.WrapMode = stc.STC_WRAP_WORD
 
     def appendProperties(self, page):
         """Append properties to PreferencesPage"""
         self.registerPropertyEditors(page)
         self.appendProperties_main(page)
         self.appendProperties_caret(page)
         self.appendProperties_selection(page)
         self.appendProperties_line_warp(page)
         self.appendProperties_syntax_colour(page)
 
 
-shellConfig = ShellEditConfig()
-
-
 class ShellPreferences(PreferencesPageBase):
     def __init__(self, parent):
         PreferencesPageBase.__init__(self, parent)
-        shellConfig.appendProperties(self)
+        self.settings = ShellEditConfig(self)
+        self.settings.appendProperties(self)
 
     def applyValues(self):
-        pane = self.app.TopWindow.panelManager.getPaneByCaption(name)
-        shellConfig.getPropertyValues(self)
-        shellConfig.apply(pane.window)
+        win = self.app.TopWindow.panelManager.getWindowByCaption(name)
+        self.settings.getPropertyValues(self)
+        self.settings.apply(win)
 
     def saveValues(self):
         self.applyValues()
-        shellConfig.save()
+        self.settings.save()
```

### Comparing `wbpShell-0.1.6/Lib/wbpShell/shellwin.py` & `wbpShell-0.1.7/Lib/wbpShell/shellwin.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 The shell panel is based on the wxPython 
 `Shell <https://wxpython.org/Phoenix/docs/html/wx.py.shell.Shell.html>`_ 
 control.
 """
 import sys
 
 import wx
+from wx import aui
 from wx.py.shell import Shell as ShellBase
 
+from wbBase.control import PanelMixin
 from wbBase.control.textEditControl import MARGIN_SYMBOLS
 
-from .preferences import shellConfig, name
+from .preferences import ShellEditConfig, name
 
-class Shell(ShellBase):
+class Shell(ShellBase, PanelMixin):
     def __init__(
         self,
         parent,
         id=wx.ID_ANY,
         pos=wx.DefaultPosition,
         size=wx.DefaultSize,
         style=wx.CLIP_CHILDREN | wx.NO_BORDER,
@@ -44,20 +46,39 @@
             introText,
             locals,
             InterpClass,
             startupScript,
             execStartupScript,
             **kwds,
         )
-        shellConfig.load()
-        shellConfig.apply(self)
+        self.settings = ShellEditConfig(self)
+        self.settings.load()
+        self.settings.apply(self)
         self.SetMargins(2, 2)
         self.SetMarginWidth(MARGIN_SYMBOLS, 0)  # not used yet - turn off
 
     def showIntro(self, text:str="") -> None:
         """
         Display introductory text in the shell.
         
         :param text: the text to display
         """
         if text:
             self.write(text)
+
+
+info = aui.AuiPaneInfo()
+info.Name(name)
+info.Caption(name)
+info.MaximizeButton(True)
+info.MinimizeButton(True)
+info.CloseButton(False)
+info.Bottom()
+info.Dock()
+info.Resizable()
+info.FloatingSize(wx.Size(300, 200))
+info.BestSize(wx.Size(800, 400))
+info.MinSize(wx.Size(300, 200))
+info.Icon(wx.ArtProvider.GetBitmap("PYSHELL", wx.ART_FRAME_ICON))
+
+
+shellPanel = (Shell, info)
```

### Comparing `wbpShell-0.1.6/setup.cfg` & `wbpShell-0.1.7/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.6
+current_version = 0.1.7
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
 
@@ -13,63 +13,77 @@
 author = Andreas Eigendorf
 description = Shell panel for Workbench applications.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 license_files = LICENSE
 url = https://gitlab.com/workbench2/workbench-plugins/wbpshell
-platforms = Any
+project_urls = 
+	Source = https://gitlab.com/workbench2/workbench-plugins/wbpshell
+	Documentation = https://workbench2.gitlab.io/workbench-plugins/wbpshell
+	Tracker = https://gitlab.com/workbench2/workbench-plugins/wbpshell/-/issues
+platforms = 
+	WIN32
+	WIN64
+	OSX
+	POSIX
 keywords = 
 	workbench
 	wxPython
 	GUI
 classifiers = 
 	Development Status :: 3 - Alpha
+	License :: OSI Approved :: MIT License
+	Operating System :: MacOS
+	Operating System :: Microsoft :: Windows
+	Operating System :: POSIX
+	Environment :: MacOS X :: Cocoa
+	Environment :: Win32 (MS Windows)
+	Environment :: X11 Applications :: GTK
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: Implementation :: CPython
 	Intended Audience :: Developers
-	Operating System :: OS Independent
-	License :: OSI Approved :: MIT License
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
 wbbase.plugin = shell = wbpShell
 
 [bumpversion:file:Lib/wbpShell/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
 
 [tox:tox]
-min_version = 4.3
+min_version = 4.4
 env_list = 
-	py37
 	py38
 	py39
 	py10
 
 [testenv]
 deps = 
 	pytest
+	pytest-cov
+	coverage
 commands = 
-	pytest
+	pytest --cov=wbpShell --cov-report html:coverage.html
 
 [tool:pytest]
 junit_family = legacy
 testpaths = 
 	tests
 
 [egg_info]
```

