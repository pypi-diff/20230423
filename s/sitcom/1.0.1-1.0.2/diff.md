# Comparing `tmp/sitcom-1.0.1.tar.gz` & `tmp/sitcom-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitcom-1.0.1.tar", last modified: Mon Apr 24 13:54:05 2023, max compression
+gzip compressed data, was "sitcom-1.0.2.tar", last modified: Mon Apr 24 14:18:05 2023, max compression
```

## Comparing `sitcom-1.0.1.tar` & `sitcom-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,28 @@
-drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-24 13:54:05.835819 sitcom-1.0.1/
--rw-rw-r--   0 purvi     (1000) purvi     (1000)     1069 2023-04-19 21:19:14.000000 sitcom-1.0.1/LICENSE
--rw-rw-r--   0 purvi     (1000) purvi     (1000)      280 2023-04-24 13:54:05.835819 sitcom-1.0.1/PKG-INFO
--rw-rw-r--   0 purvi     (1000) purvi     (1000)     1349 2023-04-06 17:47:58.000000 sitcom-1.0.1/README.md
--rw-rw-r--   0 purvi     (1000) purvi     (1000)       38 2023-04-24 13:54:05.835819 sitcom-1.0.1/setup.cfg
--rw-rw-r--   0 purvi     (1000) purvi     (1000)      537 2023-04-24 13:53:55.000000 sitcom-1.0.1/setup.py
-drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-24 13:54:05.835819 sitcom-1.0.1/sitcom/
--rw-rw-r--   0 purvi     (1000) purvi     (1000)        0 2023-04-24 12:50:03.000000 sitcom-1.0.1/sitcom/__init__.py
--rw-rw-r--   0 purvi     (1000) purvi     (1000)    47375 2023-04-24 13:51:19.000000 sitcom-1.0.1/sitcom/__main__.py
--rw-rw-r--   0 purvi     (1000) purvi     (1000)     1611 2023-04-17 18:18:20.000000 sitcom-1.0.1/sitcom/sfit.py
--rw-rw-r--   0 purvi     (1000) purvi     (1000)     6413 2023-04-19 22:32:54.000000 sitcom-1.0.1/sitcom/sirgraf.py
--rw-rw-r--   0 purvi     (1000) purvi     (1000)    37366 2023-04-24 13:39:39.000000 sitcom-1.0.1/sitcom/st1.py
--rw-rw-r--   0 purvi     (1000) purvi     (1000)     4571 2023-04-24 13:39:46.000000 sitcom-1.0.1/sitcom/st2.py
-drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-24 13:54:05.835819 sitcom-1.0.1/sitcom.egg-info/
--rw-rw-r--   0 purvi     (1000) purvi     (1000)      280 2023-04-24 13:54:05.000000 sitcom-1.0.1/sitcom.egg-info/PKG-INFO
--rw-rw-r--   0 purvi     (1000) purvi     (1000)      274 2023-04-24 13:54:05.000000 sitcom-1.0.1/sitcom.egg-info/SOURCES.txt
--rw-rw-r--   0 purvi     (1000) purvi     (1000)        1 2023-04-24 13:54:05.000000 sitcom-1.0.1/sitcom.egg-info/dependency_links.txt
--rw-rw-r--   0 purvi     (1000) purvi     (1000)       64 2023-04-24 13:54:05.000000 sitcom-1.0.1/sitcom.egg-info/requires.txt
--rw-rw-r--   0 purvi     (1000) purvi     (1000)        7 2023-04-24 13:54:05.000000 sitcom-1.0.1/sitcom.egg-info/top_level.txt
+drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-24 14:18:05.639774 sitcom-1.0.2/
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)     1069 2023-04-19 21:19:14.000000 sitcom-1.0.2/LICENSE
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)      280 2023-04-24 14:18:05.639774 sitcom-1.0.2/PKG-INFO
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)     1349 2023-04-06 17:47:58.000000 sitcom-1.0.2/README.md
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)       38 2023-04-24 14:18:05.639774 sitcom-1.0.2/setup.cfg
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)      496 2023-04-24 14:17:53.000000 sitcom-1.0.2/setup.py
+drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-24 14:18:05.627774 sitcom-1.0.2/sitcom/
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)        0 2023-04-24 12:50:03.000000 sitcom-1.0.2/sitcom/__init__.py
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)    47375 2023-04-24 14:14:54.000000 sitcom-1.0.2/sitcom/__main__.py
+drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-24 14:18:05.631774 sitcom-1.0.2/sitcom/data/
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)    84116 2023-04-06 22:34:38.000000 sitcom-1.0.2/sitcom/data/Sine_curve.png
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)   539595 2023-04-06 14:35:36.000000 sitcom-1.0.2/sitcom/data/black.png
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)   599404 2023-04-06 14:33:58.000000 sitcom-1.0.2/sitcom/data/white.png
+drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-24 14:18:05.631774 sitcom-1.0.2/sitcom/icon/
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)     4022 2023-04-19 18:48:40.000000 sitcom-1.0.2/sitcom/icon/cme.ico
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)    29744 2023-02-14 09:29:04.000000 sitcom-1.0.2/sitcom/icon/cme.png
+drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-24 14:18:05.631774 sitcom-1.0.2/sitcom/load/
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)  9159608 2023-02-26 07:43:28.000000 sitcom-1.0.2/sitcom/load/sitcom.gif
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)     1611 2023-04-17 18:18:20.000000 sitcom-1.0.2/sitcom/sfit.py
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)     6413 2023-04-19 22:32:54.000000 sitcom-1.0.2/sitcom/sirgraf.py
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)    37366 2023-04-24 14:16:42.000000 sitcom-1.0.2/sitcom/st1.py
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)     4571 2023-04-24 13:39:46.000000 sitcom-1.0.2/sitcom/st2.py
+drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-24 14:18:05.631774 sitcom-1.0.2/sitcom.egg-info/
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)      280 2023-04-24 14:18:05.000000 sitcom-1.0.2/sitcom.egg-info/PKG-INFO
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)      408 2023-04-24 14:18:05.000000 sitcom-1.0.2/sitcom.egg-info/SOURCES.txt
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)        1 2023-04-24 14:18:05.000000 sitcom-1.0.2/sitcom.egg-info/dependency_links.txt
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)       64 2023-04-24 14:18:05.000000 sitcom-1.0.2/sitcom.egg-info/requires.txt
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)        7 2023-04-24 14:18:05.000000 sitcom-1.0.2/sitcom.egg-info/top_level.txt
```

### Comparing `sitcom-1.0.1/LICENSE` & `sitcom-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sitcom-1.0.1/README.md` & `sitcom-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sitcom-1.0.1/sitcom/__main__.py` & `sitcom-1.0.2/sitcom/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -563,15 +563,15 @@
           self.Final.click()
         elif self.s[-1]=="Average":
           self.Average.click()
         elif self.s[-1]=="Movie":
           self.Movie.click()   
     def dark(self):
         self.t.append('Dark')
-        MainWindow.setStyleSheet("QMainWindow{border-image: url(sitcom/data/black.png); background-repeat:no-repeat; background-position: center;}QLabel{color:white;}")
+        MainWindow.setStyleSheet("QMainWindow{border-image: url(data/black.png); background-repeat:no-repeat; background-position: center;}QLabel{color:white;}")
         self.figure.patch.set_facecolor('black')
         mp.rcParams.update({'text.color' : "white",'axes.labelcolor' : "white",'axes.labelcolor' : "white",'axes.edgecolor':"white",'axes.facecolor':"black",'xtick.color':"white",'ytick.color':"white"})
         if self.s==[]:
           pass
         elif self.s[-1]=="Minimum":
           self.Minimum.click()
         elif self.s[-1]=="Filtered":
@@ -910,15 +910,15 @@
       self.ani.event_source.start()
 
 
  
 
 if __name__ == "__main__":
     app = QtWidgets.QApplication(sys.argv)
-    movie=QtGui.QMovie('load/sitcom.gif')
+    movie=QtGui.QMovie('sitcom/load/sitcom.gif')
     QtGui.QFontDatabase.addApplicationFont('font/lato/Lato-Semibold.ttf')
     splash = Load_Window(movie)
     splash.show()
     splash.movie.start()
     start = time.time()
     while movie.state() == QtGui.QMovie.Running and time.time() < start + 4:
         app.processEvents()
```

### Comparing `sitcom-1.0.1/sitcom/sfit.py` & `sitcom-1.0.2/sitcom/sfit.py`

 * *Files identical despite different names*

### Comparing `sitcom-1.0.1/sitcom/sirgraf.py` & `sitcom-1.0.2/sitcom/sirgraf.py`

 * *Files identical despite different names*

### Comparing `sitcom-1.0.1/sitcom/st1.py` & `sitcom-1.0.2/sitcom/st1.py`

 * *Files identical despite different names*

### Comparing `sitcom-1.0.1/sitcom/st2.py` & `sitcom-1.0.2/sitcom/st2.py`

 * *Files identical despite different names*

