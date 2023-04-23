# Comparing `tmp/q2gui-0.1.8.tar.gz` & `tmp/q2gui-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "q2gui-0.1.8.tar", max compression
+gzip compressed data, was "q2gui-0.1.9.tar", max compression
```

## Comparing `q2gui-0.1.8.tar` & `q2gui-0.1.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1485 2022-06-24 12:23:43.313507 q2gui-0.1.8/README.md
--rw-r--r--   0        0        0      517 2022-07-01 09:39:23.081170 q2gui-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       38 2022-07-01 09:36:49.292899 q2gui-0.1.8/q2gui/__init__.py
--rw-r--r--   0        0        0      860 2022-06-14 19:03:24.026484 q2gui-0.1.8/q2gui/__main__.py
--rw-r--r--   0        0        0        0 2021-11-07 21:48:48.577075 q2gui-0.1.8/q2gui/pyqt6/__init__.py
--rw-r--r--   0        0        0    12312 2022-06-26 09:35:58.547411 q2gui-0.1.8/q2gui/pyqt6/q2app.py
--rw-r--r--   0        0        0     8687 2022-06-26 09:38:19.743328 q2gui-0.1.8/q2gui/pyqt6/q2form.py
--rw-r--r--   0        0        0      292 2022-06-07 20:23:39.392676 q2gui-0.1.8/q2gui/pyqt6/q2model.py
--rw-r--r--   0        0        0     6492 2022-06-26 09:47:38.799378 q2gui-0.1.8/q2gui/pyqt6/q2widget.py
--rw-r--r--   0        0        0     4108 2022-06-30 17:50:53.772742 q2gui-0.1.8/q2gui/pyqt6/q2window.py
--rw-r--r--   0        0        0      674 2022-06-07 22:08:27.509813 q2gui-0.1.8/q2gui/pyqt6/widgets/__init__.py
--rw-r--r--   0        0        0     1284 2022-06-11 12:01:06.240215 q2gui-0.1.8/q2gui/pyqt6/widgets/q2button.py
--rw-r--r--   0        0        0     1911 2022-06-07 22:08:27.477549 q2gui-0.1.8/q2gui/pyqt6/widgets/q2check.py
--rw-r--r--   0        0        0     4902 2022-06-07 23:01:58.204314 q2gui-0.1.8/q2gui/pyqt6/widgets/q2code.py
--rw-r--r--   0        0        0     1216 2022-06-07 22:08:27.449318 q2gui-0.1.8/q2gui/pyqt6/widgets/q2combo.py
--rw-r--r--   0        0        0     5888 2022-06-26 09:38:14.730045 q2gui-0.1.8/q2gui/pyqt6/widgets/q2date.py
--rw-r--r--   0        0        0      838 2022-06-07 22:08:27.461417 q2gui-0.1.8/q2gui/pyqt6/widgets/q2doublespin.py
--rw-r--r--   0        0        0     2867 2022-06-27 19:30:58.159858 q2gui-0.1.8/q2gui/pyqt6/widgets/q2frame.py
--rw-r--r--   0        0        0     9701 2022-06-10 16:29:58.648171 q2gui-0.1.8/q2gui/pyqt6/widgets/q2grid.py
--rw-r--r--   0        0        0     1642 2022-06-25 18:59:00.919292 q2gui-0.1.8/q2gui/pyqt6/widgets/q2label.py
--rw-r--r--   0        0        0     4191 2022-06-07 22:08:27.477549 q2gui-0.1.8/q2gui/pyqt6/widgets/q2line.py
--rw-r--r--   0        0        0     1162 2022-06-07 22:08:27.477549 q2gui-0.1.8/q2gui/pyqt6/widgets/q2list.py
--rw-r--r--   0        0        0     2632 2022-06-26 09:47:01.185401 q2gui-0.1.8/q2gui/pyqt6/widgets/q2lookup.py
--rw-r--r--   0        0        0      813 2022-06-07 22:08:27.477549 q2gui-0.1.8/q2gui/pyqt6/widgets/q2progressbar.py
--rw-r--r--   0        0        0     2300 2022-06-26 09:55:42.945002 q2gui-0.1.8/q2gui/pyqt6/widgets/q2radio.py
--rw-r--r--   0        0        0     4962 2022-06-07 22:08:27.509813 q2gui-0.1.8/q2gui/pyqt6/widgets/q2relation.py
--rw-r--r--   0        0        0      354 2022-06-07 20:52:13.645764 q2gui-0.1.8/q2gui/pyqt6/widgets/q2scroller.py
--rw-r--r--   0        0        0    15862 2022-06-10 14:26:58.494219 q2gui-0.1.8/q2gui/pyqt6/widgets/q2sheet.py
--rw-r--r--   0        0        0      469 2022-06-07 22:08:27.509813 q2gui-0.1.8/q2gui/pyqt6/widgets/q2space.py
--rw-r--r--   0        0        0      548 2022-06-07 22:08:27.509813 q2gui-0.1.8/q2gui/pyqt6/widgets/q2spin.py
--rw-r--r--   0        0        0     2671 2022-06-26 19:31:59.419828 q2gui-0.1.8/q2gui/pyqt6/widgets/q2tab.py
--rw-r--r--   0        0        0      567 2022-06-07 22:08:27.481582 q2gui-0.1.8/q2gui/pyqt6/widgets/q2text.py
--rw-r--r--   0        0        0     5924 2022-06-26 09:47:24.758829 q2gui-0.1.8/q2gui/pyqt6/widgets/q2toolbar.py
--rw-r--r--   0        0        0      519 2022-06-07 22:08:27.509813 q2gui-0.1.8/q2gui/pyqt6/widgets/q2toolbutton.py
--rw-r--r--   0        0        0    14961 2022-06-27 19:23:16.038599 q2gui-0.1.8/q2gui/q2app.py
--rw-r--r--   0        0        0     7240 2022-06-07 20:23:39.416494 q2gui-0.1.8/q2gui/q2dialogs.py
--rw-r--r--   0        0        0    45210 2022-06-27 19:27:28.352291 q2gui-0.1.8/q2gui/q2form.py
--rw-r--r--   0        0        0    15185 2022-06-27 19:23:16.054592 q2gui-0.1.8/q2gui/q2model.py
--rw-r--r--   0        0        0     1456 2022-05-01 11:47:55.707188 q2gui-0.1.8/q2gui/q2utils.py
--rw-r--r--   0        0        0     3949 2022-06-11 12:02:03.191708 q2gui-0.1.8/q2gui/q2widget.py
--rw-r--r--   0        0        0     2636 2022-06-26 09:43:22.841464 q2gui-0.1.8/q2gui/q2window.py
--rw-r--r--   0        0        0       22 2022-07-01 09:39:23.873166 q2gui-0.1.8/q2gui/version.py
--rw-r--r--   0        0        0     2210 2022-07-01 09:39:25.249227 q2gui-0.1.8/setup.py
--rw-r--r--   0        0        0     2065 2022-07-01 09:39:25.249713 q2gui-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1485 2022-06-24 12:23:43.313507 q2gui-0.1.9/README.md
+-rw-r--r--   0        0        0      517 2022-07-01 15:10:40.217866 q2gui-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       38 2022-07-01 09:36:49.292899 q2gui-0.1.9/q2gui/__init__.py
+-rw-r--r--   0        0        0      860 2022-06-14 19:03:24.026484 q2gui-0.1.9/q2gui/__main__.py
+-rw-r--r--   0        0        0        0 2021-11-07 21:48:48.577075 q2gui-0.1.9/q2gui/pyqt6/__init__.py
+-rw-r--r--   0        0        0    12430 2022-07-01 14:45:12.834807 q2gui-0.1.9/q2gui/pyqt6/q2app.py
+-rw-r--r--   0        0        0     8864 2022-07-01 15:07:27.960200 q2gui-0.1.9/q2gui/pyqt6/q2form.py
+-rw-r--r--   0        0        0      292 2022-06-07 20:23:39.392676 q2gui-0.1.9/q2gui/pyqt6/q2model.py
+-rw-r--r--   0        0        0     6492 2022-06-26 09:47:38.799378 q2gui-0.1.9/q2gui/pyqt6/q2widget.py
+-rw-r--r--   0        0        0     4108 2022-06-30 17:50:53.772742 q2gui-0.1.9/q2gui/pyqt6/q2window.py
+-rw-r--r--   0        0        0      674 2022-06-07 22:08:27.509813 q2gui-0.1.9/q2gui/pyqt6/widgets/__init__.py
+-rw-r--r--   0        0        0     1284 2022-06-11 12:01:06.240215 q2gui-0.1.9/q2gui/pyqt6/widgets/q2button.py
+-rw-r--r--   0        0        0     1911 2022-06-07 22:08:27.477549 q2gui-0.1.9/q2gui/pyqt6/widgets/q2check.py
+-rw-r--r--   0        0        0     4902 2022-06-07 23:01:58.204314 q2gui-0.1.9/q2gui/pyqt6/widgets/q2code.py
+-rw-r--r--   0        0        0     1216 2022-06-07 22:08:27.449318 q2gui-0.1.9/q2gui/pyqt6/widgets/q2combo.py
+-rw-r--r--   0        0        0     5888 2022-06-26 09:38:14.730045 q2gui-0.1.9/q2gui/pyqt6/widgets/q2date.py
+-rw-r--r--   0        0        0      838 2022-06-07 22:08:27.461417 q2gui-0.1.9/q2gui/pyqt6/widgets/q2doublespin.py
+-rw-r--r--   0        0        0     2867 2022-06-27 19:30:58.159858 q2gui-0.1.9/q2gui/pyqt6/widgets/q2frame.py
+-rw-r--r--   0        0        0     9701 2022-06-10 16:29:58.648171 q2gui-0.1.9/q2gui/pyqt6/widgets/q2grid.py
+-rw-r--r--   0        0        0     1642 2022-06-25 18:59:00.919292 q2gui-0.1.9/q2gui/pyqt6/widgets/q2label.py
+-rw-r--r--   0        0        0     4191 2022-06-07 22:08:27.477549 q2gui-0.1.9/q2gui/pyqt6/widgets/q2line.py
+-rw-r--r--   0        0        0     1162 2022-06-07 22:08:27.477549 q2gui-0.1.9/q2gui/pyqt6/widgets/q2list.py
+-rw-r--r--   0        0        0     2632 2022-06-26 09:47:01.185401 q2gui-0.1.9/q2gui/pyqt6/widgets/q2lookup.py
+-rw-r--r--   0        0        0      813 2022-06-07 22:08:27.477549 q2gui-0.1.9/q2gui/pyqt6/widgets/q2progressbar.py
+-rw-r--r--   0        0        0     2300 2022-06-26 09:55:42.945002 q2gui-0.1.9/q2gui/pyqt6/widgets/q2radio.py
+-rw-r--r--   0        0        0     4962 2022-06-07 22:08:27.509813 q2gui-0.1.9/q2gui/pyqt6/widgets/q2relation.py
+-rw-r--r--   0        0        0      354 2022-06-07 20:52:13.645764 q2gui-0.1.9/q2gui/pyqt6/widgets/q2scroller.py
+-rw-r--r--   0        0        0    15862 2022-06-10 14:26:58.494219 q2gui-0.1.9/q2gui/pyqt6/widgets/q2sheet.py
+-rw-r--r--   0        0        0      469 2022-06-07 22:08:27.509813 q2gui-0.1.9/q2gui/pyqt6/widgets/q2space.py
+-rw-r--r--   0        0        0      548 2022-06-07 22:08:27.509813 q2gui-0.1.9/q2gui/pyqt6/widgets/q2spin.py
+-rw-r--r--   0        0        0     2671 2022-06-26 19:31:59.419828 q2gui-0.1.9/q2gui/pyqt6/widgets/q2tab.py
+-rw-r--r--   0        0        0      567 2022-06-07 22:08:27.481582 q2gui-0.1.9/q2gui/pyqt6/widgets/q2text.py
+-rw-r--r--   0        0        0     5924 2022-06-26 09:47:24.758829 q2gui-0.1.9/q2gui/pyqt6/widgets/q2toolbar.py
+-rw-r--r--   0        0        0      519 2022-06-07 22:08:27.509813 q2gui-0.1.9/q2gui/pyqt6/widgets/q2toolbutton.py
+-rw-r--r--   0        0        0    15066 2022-07-01 14:33:58.149853 q2gui-0.1.9/q2gui/q2app.py
+-rw-r--r--   0        0        0     7239 2022-07-01 14:51:40.124591 q2gui-0.1.9/q2gui/q2dialogs.py
+-rw-r--r--   0        0        0    45210 2022-07-01 14:39:19.872289 q2gui-0.1.9/q2gui/q2form.py
+-rw-r--r--   0        0        0    15185 2022-06-27 19:23:16.054592 q2gui-0.1.9/q2gui/q2model.py
+-rw-r--r--   0        0        0     1456 2022-05-01 11:47:55.707188 q2gui-0.1.9/q2gui/q2utils.py
+-rw-r--r--   0        0        0     3949 2022-06-11 12:02:03.191708 q2gui-0.1.9/q2gui/q2widget.py
+-rw-r--r--   0        0        0     2701 2022-07-01 14:50:49.682588 q2gui-0.1.9/q2gui/q2window.py
+-rw-r--r--   0        0        0       22 2022-07-01 15:10:41.153798 q2gui-0.1.9/q2gui/version.py
+-rw-r--r--   0        0        0     2210 2022-07-01 15:10:42.391558 q2gui-0.1.9/setup.py
+-rw-r--r--   0        0        0     2065 2022-07-01 15:10:42.392599 q2gui-0.1.9/PKG-INFO
```

### Comparing `q2gui-0.1.8/README.md` & `q2gui-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.8/pyproject.toml` & `q2gui-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "q2gui"
-version = "0.1.8"
+version = "0.1.9"
 description = "Python GUI toolkit"
 authors = ["Andrei Puchko <andrei.puchko@gmx.de>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `q2gui-0.1.8/q2gui/__main__.py` & `q2gui-0.1.9/q2gui/__main__.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.8/q2gui/pyqt6/q2app.py` & `q2gui-0.1.9/q2gui/pyqt6/q2app.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     QTabWidget,
     QTabBar,
     QMdiArea,
     QSizePolicy,
 )
 
 from PyQt6.QtCore import QEvent, Qt, QCoreApplication, QTimer
-from PyQt6.QtGui import QFontMetrics
+from PyQt6.QtGui import QFontMetrics, QIcon
 
 from q2gui.pyqt6.q2window import Q2QtWindow
 from q2gui.pyqt6.q2window import layout
 import q2gui.q2app as q2app
 
 
 class Q2App(QMainWindow, q2app.Q2App, Q2QtWindow):
@@ -208,14 +208,18 @@
         self.q2_tabwidget.setDisabled(True)
 
     def unlock(self):
         self.menuBar().setDisabled(False)
         self.q2_toolbar.setDisabled(False)
         self.q2_tabwidget.setDisabled(False)
 
+    def set_icon(self, icon_path):
+        self.icon = icon_path
+        self.setWindowIcon(QIcon(self.icon))
+
     def process_events(self):
         QApplication.processEvents()
 
     def show_menubar(self, mode=True):
         q2app.Q2App.show_menubar(self)
         if mode:
             QMainWindow.menuBar(self).show()
```

### Comparing `q2gui-0.1.8/q2gui/pyqt6/q2form.py` & `q2gui-0.1.9/q2gui/pyqt6/q2form.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,22 +123,30 @@
             pos.setY(0)
         if orginal_pos != pos:
             paw.move(pos)
         if size != original_size:
             paw.resize(size)
 
     def set_position(self, left, top):
+        left = int(left)
+        top = int(top)
         paw = self.parent()
         if paw is not None:
             paw.move(left, top)
+        else:
+            self.move(left, top)
 
     def set_size(self, w, h):
+        w = int(w)
+        h = int(h)
         paw = self.parent()
         if paw is not None:
             paw.resize(w, h)
+        else:
+            self.resize(w, h)
 
     def get_position(self):
         parent_mdi_sub_window = self.parent()
         if parent_mdi_sub_window is not None:
             return (parent_mdi_sub_window.pos().x(), parent_mdi_sub_window.pos().y())
 
     def showEvent(self, event=None):
```

### Comparing `q2gui-0.1.8/q2gui/pyqt6/q2widget.py` & `q2gui-0.1.9/q2gui/pyqt6/q2widget.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.8/q2gui/pyqt6/q2window.py` & `q2gui-0.1.9/q2gui/pyqt6/q2window.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.8/q2gui/pyqt6/widgets/__init__.py` & `q2gui-0.1.9/q2gui/pyqt6/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.8/q2gui/pyqt6/widgets/q2button.py` & `q2gui-0.1.9/q2gui/pyqt6/widgets/q2button.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.8/q2gui/pyqt6/widgets/q2check.py` & `q2gui-0.1.9/q2gui/pyqt6/widgets/q2check.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.8/q2gui/pyqt6/widgets/q2code.py` & `q2gui-0.1.9/q2gui/pyqt6/widgets/q2code.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.8/q2gui/pyqt6/widgets/q2combo.py` & `q2gui-0.1.9/q2gui/pyqt6/widgets/q2combo.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.8/q2gui/pyqt6/widgets/q2date.py` & `q2gui-0.1.9/q2gui/pyqt6/widgets/q2date.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.8/q2gui/pyqt6/widgets/q2doublespin.py` & `q2gui-0.1.9/q2gui/pyqt6/widgets/q2doublespin.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.8/q2gui/pyqt6/widgets/q2frame.py` & `q2gui-0.1.9/q2gui/pyqt6/widgets/q2frame.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.8/q2gui/pyqt6/widgets/q2grid.py` & `q2gui-0.1.9/q2gui/pyqt6/widgets/q2grid.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.8/q2gui/pyqt6/widgets/q2label.py` & `q2gui-0.1.9/q2gui/pyqt6/widgets/q2label.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.8/q2gui/pyqt6/widgets/q2line.py` & `q2gui-0.1.9/q2gui/pyqt6/widgets/q2line.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.8/q2gui/pyqt6/widgets/q2list.py` & `q2gui-0.1.9/q2gui/pyqt6/widgets/q2list.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.8/q2gui/pyqt6/widgets/q2lookup.py` & `q2gui-0.1.9/q2gui/pyqt6/widgets/q2lookup.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.8/q2gui/pyqt6/widgets/q2progressbar.py` & `q2gui-0.1.9/q2gui/pyqt6/widgets/q2progressbar.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.8/q2gui/pyqt6/widgets/q2radio.py` & `q2gui-0.1.9/q2gui/pyqt6/widgets/q2radio.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.8/q2gui/pyqt6/widgets/q2relation.py` & `q2gui-0.1.9/q2gui/pyqt6/widgets/q2relation.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.8/q2gui/pyqt6/widgets/q2sheet.py` & `q2gui-0.1.9/q2gui/pyqt6/widgets/q2sheet.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.8/q2gui/pyqt6/widgets/q2spin.py` & `q2gui-0.1.9/q2gui/pyqt6/widgets/q2spin.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.8/q2gui/pyqt6/widgets/q2tab.py` & `q2gui-0.1.9/q2gui/pyqt6/widgets/q2tab.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.8/q2gui/pyqt6/widgets/q2text.py` & `q2gui-0.1.9/q2gui/pyqt6/widgets/q2text.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.8/q2gui/pyqt6/widgets/q2toolbar.py` & `q2gui-0.1.9/q2gui/pyqt6/widgets/q2toolbar.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.8/q2gui/pyqt6/widgets/q2toolbutton.py` & `q2gui-0.1.9/q2gui/pyqt6/widgets/q2toolbutton.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.8/q2gui/q2app.py` & `q2gui-0.1.9/q2gui/q2app.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,24 +350,26 @@
         q2app.q2_app = self
         self.window_title = title
         self.heap = Q2Heap()
         self.db = None
         self.style_file = ""
         self.settings_file = ""
         self.settings_file = self.get_argv("ini")
+        self.icon = None
 
         self.menu_list = []
         self._main_menu = {}
 
         self.settings = Q2Settings(self.settings_file)
         self.style_file = self.get_argv("style")
         if self.style_file == "":
             self.style_file = "q2gui.qss"
         self.set_style_sheet()
         self.menu_list = []
+        self.set_icon("assets/q2gui.ico")
         self.on_init()
 
     def set_style_sheet(self):
         pass
 
     def get_argv(self, argtext: str):
         for x in sys.argv:
@@ -446,14 +448,17 @@
 
     def lock(self):
         pass
 
     def unlock(self):
         pass
 
+    def set_icon(self):
+        pass
+
     def process_events(self):
         pass
 
     def on_init(self):
         pass
 
     def on_start(self):
```

### Comparing `q2gui-0.1.8/q2gui/q2dialogs.py` & `q2gui-0.1.9/q2gui/q2dialogs.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import time
 from q2gui.q2form import Q2Form
 import q2gui.q2app as q2app
 
 
 def center_window(form: Q2Form):
     w, h = q2app.q2_app.get_size()
-    form.form_stack[0].set_size(w * 0.33, h * 0.5)
+    form.form_stack[0].set_size(w * 0.5, h * 0.5)
     form.form_stack[0].set_position(w * 0.33, h * 0.15)
 
 
 def q2Mess(mess="", title="Message"):
     form = Q2Form(title)
     form.do_not_save_geometry = True
     form.add_control("/v")
```

### Comparing `q2gui-0.1.8/q2gui/q2form.py` & `q2gui-0.1.9/q2gui/q2form.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.8/q2gui/q2model.py` & `q2gui-0.1.9/q2gui/q2model.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.8/q2gui/q2utils.py` & `q2gui-0.1.9/q2gui/q2utils.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.8/q2gui/q2widget.py` & `q2gui-0.1.9/q2gui/q2widget.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.8/q2gui/q2window.py` & `q2gui-0.1.9/q2gui/q2window.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,14 +87,16 @@
         top = num(settings.get(self.window_title, "top", "-9999"))
         self.set_position(left, top)
 
         if num(settings.get(self.window_title, "is_max", "0")):
             self.show_maximized()
 
     def save_geometry(self, settings):
+        if self.q2_form.do_not_save_geometry:
+            return
         settings.set(self.window_title, "is_max", f"{self.is_maximized()}")
         if not self.is_maximized():
             pos = self.get_position()
             if pos is not None:
                 settings.set(self.window_title, "left", pos[0])
                 settings.set(self.window_title, "top", pos[1])
             size = self.get_size()
```

### Comparing `q2gui-0.1.8/setup.py` & `q2gui-0.1.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['PyQt6-QScintilla>=2.13.3,<3.0.0', 'PyQt6>=6.3.0,<7.0.0', 'q2db']
 
 setup_kwargs = {
     'name': 'q2gui',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Python GUI toolkit',
     'long_description': '# The light Python GUI builder (currently based on PyQt6)\n\n# How to start \n## With docker && x11:\n```bash\ngit clone https://github.com/AndreiPuchko/q2gui.git\n#                      sudo if necessary \ncd q2gui/docker-x11 && ./build_and_run_menu.sh\n```\n## With PyPI package:\n```bash\npoetry new project_01 && cd project_01 && poetry shell\npoetry add q2gui\ncd project_01\npython -m q2gui > example_app.py && python example_app.py\n```\n## Explore sources:\n```bash\ngit clone https://github.com/AndreiPuchko/q2gui.git\ncd q2gui\npip3 install poetry\npoetry shell\npoetry install\npython3 demo/demo_00.py     # All demo launcher\npython3 demo/demo_01.py     # basic: main menu, form & widgets\npython3 demo/demo_02.py     # forms and forms in form\npython3 demo/demo_03.py     # grid form (CSV data), automatic creation of forms based on data\npython3 demo/demo_04.py     # progressbar, data loading, sorting and filtering\npython3 demo/demo_05.py     # nonmodal form\npython3 demo/demo_06.py     # code editor\npython3 demo/demo_07.py     # database app (4 tables, mock data loading) - requires a q2db package\npython3 demo/demo_08.py     # database app, requires a q2db package, autoschema\n```\n\n## demo/demo_07.py screenshot\n=======\n![Alt text](https://andreipuchko.github.io/q2gui/screenshot.png)\n# Build standalone executable \n(The resulting executable file will appear in the folder  dist/)\n### One file\n```bash\npyinstaller -F demo/demo.py\n```\n\n### One directory\n```bash\npyinstaller -D demo/demo.py\n```\n',
     'author': 'Andrei Puchko',
     'author_email': 'andrei.puchko@gmx.de',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `q2gui-0.1.8/PKG-INFO` & `q2gui-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: q2gui
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python GUI toolkit
 License: Apache 2.0
 Author: Andrei Puchko
 Author-email: andrei.puchko@gmx.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

