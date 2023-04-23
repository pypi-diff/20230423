# Comparing `tmp/sitcom-1.0.0.tar.gz` & `tmp/sitcom-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitcom-1.0.0.tar", last modified: Mon Apr 24 13:40:09 2023, max compression
+gzip compressed data, was "sitcom-1.0.1.tar", last modified: Mon Apr 24 13:54:05 2023, max compression
```

## Comparing `sitcom-1.0.0.tar` & `sitcom-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-24 13:40:09.087845 sitcom-1.0.0/
--rw-rw-r--   0 purvi     (1000) purvi     (1000)     1069 2023-04-19 21:19:14.000000 sitcom-1.0.0/LICENSE
--rw-rw-r--   0 purvi     (1000) purvi     (1000)      280 2023-04-24 13:40:09.087845 sitcom-1.0.0/PKG-INFO
--rw-rw-r--   0 purvi     (1000) purvi     (1000)     1349 2023-04-06 17:47:58.000000 sitcom-1.0.0/README.md
--rw-rw-r--   0 purvi     (1000) purvi     (1000)       38 2023-04-24 13:40:09.087845 sitcom-1.0.0/setup.cfg
--rw-rw-r--   0 purvi     (1000) purvi     (1000)      509 2023-04-24 13:38:47.000000 sitcom-1.0.0/setup.py
-drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-24 13:40:09.087845 sitcom-1.0.0/sitcom/
--rw-rw-r--   0 purvi     (1000) purvi     (1000)        0 2023-04-24 12:50:03.000000 sitcom-1.0.0/sitcom/__init__.py
--rw-rw-r--   0 purvi     (1000) purvi     (1000)    47403 2023-04-24 13:36:36.000000 sitcom-1.0.0/sitcom/__main__.py
--rw-rw-r--   0 purvi     (1000) purvi     (1000)     1611 2023-04-17 18:18:20.000000 sitcom-1.0.0/sitcom/sfit.py
--rw-rw-r--   0 purvi     (1000) purvi     (1000)     6413 2023-04-19 22:32:54.000000 sitcom-1.0.0/sitcom/sirgraf.py
--rw-rw-r--   0 purvi     (1000) purvi     (1000)    37366 2023-04-24 13:39:39.000000 sitcom-1.0.0/sitcom/st1.py
--rw-rw-r--   0 purvi     (1000) purvi     (1000)     4571 2023-04-24 13:39:46.000000 sitcom-1.0.0/sitcom/st2.py
-drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-24 13:40:09.087845 sitcom-1.0.0/sitcom.egg-info/
--rw-rw-r--   0 purvi     (1000) purvi     (1000)      280 2023-04-24 13:40:09.000000 sitcom-1.0.0/sitcom.egg-info/PKG-INFO
--rw-rw-r--   0 purvi     (1000) purvi     (1000)      274 2023-04-24 13:40:09.000000 sitcom-1.0.0/sitcom.egg-info/SOURCES.txt
--rw-rw-r--   0 purvi     (1000) purvi     (1000)        1 2023-04-24 13:40:09.000000 sitcom-1.0.0/sitcom.egg-info/dependency_links.txt
--rw-rw-r--   0 purvi     (1000) purvi     (1000)       64 2023-04-24 13:40:09.000000 sitcom-1.0.0/sitcom.egg-info/requires.txt
--rw-rw-r--   0 purvi     (1000) purvi     (1000)        7 2023-04-24 13:40:09.000000 sitcom-1.0.0/sitcom.egg-info/top_level.txt
+drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-24 13:54:05.835819 sitcom-1.0.1/
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)     1069 2023-04-19 21:19:14.000000 sitcom-1.0.1/LICENSE
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)      280 2023-04-24 13:54:05.835819 sitcom-1.0.1/PKG-INFO
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)     1349 2023-04-06 17:47:58.000000 sitcom-1.0.1/README.md
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)       38 2023-04-24 13:54:05.835819 sitcom-1.0.1/setup.cfg
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)      537 2023-04-24 13:53:55.000000 sitcom-1.0.1/setup.py
+drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-24 13:54:05.835819 sitcom-1.0.1/sitcom/
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)        0 2023-04-24 12:50:03.000000 sitcom-1.0.1/sitcom/__init__.py
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)    47375 2023-04-24 13:51:19.000000 sitcom-1.0.1/sitcom/__main__.py
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)     1611 2023-04-17 18:18:20.000000 sitcom-1.0.1/sitcom/sfit.py
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)     6413 2023-04-19 22:32:54.000000 sitcom-1.0.1/sitcom/sirgraf.py
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)    37366 2023-04-24 13:39:39.000000 sitcom-1.0.1/sitcom/st1.py
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)     4571 2023-04-24 13:39:46.000000 sitcom-1.0.1/sitcom/st2.py
+drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-24 13:54:05.835819 sitcom-1.0.1/sitcom.egg-info/
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)      280 2023-04-24 13:54:05.000000 sitcom-1.0.1/sitcom.egg-info/PKG-INFO
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)      274 2023-04-24 13:54:05.000000 sitcom-1.0.1/sitcom.egg-info/SOURCES.txt
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)        1 2023-04-24 13:54:05.000000 sitcom-1.0.1/sitcom.egg-info/dependency_links.txt
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)       64 2023-04-24 13:54:05.000000 sitcom-1.0.1/sitcom.egg-info/requires.txt
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)        7 2023-04-24 13:54:05.000000 sitcom-1.0.1/sitcom.egg-info/top_level.txt
```

### Comparing `sitcom-1.0.0/LICENSE` & `sitcom-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sitcom-1.0.0/README.md` & `sitcom-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `sitcom-1.0.0/sitcom/__main__.py` & `sitcom-1.0.1/sitcom/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         painter.drawPixmap(0, 0, pixmap)
 class Ui_MainWindow(object):     
     def setupUi(self, MainWindow):
         MainWindow.setObjectName("MainWindow")
         MainWindow.setFixedWidth(1000)
         MainWindow.setFixedHeight(550)
         icon = QtGui.QIcon()
-        icon.addPixmap(QtGui.QPixmap("sitcom/icon/cme.png"), QtGui.QIcon.Normal, QtGui.QIcon.On)
+        icon.addPixmap(QtGui.QPixmap("icon/cme.png"), QtGui.QIcon.Normal, QtGui.QIcon.On)
         MainWindow.setWindowIcon(icon)
         MainWindow.setIconSize(QtCore.QSize(40, 30))
         self.centralwidget = QtWidgets.QWidget(MainWindow)
         self.centralwidget.setObjectName("centralwidget")
         #########################################################
         self.Browse = QtWidgets.QPushButton(self.centralwidget)
         self.Browse.setGeometry(QtCore.QRect(330, 10, 89, 31))
@@ -543,15 +543,15 @@
         elif self.s[-1]=="Average":
           self.Average.click()
         elif self.s[-1]=="Movie":
           self.Movie.click()
     def light(self):
         self.t.append('Light')
         #MainWindow=QtWidgets.QMainWindow()
-        MainWindow.setStyleSheet("QMainWindow{border-image: url(sitcom/data/white.png); background-repeat:no-repeat; background-position: center;}")
+        MainWindow.setStyleSheet("QMainWindow{border-image: url(data/white.png); background-repeat:no-repeat; background-position: center;}")
         self.figure.set_facecolor('white')
         mp.rcParams.update({'text.color' : "black",'axes.labelcolor' : "black",'axes.edgecolor':"black",'axes.facecolor':"white",'xtick.color':"black",'ytick.color':"black"})
         #self.setupUi(MainWindow)
         if self.s==[]:
           pass
         elif self.s[-1]=="Minimum":
           self.Minimum.click()
@@ -910,16 +910,16 @@
       self.ani.event_source.start()
 
 
  
 
 if __name__ == "__main__":
     app = QtWidgets.QApplication(sys.argv)
-    movie=QtGui.QMovie('sitcom/load/sitcom.gif')
-    QtGui.QFontDatabase.addApplicationFont('sitcom/font/lato/Lato-Semibold.ttf')
+    movie=QtGui.QMovie('load/sitcom.gif')
+    QtGui.QFontDatabase.addApplicationFont('font/lato/Lato-Semibold.ttf')
     splash = Load_Window(movie)
     splash.show()
     splash.movie.start()
     start = time.time()
     while movie.state() == QtGui.QMovie.Running and time.time() < start + 4:
         app.processEvents()
     MainWindow = QtWidgets.QMainWindow()
```

### Comparing `sitcom-1.0.0/sitcom/sfit.py` & `sitcom-1.0.1/sitcom/sfit.py`

 * *Files identical despite different names*

### Comparing `sitcom-1.0.0/sitcom/sirgraf.py` & `sitcom-1.0.1/sitcom/sirgraf.py`

 * *Files identical despite different names*

### Comparing `sitcom-1.0.0/sitcom/st1.py` & `sitcom-1.0.1/sitcom/st1.py`

 * *Files identical despite different names*

### Comparing `sitcom-1.0.0/sitcom/st2.py` & `sitcom-1.0.1/sitcom/st2.py`

 * *Files identical despite different names*

