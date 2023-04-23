# Comparing `tmp/dotscanner-1.2.8.tar.gz` & `tmp/dotscanner-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dotscanner-1.2.8.tar", last modified: Sat Oct 29 03:08:39 2022, max compression
+gzip compressed data, was "dist/dotscanner-1.2.9.tar", last modified: Sun Oct 30 13:50:51 2022, max compression
```

## Comparing `dotscanner-1.2.8.tar` & `dotscanner-1.2.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2022-10-29 03:08:39.097633 dotscanner-1.2.8/
--rw-r--r--   0 holly      (501) staff       (20)    13797 2022-10-29 03:08:39.097472 dotscanner-1.2.8/PKG-INFO
--rw-r--r--   0 holly      (501) staff       (20)    11731 2022-10-29 03:07:19.000000 dotscanner-1.2.8/README.md
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2022-10-29 03:08:39.093737 dotscanner-1.2.8/dotscanner/
--rw-r--r--   0 holly      (501) staff       (20)        0 2022-10-29 01:56:24.000000 dotscanner-1.2.8/dotscanner/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     2183 2022-10-29 01:56:24.000000 dotscanner-1.2.8/dotscanner/__main__.py
--rw-r--r--   0 holly      (501) staff       (20)     8425 2022-10-29 01:56:24.000000 dotscanner-1.2.8/dotscanner/dataprocessing.py
--rw-r--r--   0 holly      (501) staff       (20)     5306 2022-10-29 01:56:24.000000 dotscanner-1.2.8/dotscanner/density.py
--rw-r--r--   0 holly      (501) staff       (20)     3291 2022-10-29 01:56:24.000000 dotscanner-1.2.8/dotscanner/files.py
--rw-r--r--   0 holly      (501) staff       (20)     8582 2022-10-29 01:56:24.000000 dotscanner-1.2.8/dotscanner/lifetime.py
--rw-r--r--   0 holly      (501) staff       (20)     3996 2022-10-29 01:56:24.000000 dotscanner-1.2.8/dotscanner/strings.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2022-10-29 03:08:39.095727 dotscanner-1.2.8/dotscanner/ui/
--rw-r--r--   0 holly      (501) staff       (20)     5240 2022-10-29 03:07:29.000000 dotscanner-1.2.8/dotscanner/ui/DefaultUserSettingsEditor.py
--rw-r--r--   0 holly      (501) staff       (20)     1879 2022-10-29 03:07:28.000000 dotscanner-1.2.8/dotscanner/ui/DialogWindow.py
--rw-r--r--   0 holly      (501) staff       (20)     3468 2022-10-29 01:56:24.000000 dotscanner-1.2.8/dotscanner/ui/MicroscopeImage.py
--rw-r--r--   0 holly      (501) staff       (20)     5145 2022-10-29 01:56:24.000000 dotscanner-1.2.8/dotscanner/ui/RegionSelector.py
--rw-r--r--   0 holly      (501) staff       (20)    15009 2022-10-29 01:56:24.000000 dotscanner-1.2.8/dotscanner/ui/ThresholdAdjuster.py
--rw-r--r--   0 holly      (501) staff       (20)    10250 2022-10-29 01:56:24.000000 dotscanner-1.2.8/dotscanner/ui/UserSettings.py
--rw-r--r--   0 holly      (501) staff       (20)        0 2022-10-29 01:56:24.000000 dotscanner-1.2.8/dotscanner/ui/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     3135 2022-10-29 01:56:24.000000 dotscanner-1.2.8/dotscanner/ui/window.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2022-10-29 03:08:39.094536 dotscanner-1.2.8/dotscanner.egg-info/
--rw-r--r--   0 holly      (501) staff       (20)    13797 2022-10-29 03:08:39.000000 dotscanner-1.2.8/dotscanner.egg-info/PKG-INFO
--rw-r--r--   0 holly      (501) staff       (20)      898 2022-10-29 03:08:39.000000 dotscanner-1.2.8/dotscanner.egg-info/SOURCES.txt
--rw-r--r--   0 holly      (501) staff       (20)        1 2022-10-29 03:08:39.000000 dotscanner-1.2.8/dotscanner.egg-info/dependency_links.txt
--rw-r--r--   0 holly      (501) staff       (20)       57 2022-10-29 03:08:39.000000 dotscanner-1.2.8/dotscanner.egg-info/entry_points.txt
--rw-r--r--   0 holly      (501) staff       (20)       17 2022-10-29 03:08:39.000000 dotscanner-1.2.8/dotscanner.egg-info/requires.txt
--rw-r--r--   0 holly      (501) staff       (20)       26 2022-10-29 03:08:39.000000 dotscanner-1.2.8/dotscanner.egg-info/top_level.txt
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2022-10-29 03:08:39.096085 dotscanner-1.2.8/settings/
--rw-r--r--   0 holly      (501) staff       (20)        0 2022-10-29 01:56:24.000000 dotscanner-1.2.8/settings/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     5812 2022-10-29 01:56:24.000000 dotscanner-1.2.8/settings/config.py
--rw-r--r--   0 holly      (501) staff       (20)    10229 2022-10-29 01:56:24.000000 dotscanner-1.2.8/settings/configmanagement.py
--rw-r--r--   0 holly      (501) staff       (20)       38 2022-10-29 03:08:39.097691 dotscanner-1.2.8/setup.cfg
--rw-r--r--   0 holly      (501) staff       (20)     1633 2022-10-29 03:07:27.000000 dotscanner-1.2.8/setup.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2022-10-29 03:08:39.097183 dotscanner-1.2.8/tests/
--rw-r--r--   0 holly      (501) staff       (20)      554 2022-10-29 01:56:24.000000 dotscanner-1.2.8/tests/FakeUserSettings.py
--rw-r--r--   0 holly      (501) staff       (20)        0 2022-10-29 01:56:24.000000 dotscanner-1.2.8/tests/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     3613 2022-10-29 01:56:24.000000 dotscanner-1.2.8/tests/test_MicroscopeImage.py
--rw-r--r--   0 holly      (501) staff       (20)     5098 2022-10-29 01:56:24.000000 dotscanner-1.2.8/tests/test_dataprocessing.py
--rw-r--r--   0 holly      (501) staff       (20)     1690 2022-10-29 01:56:24.000000 dotscanner-1.2.8/tests/test_density.py
--rw-r--r--   0 holly      (501) staff       (20)     4802 2022-10-29 01:56:24.000000 dotscanner-1.2.8/tests/test_files.py
--rw-r--r--   0 holly      (501) staff       (20)     9963 2022-10-29 01:56:24.000000 dotscanner-1.2.8/tests/test_lifetime.py
--rw-r--r--   0 holly      (501) staff       (20)     2155 2022-10-29 01:56:24.000000 dotscanner-1.2.8/tests/test_strings.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2022-10-30 13:50:51.899818 dotscanner-1.2.9/
+-rw-r--r--   0 holly      (501) staff       (20)    13890 2022-10-30 13:50:51.899591 dotscanner-1.2.9/PKG-INFO
+-rw-r--r--   0 holly      (501) staff       (20)    11824 2022-10-30 11:35:44.000000 dotscanner-1.2.9/README.md
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2022-10-30 13:50:51.893289 dotscanner-1.2.9/dotscanner/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2022-10-30 11:35:44.000000 dotscanner-1.2.9/dotscanner/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     2183 2022-10-30 11:35:44.000000 dotscanner-1.2.9/dotscanner/__main__.py
+-rw-r--r--   0 holly      (501) staff       (20)     8425 2022-10-30 11:35:44.000000 dotscanner-1.2.9/dotscanner/dataprocessing.py
+-rw-r--r--   0 holly      (501) staff       (20)     5306 2022-10-30 11:35:44.000000 dotscanner-1.2.9/dotscanner/density.py
+-rw-r--r--   0 holly      (501) staff       (20)     3291 2022-10-30 11:35:44.000000 dotscanner-1.2.9/dotscanner/files.py
+-rw-r--r--   0 holly      (501) staff       (20)     8582 2022-10-30 11:35:44.000000 dotscanner-1.2.9/dotscanner/lifetime.py
+-rw-r--r--   0 holly      (501) staff       (20)     4098 2022-10-30 13:47:00.000000 dotscanner-1.2.9/dotscanner/strings.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2022-10-30 13:50:51.896602 dotscanner-1.2.9/dotscanner/ui/
+-rw-r--r--   0 holly      (501) staff       (20)     5240 2022-10-30 11:35:44.000000 dotscanner-1.2.9/dotscanner/ui/DefaultUserSettingsEditor.py
+-rw-r--r--   0 holly      (501) staff       (20)     1879 2022-10-30 11:35:44.000000 dotscanner-1.2.9/dotscanner/ui/DialogWindow.py
+-rw-r--r--   0 holly      (501) staff       (20)     3477 2022-10-30 13:03:04.000000 dotscanner-1.2.9/dotscanner/ui/MicroscopeImage.py
+-rw-r--r--   0 holly      (501) staff       (20)     5145 2022-10-30 11:35:44.000000 dotscanner-1.2.9/dotscanner/ui/RegionSelector.py
+-rw-r--r--   0 holly      (501) staff       (20)    14800 2022-10-30 13:28:42.000000 dotscanner-1.2.9/dotscanner/ui/ThresholdAdjuster.py
+-rw-r--r--   0 holly      (501) staff       (20)    10626 2022-10-30 13:35:09.000000 dotscanner-1.2.9/dotscanner/ui/UserSettings.py
+-rw-r--r--   0 holly      (501) staff       (20)        0 2022-10-30 11:35:44.000000 dotscanner-1.2.9/dotscanner/ui/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     3135 2022-10-30 11:35:44.000000 dotscanner-1.2.9/dotscanner/ui/window.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2022-10-30 13:50:51.894608 dotscanner-1.2.9/dotscanner.egg-info/
+-rw-r--r--   0 holly      (501) staff       (20)    13890 2022-10-30 13:50:51.000000 dotscanner-1.2.9/dotscanner.egg-info/PKG-INFO
+-rw-r--r--   0 holly      (501) staff       (20)      898 2022-10-30 13:50:51.000000 dotscanner-1.2.9/dotscanner.egg-info/SOURCES.txt
+-rw-r--r--   0 holly      (501) staff       (20)        1 2022-10-30 13:50:51.000000 dotscanner-1.2.9/dotscanner.egg-info/dependency_links.txt
+-rw-r--r--   0 holly      (501) staff       (20)       57 2022-10-30 13:50:51.000000 dotscanner-1.2.9/dotscanner.egg-info/entry_points.txt
+-rw-r--r--   0 holly      (501) staff       (20)       17 2022-10-30 13:50:51.000000 dotscanner-1.2.9/dotscanner.egg-info/requires.txt
+-rw-r--r--   0 holly      (501) staff       (20)       26 2022-10-30 13:50:51.000000 dotscanner-1.2.9/dotscanner.egg-info/top_level.txt
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2022-10-30 13:50:51.897293 dotscanner-1.2.9/settings/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2022-10-30 11:35:44.000000 dotscanner-1.2.9/settings/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     5629 2022-10-30 13:38:35.000000 dotscanner-1.2.9/settings/config.py
+-rw-r--r--   0 holly      (501) staff       (20)    10355 2022-10-30 13:38:26.000000 dotscanner-1.2.9/settings/configmanagement.py
+-rw-r--r--   0 holly      (501) staff       (20)       38 2022-10-30 13:50:51.899916 dotscanner-1.2.9/setup.cfg
+-rw-r--r--   0 holly      (501) staff       (20)     1460 2022-10-30 11:35:44.000000 dotscanner-1.2.9/setup.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2022-10-30 13:50:51.899166 dotscanner-1.2.9/tests/
+-rw-r--r--   0 holly      (501) staff       (20)      554 2022-10-30 11:35:44.000000 dotscanner-1.2.9/tests/FakeUserSettings.py
+-rw-r--r--   0 holly      (501) staff       (20)        0 2022-10-30 11:35:44.000000 dotscanner-1.2.9/tests/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     3857 2022-10-30 12:55:59.000000 dotscanner-1.2.9/tests/test_MicroscopeImage.py
+-rw-r--r--   0 holly      (501) staff       (20)     5098 2022-10-30 11:35:44.000000 dotscanner-1.2.9/tests/test_dataprocessing.py
+-rw-r--r--   0 holly      (501) staff       (20)     1690 2022-10-30 11:35:44.000000 dotscanner-1.2.9/tests/test_density.py
+-rw-r--r--   0 holly      (501) staff       (20)     4802 2022-10-30 11:35:44.000000 dotscanner-1.2.9/tests/test_files.py
+-rw-r--r--   0 holly      (501) staff       (20)     9963 2022-10-30 11:35:44.000000 dotscanner-1.2.9/tests/test_lifetime.py
+-rw-r--r--   0 holly      (501) staff       (20)     2155 2022-10-30 11:35:44.000000 dotscanner-1.2.9/tests/test_strings.py
```

### Comparing `dotscanner-1.2.8/PKG-INFO` & `dotscanner-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotscanner
-Version: 1.2.8
+Version: 1.2.9
 Summary: A program designed for analysis of microscope imaging data
 Home-page: https://github.com/bdavis222/dotscanner
 Author: Holly Allen and Brian Davis
 Author-email: holly.allen@colorado.edu
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bdavis222/dotscanner/issues
 Project-URL: Funding, https://www.paypal.com/donate/?business=UA5NL9MJSFMVY
@@ -84,15 +84,15 @@
         #### Skips allowed
         This sets the number of consecutive images that are allowed to be skipped in a lifetime calculation. This can be useful for dimmer dots where an image or two in a series are relatively out of focus, resulting in an unwanted non-detection for those frames. By increasing the number of skips allowed, these particles will be retained as long as they are back in focus and bright enough for detection in subsequent frames.
               
         #### Remove edge frames
         This dictates whether edge frames should be removed from a lifetime calculation. If a particle is detected in the first frame of an image, for example, it cannot be determined whether the particle existed before the first image was taken, so it might not make sense to include this in a lifetime calculation (and the same may also be true for particles in the last frame). If the number of skips allowed in the lifetime calculation is greater than zero, this will increase how many edge frames are removed from analysis.
         
         #### Edit defaults
-        This opens a new window that allows the user to edit or reset the configuration file directly.
+        This opens a new window that allows the user to edit the default filepath or edit/reset the entire configuration file directly.
         
         Clicking **Next**, or pressing the **return** key on the keyboard, will save the user’s selections and open the Threshold Adjustment Window.
         
         ## The Threshold Adjustment Window
         This window shows the image data with the dots and blobs identified, and features several button groups on the left sidebar:
         ![](https://github.com/bdavis222/dotscanner/blob/main/images/7.png)
         
@@ -110,15 +110,15 @@
         #### Blobs
         These buttons adjust the sensitivity for detecting “blobs” in the image. The user can also press the **right** and **left** arrow keys on the keyboard to make these adjustments.
         
         #### Edit
         This button changes the left button bar view to display some manual threshold adjustment options:
         ![](https://github.com/bdavis222/dotscanner/blob/main/images/8.png)
         
-        *(Once the thresholds are changed by entering new numbers into the text boxes, the* **Done** *button saves the settings and returns the left button bar to the original button configuration.)*
+        *(Once the thresholds are changed by entering new numbers into the text boxes, clicking the* **Done** *button, or pressing the* **return** *key on the keyboard, saves the settings and returns the left button bar to the original button configuration.)*
         
         #### Reset
         This button resets the adjusted thresholds back to the default values.
         
         #### Skip
         This button skips the current image (for example, if the user decides the data quality is not sufficient for measurement). The **escape** key on the keyboard can also be pressed to perform a skip.
         
@@ -134,15 +134,15 @@
         
         Holly Allen (holly.allen@colorado.edu)
         
         Brian Davis
         
         ## Release History
         
-        * 1.2.8
+        * 1.2.9
              * Bug fixes
         * 1.2.0
              * Added options for editing the configuration file
              * Added startup processes to check the configuration file for errors
         * 1.1.0
              * Migrated the remaining portions of the app from a terminal interface to a GUI
         * 1.0.0
```

### Comparing `dotscanner-1.2.8/README.md` & `dotscanner-1.2.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 #### Skips allowed
 This sets the number of consecutive images that are allowed to be skipped in a lifetime calculation. This can be useful for dimmer dots where an image or two in a series are relatively out of focus, resulting in an unwanted non-detection for those frames. By increasing the number of skips allowed, these particles will be retained as long as they are back in focus and bright enough for detection in subsequent frames.
       
 #### Remove edge frames
 This dictates whether edge frames should be removed from a lifetime calculation. If a particle is detected in the first frame of an image, for example, it cannot be determined whether the particle existed before the first image was taken, so it might not make sense to include this in a lifetime calculation (and the same may also be true for particles in the last frame). If the number of skips allowed in the lifetime calculation is greater than zero, this will increase how many edge frames are removed from analysis.
 
 #### Edit defaults
-This opens a new window that allows the user to edit or reset the configuration file directly.
+This opens a new window that allows the user to edit the default filepath or edit/reset the entire configuration file directly.
 
 Clicking **Next**, or pressing the **return** key on the keyboard, will save the user’s selections and open the Threshold Adjustment Window.
 
 ## The Threshold Adjustment Window
 This window shows the image data with the dots and blobs identified, and features several button groups on the left sidebar:
 ![](https://github.com/bdavis222/dotscanner/blob/main/images/7.png)
 
@@ -99,15 +99,15 @@
 #### Blobs
 These buttons adjust the sensitivity for detecting “blobs” in the image. The user can also press the **right** and **left** arrow keys on the keyboard to make these adjustments.
 
 #### Edit
 This button changes the left button bar view to display some manual threshold adjustment options:
 ![](https://github.com/bdavis222/dotscanner/blob/main/images/8.png)
 
-*(Once the thresholds are changed by entering new numbers into the text boxes, the* **Done** *button saves the settings and returns the left button bar to the original button configuration.)*
+*(Once the thresholds are changed by entering new numbers into the text boxes, clicking the* **Done** *button, or pressing the* **return** *key on the keyboard, saves the settings and returns the left button bar to the original button configuration.)*
 
 #### Reset
 This button resets the adjusted thresholds back to the default values.
 
 #### Skip
 This button skips the current image (for example, if the user decides the data quality is not sufficient for measurement). The **escape** key on the keyboard can also be pressed to perform a skip.
 
@@ -123,15 +123,15 @@
 
 Holly Allen (holly.allen@colorado.edu)
 
 Brian Davis
 
 ## Release History
 
-* 1.2.8
+* 1.2.9
      * Bug fixes
 * 1.2.0
      * Added options for editing the configuration file
      * Added startup processes to check the configuration file for errors
 * 1.1.0
      * Migrated the remaining portions of the app from a terminal interface to a GUI
 * 1.0.0
```

### Comparing `dotscanner-1.2.8/dotscanner/__main__.py` & `dotscanner-1.2.9/dotscanner/__main__.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.2.8/dotscanner/dataprocessing.py` & `dotscanner-1.2.9/dotscanner/dataprocessing.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.2.8/dotscanner/density.py` & `dotscanner-1.2.9/dotscanner/density.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.2.8/dotscanner/files.py` & `dotscanner-1.2.9/dotscanner/files.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.2.8/dotscanner/lifetime.py` & `dotscanner-1.2.9/dotscanner/lifetime.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.2.8/dotscanner/strings.py` & `dotscanner-1.2.9/dotscanner/strings.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 lifetimeSingleFileWarning = "WARNING: Lifetimes must be calculated using a directory of images, \
 not a single image."
 
 lowerBlobThreshScaleWarning = "\nWARNING: Lower blob threshold scale set below 1.0, which means \
 blobs can be dimmer than the brightest dots, which shouldn't happen. Setting to 1.0."
 
+maxContrastWarning = "\nWARNING: Max contrast reached. Previous contrast values will be retained."
+
 noFilesException = "No files selected. Check the values of 'FILEPATH' and 'START_IMAGE' in the \
 configurations file."
 
 programNameException = "Invalid program name selected in configurations file."
 
 regionSelectorWindowTitle = "Dot Scanner - Region Selection (click the plot to add polygon \
 vertices)"
```

### Comparing `dotscanner-1.2.8/dotscanner/ui/DefaultUserSettingsEditor.py` & `dotscanner-1.2.9/dotscanner/ui/DefaultUserSettingsEditor.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.2.8/dotscanner/ui/DialogWindow.py` & `dotscanner-1.2.9/dotscanner/ui/DialogWindow.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.2.8/dotscanner/ui/MicroscopeImage.py` & `dotscanner-1.2.9/dotscanner/ui/MicroscopeImage.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,25 +24,24 @@
 		self.data = dp.getData(directory, filename)
 		self.sums = dp.getFullDataSquareSum(self.data)
 		self.dotCoords, self.blobCoords = self.getCoords()
 		
 	def decreaseLowerDotThreshScale(self):
 		value = self.lowerDotThreshScale - cfg.THRESHOLD_DELTA
 		value = round(value, 1)
-		if value < 0:
-			value = 0
 		self.lowerDotThreshScale = value
 		self.updateThresholds()
 		self.dotCoords, self.blobCoords = self.getCoords()
 	
 	def decreaseUpperDotThreshScale(self):
 		value = self.upperDotThreshScale - cfg.THRESHOLD_DELTA
 		value = round(value, 1)
 		if value < self.lowerDotThreshScale:
-			value = self.lowerDotThreshScale
+			print(strings.upperDotThreshScaleWarning)
+			return
 		self.upperDotThreshScale = value
 		self.updateThresholds()
 		self.dotCoords, self.blobCoords = self.getCoords()
 	
 	def getCoords(self):
 		if self.thresholds in self.memoizedCoords:
 			dotCoords, blobCoords = self.memoizedCoords[self.thresholds]
@@ -53,15 +52,16 @@
 			self.memoizedCoords[self.thresholds] = (dotCoords, blobCoords)
 		return dotCoords, blobCoords
 	
 	def increaseLowerDotThreshScale(self):
 		value = self.lowerDotThreshScale + cfg.THRESHOLD_DELTA
 		value = round(value, 1)
 		if value > self.upperDotThreshScale:
-			value = self.upperDotThreshScale
+			print(strings.upperDotThreshScaleWarning)
+			return
 		self.lowerDotThreshScale = value
 		self.updateThresholds()
 		self.dotCoords, self.blobCoords = self.getCoords()
 	
 	def increaseUpperDotThreshScale(self):
 		value = self.upperDotThreshScale + cfg.THRESHOLD_DELTA
 		value = round(value, 1)
```

### Comparing `dotscanner-1.2.8/dotscanner/ui/RegionSelector.py` & `dotscanner-1.2.9/dotscanner/ui/RegionSelector.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.2.8/dotscanner/ui/ThresholdAdjuster.py` & `dotscanner-1.2.9/dotscanner/ui/ThresholdAdjuster.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import dotscanner.dataprocessing as dp
 import dotscanner.strings as strings
 import dotscanner.ui.window as ui
-import settings.config as cfg
 import matplotlib
 matplotlib.use("TkAgg")
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
 import numpy as np
 import tkinter as tk
 
 class ThresholdAdjuster:
@@ -346,25 +345,21 @@
 		
 		self.image.dotCoords, self.image.blobCoords = self.image.getCoords()
 		dp.setScatterData(self.image.dotCoords, self.image.blobCoords, self.dotScatter, 
 							self.blobScatter)
 		self.canvas.draw()
 	
 	def upperContrastDown(self):
-		value = self.userSettings.upperContrast - cfg.CONTRAST_DELTA
-		value = round(value, 1)
-		self.userSettings.upperContrast = value
+		self.userSettings.decreaseUpperContrast()
 		self.dataPlot.set_clim(self.userSettings.lowerContrast, 
 								self.userSettings.upperContrast * np.std(self.data))
 		self.canvas.draw()
 	
 	def upperContrastUp(self):
-		value = self.userSettings.upperContrast + cfg.CONTRAST_DELTA
-		value = round(value, 1)
-		self.userSettings.upperContrast = value
+		self.userSettings.increaseUpperContrast()
 		self.dataPlot.set_clim(self.userSettings.lowerContrast, 
 								self.userSettings.upperContrast * np.std(self.data))
 		self.canvas.draw()
 	
 	def upperDotThresholdScaleDown(self):
 		self.image.decreaseUpperDotThreshScale()
 		self.setThresholdEntries(self.image.thresholds)
```

### Comparing `dotscanner-1.2.8/dotscanner/ui/UserSettings.py` & `dotscanner-1.2.9/dotscanner/ui/UserSettings.py`

 * *Files 5% similar despite different names*

```diff
@@ -187,14 +187,22 @@
 					self.buttonSelectStartingImage.config(text="Browse...", fg="black")
 					self.startImage = ""
 					self.labelWarning.configure(text = strings.fileNumberingWarning)
 		
 		self.window.update()
 		self.window.focus_force()
 	
+	def decreaseUpperContrast(self):
+		value = self.upperContrast - cfg.CONTRAST_DELTA
+		value = round(value, 1)
+		if value <= self.lowerContrast:
+			print(strings.maxContrastWarning)
+			return
+		self.upperContrast = value
+	
 	def done(self):
 		if self.filepath in ["", " ", "/"]:
 			return
 		self.dotSize = int(self.entryDotSize.get())
 		self.blobSize = int(self.entryBlobSize.get())
 		self.lowerDotThresh = round(float(self.entryThreshold1.get()), 1)
 		self.upperDotThresh = round(float(self.entryThreshold2.get()), 1)
@@ -209,14 +217,19 @@
 	
 	def doneWithReturnKey(self, event):        
 		self.done()
 	
 	def editDefaults(self):
 		DefaultUserSettingsEditor(self)
 	
+	def increaseUpperContrast(self):
+		value = self.upperContrast + cfg.CONTRAST_DELTA
+		value = round(value, 1)
+		self.upperContrast = value
+	
 	def quitWithQKey(self, event):
 		quit()
 
 	def setRemoveEdge(self):
 		if self.checkboxRemoveEdgeVar.get():
 			self.removeEdgeFrames = True
 		else:
```

### Comparing `dotscanner-1.2.8/dotscanner/ui/window.py` & `dotscanner-1.2.9/dotscanner/ui/window.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.2.8/dotscanner.egg-info/PKG-INFO` & `dotscanner-1.2.9/dotscanner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotscanner
-Version: 1.2.8
+Version: 1.2.9
 Summary: A program designed for analysis of microscope imaging data
 Home-page: https://github.com/bdavis222/dotscanner
 Author: Holly Allen and Brian Davis
 Author-email: holly.allen@colorado.edu
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bdavis222/dotscanner/issues
 Project-URL: Funding, https://www.paypal.com/donate/?business=UA5NL9MJSFMVY
@@ -84,15 +84,15 @@
         #### Skips allowed
         This sets the number of consecutive images that are allowed to be skipped in a lifetime calculation. This can be useful for dimmer dots where an image or two in a series are relatively out of focus, resulting in an unwanted non-detection for those frames. By increasing the number of skips allowed, these particles will be retained as long as they are back in focus and bright enough for detection in subsequent frames.
               
         #### Remove edge frames
         This dictates whether edge frames should be removed from a lifetime calculation. If a particle is detected in the first frame of an image, for example, it cannot be determined whether the particle existed before the first image was taken, so it might not make sense to include this in a lifetime calculation (and the same may also be true for particles in the last frame). If the number of skips allowed in the lifetime calculation is greater than zero, this will increase how many edge frames are removed from analysis.
         
         #### Edit defaults
-        This opens a new window that allows the user to edit or reset the configuration file directly.
+        This opens a new window that allows the user to edit the default filepath or edit/reset the entire configuration file directly.
         
         Clicking **Next**, or pressing the **return** key on the keyboard, will save the user’s selections and open the Threshold Adjustment Window.
         
         ## The Threshold Adjustment Window
         This window shows the image data with the dots and blobs identified, and features several button groups on the left sidebar:
         ![](https://github.com/bdavis222/dotscanner/blob/main/images/7.png)
         
@@ -110,15 +110,15 @@
         #### Blobs
         These buttons adjust the sensitivity for detecting “blobs” in the image. The user can also press the **right** and **left** arrow keys on the keyboard to make these adjustments.
         
         #### Edit
         This button changes the left button bar view to display some manual threshold adjustment options:
         ![](https://github.com/bdavis222/dotscanner/blob/main/images/8.png)
         
-        *(Once the thresholds are changed by entering new numbers into the text boxes, the* **Done** *button saves the settings and returns the left button bar to the original button configuration.)*
+        *(Once the thresholds are changed by entering new numbers into the text boxes, clicking the* **Done** *button, or pressing the* **return** *key on the keyboard, saves the settings and returns the left button bar to the original button configuration.)*
         
         #### Reset
         This button resets the adjusted thresholds back to the default values.
         
         #### Skip
         This button skips the current image (for example, if the user decides the data quality is not sufficient for measurement). The **escape** key on the keyboard can also be pressed to perform a skip.
         
@@ -134,15 +134,15 @@
         
         Holly Allen (holly.allen@colorado.edu)
         
         Brian Davis
         
         ## Release History
         
-        * 1.2.8
+        * 1.2.9
              * Bug fixes
         * 1.2.0
              * Added options for editing the configuration file
              * Added startup processes to check the configuration file for errors
         * 1.1.0
              * Migrated the remaining portions of the app from a terminal interface to a GUI
         * 1.0.0
```

### Comparing `dotscanner-1.2.8/dotscanner.egg-info/SOURCES.txt` & `dotscanner-1.2.9/dotscanner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dotscanner-1.2.8/settings/config.py` & `dotscanner-1.2.9/settings/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,143 +1,125 @@
-# Default selections run by the software (can be changed by the user):
-
-FILEPATH = ""
-# Path to the file or directory of files that should be used. The default value is an empty string: ""
-
-PROGRAM = "density"
-# Whether a "density" program or "lifetime" program should be run
-
-SCALE = None
-# Scale of the image (in nanometers per pixel). If unknown, leave as None.
-
-############################################
-############ THRESHOLD SETTINGS ############
-############################################
-
-LOWER_DOT_THRESH_SCALE = 1.5
-# Scaling for the lower threshold defining the brightness of the dots. The default is 1.5,
-# which corresponds to 1.5 standard deviations above the mean.
-# Lower this value to increase the number of faint dots detected, or raise it to reduce the number.
-
-UPPER_DOT_THRESH_SCALE = 5.0
-# Scaling for the upper threshold defining the brightness of the dots. The default is 5,
-# which corresponds to 5 standard deviations above the mean.
-# Lower this value to reduce the number of bright dots detected, or raise it to increase the number.
-
-LOWER_BLOB_THRESH_SCALE = 2.0
-# Scaling for the lower threshold defining the brightness of the blobs. The default is 2,
-# which corresponds to 2 times the value of UPPER_DOT_THRESH_SCALE.
-# Lower this value to increase the number of blobs detected, or raise it to reduce the number.
-
-THRESHOLD_DELTA = 0.1
-# Amount by which a threshold will change when clicking the up and down arrows in the plotting UI.
-# The default value is 0.1, and will be rounded to the nearest 0.1.
-
-#################################################
-############ IMAGE CONTRAST SETTINGS ############
-#################################################
-
-LOWER_CONTRAST = 0.0
-# The lower bound of the plotting range for the data. The default value is 0.0, or 0 standard
-# deviations above the mean of the dataset. Decrease this value if the image is too dark.
-
-UPPER_CONTRAST = 5.0
-# The upper bound of the plotting range for the data. The default value is 5.0, or 5 standard
-# deviations above the mean of the dataset. Increase this value if the image is too saturated.
-
-CONTRAST_DELTA = 0.5
-# Amount by which the contrast will change when clicking the up and down arrows in the plotting UI.
-# The default value is 0.5, and will be rounded to the nearest 0.1.
-
-###########################################
-############ LIFETIME SETTINGS ############
-###########################################
-
-SKIPS_ALLOWED = 1
-# The number of consecutive images that are allowed to be skipped in a lifetime calculation
-
-REMOVE_EDGE_FRAMES = True
-# Whether edge frames should be removed from a lifetime calculation
-
-LIFETIME_MIN_FOR_PLOT = 1
-# Minimum lifetime to mark a dot in the output figure. The default value is 1, so that all dots
-# with a lifetime of 1 or greater are plotted.
-
-######################################
-############ DOT SETTINGS ############
-######################################
-
-DOT_SIZE = 2
-# Radius of exclusion between other dots (in pixels)
-
-DOT_COLOR = "lime"
-# The color used for dot markers in output plots. 
-# Only use default Python colors (https://matplotlib.org/3.5.0/gallery/color/named_colors.html)
-
-DOT_THICKNESS = 0.5
-# The line thickness used for dots in output plots. Default is 0.5.
-
-#######################################
-############ BLOB SETTINGS ############
-#######################################
-
-BLOB_SIZE = 5
-# Radius of exclusion around blobs (in pixels)
-
-PLOT_BLOBS = False
-# Whether to plot markers on the blobs in outputted figures. Default is False.
-
-BLOB_COLOR = "red"
-# The color used for blob markers in output plots. 
-# Only use default Python colors (https://matplotlib.org/3.5.0/gallery/color/named_colors.html)
-
-BLOB_THICKNESS = 0.5
-# The line thickness used for blobs in output plots. Default is 0.5.
-
-##########################################
-############ POLYGON SETTINGS ############
-##########################################
-
-PLOT_POLYGON = True
-# Whether to plot the polygon in outputted figures. Default is True.
-
-POLYGON_COLOR = "darkorange"
-# The color used for the polygon in output plots. 
-# Only use default Python colors (https://matplotlib.org/3.5.0/gallery/color/named_colors.html)
-
-POLYGON_THICKNESS = 0.5
-# The line thickness used for the polygon in output plots. Default is 0.5.
-
-#########################################
-############ WINDOW SETTINGS ############
-#########################################
-
-DYNAMIC_WINDOW = True
-# Whether the window dynamically scales to the detected screen size.
-
-WINDOW_HEIGHT = 550
-WINDOW_WIDTH = 650
-# Dimensions of “threshold adjustment” and “region selection” windows in pixels.
-# DYNAMIC_WINDOW must be set to False to set these values manually.
-
-WINDOW_X = 10
-WINDOW_Y = 30
-# Starting position of the upper left corner of all GUI windows in pixels
-
-#########################################
-############ OUTPUT SETTINGS ############
-#########################################
-
-SAVE_FIGURES = False
-# Whether the displayed figures should be saved in a "figures" directory. Default is False.
-
-DENSITY_OUTPUT_FILENAME = "densities.txt"
-# The filename to be saved in the directory containing the images used for density measurement.
-# This file will contain the measurements for each of those image files.
-
-LIFETIME_OUTPUT_FILENAME = "lifetimes.txt"
-# The filename to be saved in the directory containing the images used for lifetime measurement.
-
-FIGURE_DIRECTORY_NAME = "figures/"
-# The directory name where figures are to be saved (only if SAVE_FIGURES = True).
-# The default is "figures/", but this can be changed if the user typically keeps a similarly
-# named folder in their file structure for something else.
+# Default selections run by the software (can be changed by the user):
+
+FILEPATH = ""
+# Path to the file or directory of files that should be used. The default value is an empty string: ""
+
+PROGRAM = "density"
+# Whether a "density" program or "lifetime" program should be run
+
+SCALE = None
+# Scale of the image (in nanometers per pixel). If unknown, leave as None.
+
+############################################
+############ THRESHOLD SETTINGS ############
+############################################
+
+LOWER_DOT_THRESH_SCALE = 1.5
+# Scaling for the lower threshold defining the brightness of the dots. The default is 1.5, which corresponds to 1.5 standard deviations above the mean. Lower this value to increase the number of faint dots detected, or raise it to reduce the number.
+
+UPPER_DOT_THRESH_SCALE = 5.0
+# Scaling for the upper threshold defining the brightness of the dots. The default is 5, which corresponds to 5 standard deviations above the mean. Lower this value to reduce the number of bright dots detected, or raise it to increase the number.
+
+LOWER_BLOB_THRESH_SCALE = 2.0
+# Scaling for the lower threshold defining the brightness of the blobs. The default is 2, which corresponds to 2 times the value of UPPER_DOT_THRESH_SCALE. Lower this value to increase the number of blobs detected, or raise it to reduce the number.
+
+THRESHOLD_DELTA = 0.1
+# Amount by which a threshold will change when clicking the up and down arrows in the plotting UI. The default value is 0.1, and will be rounded to the nearest 0.1.
+
+#################################################
+############ IMAGE CONTRAST SETTINGS ############
+#################################################
+
+LOWER_CONTRAST = 0.0
+# The lower bound of the plotting range for the data. The default value is 0.0, or 0 standard deviations above the mean of the dataset. Decrease this value if the image is too dark.
+
+UPPER_CONTRAST = 5.0
+# The upper bound of the plotting range for the data. The default value is 5.0, or 5 standard deviations above the mean of the dataset. Increase this value if the image is too saturated.
+
+CONTRAST_DELTA = 0.5
+# Amount by which the contrast will change when clicking the up and down arrows in the plotting UI. The default value is 0.5, and will be rounded to the nearest 0.1.
+
+###########################################
+############ LIFETIME SETTINGS ############
+###########################################
+
+SKIPS_ALLOWED = 1
+# The number of consecutive images that are allowed to be skipped in a lifetime calculation
+
+REMOVE_EDGE_FRAMES = True
+# Whether edge frames should be removed from a lifetime calculation
+
+LIFETIME_MIN_FOR_PLOT = 1
+# Minimum lifetime to mark a dot in the output figure. The default value is 1, so that all dots with a lifetime of 1 or greater are plotted.
+
+######################################
+############ DOT SETTINGS ############
+######################################
+
+DOT_SIZE = 2
+# Radius of exclusion between other dots (in pixels)
+
+DOT_COLOR = "lime"
+# The color used for dot markers in output plots. Only use default Python colors (https://matplotlib.org/3.5.0/gallery/color/named_colors.html)
+
+DOT_THICKNESS = 0.5
+# The line thickness used for dots in output plots. Default is 0.5.
+
+#######################################
+############ BLOB SETTINGS ############
+#######################################
+
+BLOB_SIZE = 5
+# Radius of exclusion around blobs (in pixels)
+
+PLOT_BLOBS = False
+# Whether to plot markers on the blobs in outputted figures. Default is False.
+
+BLOB_COLOR = "red"
+# The color used for blob markers in output plots. Only use default Python colors (https://matplotlib.org/3.5.0/gallery/color/named_colors.html)
+
+BLOB_THICKNESS = 0.5
+# The line thickness used for blobs in output plots. Default is 0.5.
+
+##########################################
+############ POLYGON SETTINGS ############
+##########################################
+
+PLOT_POLYGON = True
+# Whether to plot the polygon in outputted figures. Default is True.
+
+POLYGON_COLOR = "darkorange"
+# The color used for the polygon in output plots. Only use default Python colors (https://matplotlib.org/3.5.0/gallery/color/named_colors.html)
+
+POLYGON_THICKNESS = 0.5
+# The line thickness used for the polygon in output plots. Default is 0.5.
+
+#########################################
+############ WINDOW SETTINGS ############
+#########################################
+
+DYNAMIC_WINDOW = True
+# Whether the window dynamically scales to the detected screen size.
+
+WINDOW_HEIGHT = 550
+WINDOW_WIDTH = 650
+# Dimensions of “threshold adjustment” and “region selection” windows in pixels. DYNAMIC_WINDOW must be set to False to set these values manually.
+
+WINDOW_X = 10
+WINDOW_Y = 30
+# Starting position of the upper left corner of all GUI windows in pixels
+
+#########################################
+############ OUTPUT SETTINGS ############
+#########################################
+
+SAVE_FIGURES = False
+# Whether the displayed figures should be saved in a "figures" directory. Default is False.
+
+DENSITY_OUTPUT_FILENAME = "densities.txt"
+# The filename to be saved in the directory containing the images used for density measurement. This file will contain the measurements for each of those image files.
+
+LIFETIME_OUTPUT_FILENAME = "lifetimes.txt"
+# The filename to be saved in the directory containing the images used for lifetime measurement.
+
+FIGURE_DIRECTORY_NAME = "figures/"
+# The directory name where figures are to be saved (only if SAVE_FIGURES = True). The default is "figures/", but this can be changed if the user typically keeps a similarly named folder in their file structure for something else.
```

### Comparing `dotscanner-1.2.8/settings/configmanagement.py` & `dotscanner-1.2.9/settings/configmanagement.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,23 +21,28 @@
 	
 	assert type(cfg.FILEPATH) == str
 	assert cfg.PROGRAM in ["density", "lifetime"]
 	assert cfg.SCALE is None or type(cfg.SCALE) in [int, float]
 	
 	assert type(cfg.LOWER_DOT_THRESH_SCALE) in [int, float]
 	assert type(cfg.UPPER_DOT_THRESH_SCALE) in [int, float]
+	assert cfg.LOWER_DOT_THRESH_SCALE <= cfg.UPPER_DOT_THRESH_SCALE
 	assert type(cfg.LOWER_BLOB_THRESH_SCALE) in [int, float]
+	assert cfg.LOWER_BLOB_THRESH_SCALE >= 1
 	assert type(cfg.THRESHOLD_DELTA) in [int, float]
 	
 	assert type(cfg.LOWER_CONTRAST) in [int, float]
 	assert type(cfg.UPPER_CONTRAST) in [int, float]
+	assert cfg.LOWER_CONTRAST < cfg.UPPER_CONTRAST
 	assert type(cfg.CONTRAST_DELTA) in [int, float]
 	
 	assert type(cfg.SKIPS_ALLOWED) == int
+	assert cfg.SKIPS_ALLOWED >= 0
 	assert type(cfg.REMOVE_EDGE_FRAMES) == bool
+	assert type(cfg.LIFETIME_MIN_FOR_PLOT) == int
 	
 	assert type(cfg.DOT_SIZE) == int
 	assert cfg.DOT_COLOR in matplotlibColors
 	assert type(cfg.DOT_THICKNESS) in [int, float]
 	
 	assert type(cfg.BLOB_SIZE) == int
 	assert type(cfg.PLOT_BLOBS) == bool
@@ -144,72 +149,60 @@
 # Scale of the image (in nanometers per pixel). If unknown, leave as None.\n\
 \n\
 ############################################\n\
 ############ THRESHOLD SETTINGS ############\n\
 ############################################\n\
 \n\
 LOWER_DOT_THRESH_SCALE = 1.5\n\
-# Scaling for the lower threshold defining the brightness of the dots. The default is 1.5,\n\
-# which corresponds to 1.5 standard deviations above the mean.\n\
-# Lower this value to increase the number of faint dots detected, or raise it to reduce the number.\n\
+# Scaling for the lower threshold defining the brightness of the dots. The default is 1.5, which corresponds to 1.5 standard deviations above the mean. Lower this value to increase the number of faint dots detected, or raise it to reduce the number.\n\
 \n\
 UPPER_DOT_THRESH_SCALE = 5.0\n\
-# Scaling for the upper threshold defining the brightness of the dots. The default is 5,\n\
-# which corresponds to 5 standard deviations above the mean.\n\
-# Lower this value to reduce the number of bright dots detected, or raise it to increase the number.\n\
+# Scaling for the upper threshold defining the brightness of the dots. The default is 5, which corresponds to 5 standard deviations above the mean. Lower this value to reduce the number of bright dots detected, or raise it to increase the number.\n\
 \n\
 LOWER_BLOB_THRESH_SCALE = 2.0\n\
-# Scaling for the lower threshold defining the brightness of the blobs. The default is 2,\n\
-# which corresponds to 2 times the value of UPPER_DOT_THRESH_SCALE.\n\
-# Lower this value to increase the number of blobs detected, or raise it to reduce the number.\n\
+# Scaling for the lower threshold defining the brightness of the blobs. The default is 2, which corresponds to 2 times the value of UPPER_DOT_THRESH_SCALE. Lower this value to increase the number of blobs detected, or raise it to reduce the number.\n\
 \n\
 THRESHOLD_DELTA = 0.1\n\
-# Amount by which a threshold will change when clicking the up and down arrows in the plotting UI.\n\
-# The default value is 0.1, and will be rounded to the nearest 0.1.\n\
+# Amount by which a threshold will change when clicking the up and down arrows in the plotting UI. The default value is 0.1, and will be rounded to the nearest 0.1.\n\
 \n\
 #################################################\n\
 ############ IMAGE CONTRAST SETTINGS ############\n\
 #################################################\n\
 \n\
 LOWER_CONTRAST = 0.0\n\
-# The lower bound of the plotting range for the data. The default value is 0.0, or 0 standard\n\
-# deviations above the mean of the dataset. Decrease this value if the image is too dark.\n\
+# The lower bound of the plotting range for the data. The default value is 0.0, or 0 standard deviations above the mean of the dataset. Decrease this value if the image is too dark.\n\
 \n\
 UPPER_CONTRAST = 5.0\n\
-# The upper bound of the plotting range for the data. The default value is 5.0, or 5 standard\n\
-# deviations above the mean of the dataset. Increase this value if the image is too saturated.\n\
+# The upper bound of the plotting range for the data. The default value is 5.0, or 5 standard deviations above the mean of the dataset. Increase this value if the image is too saturated.\n\
 \n\
 CONTRAST_DELTA = 0.5\n\
-# Amount by which the contrast will change when clicking the up and down arrows in the plotting UI.\n\
-# The default value is 0.5, and will be rounded to the nearest 0.1.\n\
+# Amount by which the contrast will change when clicking the up and down arrows in the plotting UI. The default value is 0.5, and will be rounded to the nearest 0.1.\n\
 \n\
 ###########################################\n\
 ############ LIFETIME SETTINGS ############\n\
 ###########################################\n\
 \n\
 SKIPS_ALLOWED = 1\n\
 # The number of consecutive images that are allowed to be skipped in a lifetime calculation\n\
 \n\
 REMOVE_EDGE_FRAMES = True\n\
 # Whether edge frames should be removed from a lifetime calculation\n\
 \n\
 LIFETIME_MIN_FOR_PLOT = 1\n\
-# Minimum lifetime to mark a dot in the output figure. The default value is 1, so that all dots\n\
-# with a lifetime of 1 or greater are plotted.\n\
+# Minimum lifetime to mark a dot in the output figure. The default value is 1, so that all dots with a lifetime of 1 or greater are plotted.\n\
 \n\
 ######################################\n\
 ############ DOT SETTINGS ############\n\
 ######################################\n\
 \n\
 DOT_SIZE = 2\n\
 # Radius of exclusion between other dots (in pixels)\n\
 \n\
 DOT_COLOR = "lime"\n\
-# The color used for dot markers in output plots. \n\
-# Only use default Python colors (https://matplotlib.org/3.5.0/gallery/color/named_colors.html)\n\
+# The color used for dot markers in output plots. Only use default Python colors (https://matplotlib.org/3.5.0/gallery/color/named_colors.html)\n\
 \n\
 DOT_THICKNESS = 0.5\n\
 # The line thickness used for dots in output plots. Default is 0.5.\n\
 \n\
 #######################################\n\
 ############ BLOB SETTINGS ############\n\
 #######################################\n\
@@ -217,64 +210,58 @@
 BLOB_SIZE = 5\n\
 # Radius of exclusion around blobs (in pixels)\n\
 \n\
 PLOT_BLOBS = False\n\
 # Whether to plot markers on the blobs in outputted figures. Default is False.\n\
 \n\
 BLOB_COLOR = "red"\n\
-# The color used for blob markers in output plots. \n\
-# Only use default Python colors (https://matplotlib.org/3.5.0/gallery/color/named_colors.html)\n\
+# The color used for blob markers in output plots. Only use default Python colors (https://matplotlib.org/3.5.0/gallery/color/named_colors.html)\n\
 \n\
 BLOB_THICKNESS = 0.5\n\
 # The line thickness used for blobs in output plots. Default is 0.5.\n\
 \n\
 ##########################################\n\
 ############ POLYGON SETTINGS ############\n\
 ##########################################\n\
 \n\
 PLOT_POLYGON = True\n\
 # Whether to plot the polygon in outputted figures. Default is True.\n\
 \n\
 POLYGON_COLOR = "darkorange"\n\
-# The color used for the polygon in output plots. \n\
-# Only use default Python colors (https://matplotlib.org/3.5.0/gallery/color/named_colors.html)\n\
+# The color used for the polygon in output plots. Only use default Python colors (https://matplotlib.org/3.5.0/gallery/color/named_colors.html)\n\
 \n\
 POLYGON_THICKNESS = 0.5\n\
 # The line thickness used for the polygon in output plots. Default is 0.5.\n\
 \n\
 #########################################\n\
 ############ WINDOW SETTINGS ############\n\
 #########################################\n\
 \n\
 DYNAMIC_WINDOW = True\n\
 # Whether the window dynamically scales to the detected screen size.\n\
 \n\
 WINDOW_HEIGHT = 550\n\
 WINDOW_WIDTH = 650\n\
-# Dimensions of “threshold adjustment” and “region selection” windows in pixels.\n\
-# DYNAMIC_WINDOW must be set to False to set these values manually.\n\
+# Dimensions of “threshold adjustment” and “region selection” windows in pixels. DYNAMIC_WINDOW must be set to False to set these values manually.\n\
 \n\
 WINDOW_X = 10\n\
 WINDOW_Y = 30\n\
 # Starting position of the upper left corner of all GUI windows in pixels\n\
 \n\
 #########################################\n\
 ############ OUTPUT SETTINGS ############\n\
 #########################################\n\
 \n\
 SAVE_FIGURES = False\n\
 # Whether the displayed figures should be saved in a "figures" directory. Default is False.\n\
 \n\
 DENSITY_OUTPUT_FILENAME = "densities.txt"\n\
-# The filename to be saved in the directory containing the images used for density measurement.\n\
-# This file will contain the measurements for each of those image files.\n\
+# The filename to be saved in the directory containing the images used for density measurement. This file will contain the measurements for each of those image files.\n\
 \n\
 LIFETIME_OUTPUT_FILENAME = "lifetimes.txt"\n\
 # The filename to be saved in the directory containing the images used for lifetime measurement.\n\
 \n\
 FIGURE_DIRECTORY_NAME = "figures/"\n\
-# The directory name where figures are to be saved (only if SAVE_FIGURES = True).\n\
-# The default is "figures/", but this can be changed if the user typically keeps a similarly\n\
-# named folder in their file structure for something else.\
+# The directory name where figures are to be saved (only if SAVE_FIGURES = True). The default is "figures/", but this can be changed if the user typically keeps a similarly named folder in their file structure for something else.\
 ')
 	
 	quit()
```

### Comparing `dotscanner-1.2.8/tests/FakeUserSettings.py` & `dotscanner-1.2.9/tests/FakeUserSettings.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.2.8/tests/test_MicroscopeImage.py` & `dotscanner-1.2.9/tests/test_MicroscopeImage.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,50 +36,54 @@
 		self.assertEqual(microscopeImage.removeEdgeFrames, True)
 		self.assertEqual(microscopeImage.thresholds, (1.5, 5.0, 2.0))
 		self.assertIn(3, microscopeImage.dotCoords)
 		self.assertIn(1, microscopeImage.dotCoords[3])
 		self.assertEqual(microscopeImage.blobCoords, {})
 	
 	@mock.patch('settings.config.THRESHOLD_DELTA', 0.1)
+	@mock.patch('settings.config.LOWER_DOT_THRESH_SCALE', 1.5)
 	def test_decreaseLowerDotThreshScale(self):
 		microscopeImage = self.getMicroscopeImage()
 		
 		microscopeImage.decreaseLowerDotThreshScale()
 		
 		self.assertEqual(microscopeImage.lowerDotThreshScale, 1.4)
 		
 		microscopeImage.decreaseLowerDotThreshScale()
 		
 		self.assertEqual(microscopeImage.lowerDotThreshScale, 1.3)
 	
 	@mock.patch('settings.config.THRESHOLD_DELTA', 0.1)
+	@mock.patch('settings.config.LOWER_DOT_THRESH_SCALE', 1.5)
 	def test_increaseLowerDotThreshScale(self):
 		microscopeImage = self.getMicroscopeImage()
 		
 		microscopeImage.increaseLowerDotThreshScale()
 		
 		self.assertEqual(microscopeImage.lowerDotThreshScale, 1.6)
 		
 		microscopeImage.increaseLowerDotThreshScale()
 		
 		self.assertEqual(microscopeImage.lowerDotThreshScale, 1.7)
 	
 	@mock.patch('settings.config.THRESHOLD_DELTA', 0.1)
+	@mock.patch('settings.config.UPPER_DOT_THRESH_SCALE', 5.0)
 	def test_decreaseUpperDotThreshScale(self):
 		microscopeImage = self.getMicroscopeImage()
 		
 		microscopeImage.decreaseUpperDotThreshScale()
 		
 		self.assertEqual(microscopeImage.upperDotThreshScale, 4.9)
 		
 		microscopeImage.decreaseUpperDotThreshScale()
 		
 		self.assertEqual(microscopeImage.upperDotThreshScale, 4.8)
 	
 	@mock.patch('settings.config.THRESHOLD_DELTA', 0.1)
+	@mock.patch('settings.config.UPPER_DOT_THRESH_SCALE', 5.0)
 	def test_increaseUpperDotThreshScale(self):
 		microscopeImage = self.getMicroscopeImage()
 		
 		microscopeImage.increaseUpperDotThreshScale()
 		
 		self.assertEqual(microscopeImage.upperDotThreshScale, 5.1)
```

### Comparing `dotscanner-1.2.8/tests/test_dataprocessing.py` & `dotscanner-1.2.9/tests/test_dataprocessing.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.2.8/tests/test_density.py` & `dotscanner-1.2.9/tests/test_density.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.2.8/tests/test_files.py` & `dotscanner-1.2.9/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.2.8/tests/test_lifetime.py` & `dotscanner-1.2.9/tests/test_lifetime.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.2.8/tests/test_strings.py` & `dotscanner-1.2.9/tests/test_strings.py`

 * *Files identical despite different names*

