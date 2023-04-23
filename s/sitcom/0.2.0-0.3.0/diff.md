# Comparing `tmp/sitcom-0.2.0.tar.gz` & `tmp/sitcom-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitcom-0.2.0.tar", max compression
+gzip compressed data, was "sitcom-0.3.0.tar", last modified: Mon Apr 24 13:23:52 2023, max compression
```

## Comparing `sitcom-0.2.0.tar` & `sitcom-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,19 @@
--rw-r--r--   0        0        0     1069 2023-04-20 09:49:15.900364 sitcom-0.2.0/LICENSE
--rw-r--r--   0        0        0      519 2023-04-20 11:11:42.935081 sitcom-0.2.0/pyproject.toml
--rw-r--r--   0        0        0   669228 2022-11-06 01:18:32.000000 sitcom-0.2.0/src/sitcom/Lato-Semibold.ttf
--rw-r--r--   0        0        0      168 2023-01-18 17:37:14.000000 sitcom-0.2.0/src/sitcom/Pipfile
--rw-r--r--   0        0        0      497 2023-01-18 17:37:14.000000 sitcom-0.2.0/src/sitcom/Pipfile.lock
--rw-r--r--   0        0        0    84116 2023-04-07 11:04:38.000000 sitcom-0.2.0/src/sitcom/Sine_curve.png
--rw-r--r--   0        0        0      313 2023-04-19 08:07:39.639901 sitcom-0.2.0/src/sitcom/__init.py__
--rw-r--r--   0        0        0      697 2023-04-20 06:24:29.200074 sitcom-0.2.0/src/sitcom/__main__.py
--rw-r--r--   0        0        0   539595 2023-04-07 03:05:36.000000 sitcom-0.2.0/src/sitcom/black.png
--rw-r--r--   0        0        0       60 2023-04-19 08:06:00.824504 sitcom-0.2.0/src/sitcom/config.toml
--rw-r--r--   0        0        0     1611 2023-04-18 06:48:20.931330 sitcom-0.2.0/src/sitcom/sfit.py
--rw-r--r--   0        0        0     6413 2023-04-20 11:02:55.695807 sitcom-0.2.0/src/sitcom/sirgraf.py
--rw-r--r--   0        0        0     1693 2023-04-19 12:35:24.173813 sitcom-0.2.0/src/sitcom/sitcom.egg-info/PKG-INFO
--rw-r--r--   0        0        0      325 2023-04-19 12:35:24.189813 sitcom-0.2.0/src/sitcom/sitcom.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2023-04-19 12:35:24.173813 sitcom-0.2.0/src/sitcom/sitcom.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       48 2023-04-19 12:35:24.173813 sitcom-0.2.0/src/sitcom/sitcom.egg-info/requires.txt
--rw-r--r--   0        0        0        7 2023-04-19 12:35:24.173813 sitcom-0.2.0/src/sitcom/sitcom.egg-info/top_level.txt
--rw-r--r--   0        0        0    47356 2023-04-20 11:01:59.431458 sitcom-0.2.0/src/sitcom/st.py
--rw-r--r--   0        0        0    37378 2023-04-20 10:07:37.111202 sitcom-0.2.0/src/sitcom/st1.py
--rw-r--r--   0        0        0     4577 2023-04-20 09:42:27.505828 sitcom-0.2.0/src/sitcom/st2.py
--rw-r--r--   0        0        0   599404 2023-04-07 03:03:58.000000 sitcom-0.2.0/src/sitcom/white.png
--rw-r--r--   0        0        0      636 1970-01-01 00:00:00.000000 sitcom-0.2.0/PKG-INFO
+drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-24 13:23:52.607875 sitcom-0.3.0/
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)     1069 2023-04-19 21:19:14.000000 sitcom-0.3.0/LICENSE
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)      276 2023-04-24 13:23:52.607875 sitcom-0.3.0/PKG-INFO
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)     1349 2023-04-06 17:47:58.000000 sitcom-0.3.0/README.md
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)       38 2023-04-24 13:23:52.607875 sitcom-0.3.0/setup.cfg
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)      459 2023-04-24 13:15:33.000000 sitcom-0.3.0/setup.py
+drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-24 13:23:52.607875 sitcom-0.3.0/sitcom/
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)        0 2023-04-24 12:50:03.000000 sitcom-0.3.0/sitcom/__init__.py
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)    47379 2023-04-24 13:21:26.000000 sitcom-0.3.0/sitcom/__main__.py
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)     1611 2023-04-17 18:18:20.000000 sitcom-0.3.0/sitcom/sfit.py
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)     6413 2023-04-19 22:32:54.000000 sitcom-0.3.0/sitcom/sirgraf.py
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)    37352 2023-04-24 13:18:56.000000 sitcom-0.3.0/sitcom/st1.py
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)     4564 2023-04-24 13:19:28.000000 sitcom-0.3.0/sitcom/st2.py
+drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-24 13:23:52.607875 sitcom-0.3.0/sitcom.egg-info/
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)      276 2023-04-24 13:23:52.000000 sitcom-0.3.0/sitcom.egg-info/PKG-INFO
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)      274 2023-04-24 13:23:52.000000 sitcom-0.3.0/sitcom.egg-info/SOURCES.txt
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)        1 2023-04-24 13:23:52.000000 sitcom-0.3.0/sitcom.egg-info/dependency_links.txt
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)       26 2023-04-24 13:23:52.000000 sitcom-0.3.0/sitcom.egg-info/requires.txt
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)        7 2023-04-24 13:23:52.000000 sitcom-0.3.0/sitcom.egg-info/top_level.txt
```

### Comparing `sitcom-0.2.0/LICENSE` & `sitcom-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sitcom-0.2.0/src/sitcom/sfit.py` & `sitcom-0.3.0/sitcom/sfit.py`

 * *Files identical despite different names*

### Comparing `sitcom-0.2.0/src/sitcom/sirgraf.py` & `sitcom-0.3.0/sitcom/sirgraf.py`

 * *Files identical despite different names*

### Comparing `sitcom-0.2.0/src/sitcom/sitcom.egg-info/PKG-INFO` & `sitcom-0.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1 @@
-Metadata-Version: 2.1
-Name: sitcom
-Version: 0.0.1
-Summary: SITCoM: SiRGraF Integrated Tool for Coronal dynaMics
-Author: Purvi Udhwani
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 SiRGraF Integrated Tool for Coronal dynaMics (SITCoM) is a python package based on Simple Radial Gradient Filter (SiRGraF) used to filter the radial gradient in the white-light coronagraph images and bring out dynamic structures. SITCoM has been developed in Python and integrated with SunPy which enables the user to pass the white-light coronagraph data to the tool and generate radially filtered output with an option to save in various formats as required. The outputs can be viewed in Cartesian and polar coordinate systems. We have implemented the functionality of tracking the transients such as coronal mass ejections (CMEs), outflows, plasma blobs etc. using height-time plots and derive their kinematics. In addition, SITCoM also supports oscillation and waves studies such as for streamer waves. This is done by creating a distance-time plot at a user-defined location (artificial slice) and fitting a sinusoidal function to derive the properties: of time period, amplitude, and damping (if any) which could be used for seismology. We provide the provision to manually or automatically select the data points to be used for fitting. SITCoM is a tool to quickly analyze some properties of coronal dynamics. We present an overview of the SITCoM with the applications for deriving coronal dynamics’ kinematics and oscillation properties.
```

### Comparing `sitcom-0.2.0/src/sitcom/st.py` & `sitcom-0.3.0/sitcom/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import matplotlib.pyplot as plt
 import matplotlib.patches as pa
 import matplotlib.animation as animation
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 
 import numpy as np
 import glob,os,cv2,platform
-import time
+import time,sys
 import sitcom.sirgraf as sf
 
 
 from astropy.io import fits
 from astropy.visualization import ZScaleInterval
 
 if platform.system()=='Windows':
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
@@ -542,17 +542,19 @@
           self.Final.click()
         elif self.s[-1]=="Average":
           self.Average.click()
         elif self.s[-1]=="Movie":
           self.Movie.click()
     def light(self):
         self.t.append('Light')
-        MainWindow.setStyleSheet("QMainWindow{border-image: url(sitcom/src/sitcom/white.png); background-repeat:no-repeat; background-position: center;}")
+        #MainWindow=QtWidgets.QMainWindow()
+        MainWindow.setStyleSheet("QMainWindow{border-image: url(data/white.png); background-repeat:no-repeat; background-position: center;}")
         self.figure.set_facecolor('white')
         mp.rcParams.update({'text.color' : "black",'axes.labelcolor' : "black",'axes.edgecolor':"black",'axes.facecolor':"white",'xtick.color':"black",'ytick.color':"black"})
+        #self.setupUi(MainWindow)
         if self.s==[]:
           pass
         elif self.s[-1]=="Minimum":
           self.Minimum.click()
         elif self.s[-1]=="Filtered":
           self.Filtered.click()
         elif self.s[-1]=="Uniform":
@@ -561,15 +563,15 @@
           self.Final.click()
         elif self.s[-1]=="Average":
           self.Average.click()
         elif self.s[-1]=="Movie":
           self.Movie.click()   
     def dark(self):
         self.t.append('Dark')
-        MainWindow.setStyleSheet("QMainWindow{border-image: url(sitcom/src/sitcom/black.png); background-repeat:no-repeat; background-position: center;}QLabel{color:white;}")
+        MainWindow.setStyleSheet("QMainWindow{border-image: url(data/black.png); background-repeat:no-repeat; background-position: center;}QLabel{color:white;}")
         self.figure.patch.set_facecolor('black')
         mp.rcParams.update({'text.color' : "white",'axes.labelcolor' : "white",'axes.labelcolor' : "white",'axes.edgecolor':"white",'axes.facecolor':"black",'xtick.color':"white",'ytick.color':"white"})
         if self.s==[]:
           pass
         elif self.s[-1]=="Minimum":
           self.Minimum.click()
         elif self.s[-1]=="Filtered":
@@ -907,17 +909,16 @@
     def tplay(self):
       self.ani.event_source.start()
 
 
  
 
 if __name__ == "__main__":
-    import sys
     app = QtWidgets.QApplication(sys.argv)
-    movie=QtGui.QMovie('sitcom/src/load/sitcom.gif')
+    movie=QtGui.QMovie('load/sitcom.gif')
     QtGui.QFontDatabase.addApplicationFont('sitcom/src/font/lato/Lato-Semibold.ttf')
     splash = Load_Window(movie)
     splash.show()
     splash.movie.start()
     start = time.time()
     while movie.state() == QtGui.QMovie.Running and time.time() < start + 4:
         app.processEvents()
```

### Comparing `sitcom-0.2.0/src/sitcom/st1.py` & `sitcom-0.3.0/sitcom/st1.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,25 +191,25 @@
         self.plot_button.setText(_translate("SecondWindow", "Plot"))
         self.plot_button.setEnabled(False)
         self.menuTheme.setTitle(_translate("SecondWindow", "Theme"))
         self.actionLight.setText(_translate("SecondWindow", "Light"))
         self.actionDark.setText(_translate("SecondWindow", "Dark"))
 
     def light(self,SecondWindow):
-        SecondWindow.setStyleSheet("QMainWindow{border-image: url(sitcom/src/sitcom/white.png); background-repeat:no-repeat; background-position: center;}")
+        SecondWindow.setStyleSheet("QMainWindow{border-image: url(data/white.png); background-repeat:no-repeat; background-position: center;}")
         self.figure.set_facecolor('white')
         mp.rcParams.update({'text.color' : "black",'axes.labelcolor' : "black",'axes.edgecolor':"black",'axes.facecolor':"white",'xtick.color':"black",'ytick.color':"black"})
         if self.t==[]:
           pass
         elif self.t[-1]=='Movie':
           self.pmovie.click()
         elif self.t[-1]=='HTP':
           self.htp.click()
     def dark(self,SecondWindow):
-        SecondWindow.setStyleSheet("QMainWindow{border-image: url(sitcom/src/sitcom/black.png); background-repeat:no-repeat; background-position: center;}QLabel{color:white;}")
+        SecondWindow.setStyleSheet("QMainWindow{border-image: url(data/black.png); background-repeat:no-repeat; background-position: center;}QLabel{color:white;}")
         self.figure.patch.set_facecolor('black')
         mp.rcParams.update({'text.color' : "white",'axes.labelcolor' : "white",'axes.edgecolor':"white",'axes.facecolor':"black",'xtick.color':"white",'ytick.color':"white"})
         if self.t==[]:
           pass
         elif self.t[-1]=='Movie':
           self.pmovie.click()
         elif self.t[-1]=='HTP':
```

### Comparing `sitcom-0.2.0/src/sitcom/st2.py` & `sitcom-0.3.0/sitcom/st2.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         SWindow.setObjectName("SWindow")
         SWindow.setFixedWidth(596)
         SWindow.setFixedHeight(442)
         self.centralwidget = QtWidgets.QWidget(SWindow)
         self.centralwidget.setObjectName("centralwidget")
         self.horizontalFrame = QtWidgets.QFrame(self.centralwidget)
         self.horizontalFrame.setGeometry(QtCore.QRect(10, 10, 571, 331))
-        self.horizontalFrame.setStyleSheet("QFrame{border-image: url(sitcom/src/sitcom/Sine_curve.png); background-repeat:no-repeat; background-position: center;}")
+        self.horizontalFrame.setStyleSheet("QFrame{border-image: url(data/Sine_curve.png); background-repeat:no-repeat; background-position: center;}")
         self.horizontalFrame.setObjectName("horizontalFrame")
         self.diagram = QtWidgets.QHBoxLayout(self.horizontalFrame)
         self.diagram.setObjectName("diagram")
         
         self.p0SpinBox = QtWidgets.QDoubleSpinBox(self.centralwidget)
         self.p0SpinBox.setGeometry(QtCore.QRect(40, 370, 61, 41))
         self.p0SpinBox.setRange(-100000,100000)
```

