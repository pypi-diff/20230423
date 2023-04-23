# Comparing `tmp/media_manager-0.8.0-py2.py3-none-any.whl.zip` & `tmp/media_manager-0.9.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 7303 bytes, number of entries: 9
+Zip file size: 7310 bytes, number of entries: 9
 -rw-r--r--  2.0 unx      310 b- defN 23-Feb-07 03:23 media_manager/__init__.py
--rw-r--r--  2.0 unx    18685 b- defN 23-Feb-07 06:41 media_manager/media_manager.py
--rw-r--r--  2.0 unx      116 b- defN 23-Feb-07 06:41 media_manager/version.py
--rw-r--r--  2.0 unx     1210 b- defN 23-Feb-07 06:41 media_manager-0.8.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2293 b- defN 23-Feb-07 06:41 media_manager-0.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Feb-07 06:41 media_manager-0.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       68 b- defN 23-Feb-07 06:41 media_manager-0.8.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       14 b- defN 23-Feb-07 06:41 media_manager-0.8.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      767 b- defN 23-Feb-07 06:41 media_manager-0.8.0.dist-info/RECORD
-9 files, 23573 bytes uncompressed, 5969 bytes compressed:  74.7%
+-rw-r--r--  2.0 unx    18728 b- defN 23-Feb-07 06:48 media_manager/media_manager.py
+-rw-r--r--  2.0 unx      116 b- defN 23-Feb-07 06:48 media_manager/version.py
+-rw-r--r--  2.0 unx     1210 b- defN 23-Feb-07 06:48 media_manager-0.9.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2293 b- defN 23-Feb-07 06:48 media_manager-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Feb-07 06:48 media_manager-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       68 b- defN 23-Feb-07 06:48 media_manager-0.9.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 23-Feb-07 06:48 media_manager-0.9.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      767 b- defN 23-Feb-07 06:48 media_manager-0.9.0.dist-info/RECORD
+9 files, 23616 bytes uncompressed, 5976 bytes compressed:  74.7%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: media_manager/media_manager.py
 Comment: 
 
 Filename: media_manager/version.py
 Comment: 
 
-Filename: media_manager-0.8.0.dist-info/LICENSE
+Filename: media_manager-0.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: media_manager-0.8.0.dist-info/METADATA
+Filename: media_manager-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: media_manager-0.8.0.dist-info/WHEEL
+Filename: media_manager-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: media_manager-0.8.0.dist-info/entry_points.txt
+Filename: media_manager-0.9.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: media_manager-0.8.0.dist-info/top_level.txt
+Filename: media_manager-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: media_manager-0.8.0.dist-info/RECORD
+Filename: media_manager-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## media_manager/media_manager.py

```diff
@@ -299,15 +299,15 @@
         self.file_extension = ""
         self.media_files = []
         self.media_file_directories = []
 
     # Iterate through all media files found
     def clean_media(self):
         while self.media_file_index < len(self.media_files):
-            print(f"Validating ({self.media_file_index+1}/{len(self.media_files)}): {self.media_files[self.media_file_index]}\n\n")
+            print(f"Validating ({self.media_file_index+1}/{len(self.media_files)}): {self.media_files[self.media_file_index]}\n")
             self.directory = os.path.dirname(self.media_files[self.media_file_index])
             self.media_file = os.path.basename(self.media_files[self.media_file_index])
             self.file_name, self.file_extension = os.path.splitext(self.media_file)
             self.new_file_name = self.file_name
             self.media_detection()
             self.clean_file_name()
             self.verify_parent_directory()
@@ -318,15 +318,15 @@
         self.reset_variables()
 
     # Move media to new destination
     def move_media(self, target_directory: str, type="media"):   
         if not os.path.isdir(target_directory):
             print(f"Directory {target_directory} does not exist")
             return
-        
+        print(f"Moving {type} to {target_directory}")
         self.find_media()               
         for media_directory_index in range(0, len(self.media_file_directories)):
             # Find if file inside this directory is named as a series
             move = False
             files = glob.glob(f"{self.media_file_directories[media_directory_index]}/*", recursive=True)
             for file in files:
                 move = False
```

## media_manager/version.py

```diff
@@ -1,6 +1,6 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 __author__ = 'Audel Rouhi'
 __credits__ = 'Audel Rouhi'
```

## Comparing `media_manager-0.8.0.dist-info/LICENSE` & `media_manager-0.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `media_manager-0.8.0.dist-info/METADATA` & `media_manager-0.9.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: media-manager
-Version: 0.8.0
+Version: 0.9.0
 Summary: Manage your media!
 Home-page: https://github.com/Knuckles-Team/media-manager
 Author: Audel Rouhi
 Author-email: knucklessg1@gmail.com
 License: Unlicense
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ffmpeg-python (>=0.2.0)
 
 # Media Manager
-*Version: 0.8.0*
+*Version: 0.9.0*
 
 Manage your media
 - Automatically clean file names 
 - Set Title and Comment metadata to match filename
 - Apply subtitles in media's "Sub" directory automatically
 - Move media to desired destination
```

## Comparing `media_manager-0.8.0.dist-info/RECORD` & `media_manager-0.9.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 media_manager/__init__.py,sha256=IMuj1fFl0p6HrPEyDCtWwWFQOURx1KmO57kHZ3UN3f4,310
-media_manager/media_manager.py,sha256=TrXjRH7OgPAI-igi1Mvki0DCOsiGoL5t22DfnxexRUY,18685
-media_manager/version.py,sha256=tDDkCMChiJvcYngqfjlW_EaRz0JpbXA3z7tYvqWYe8M,116
-media_manager-0.8.0.dist-info/LICENSE,sha256=yiq99pWITHfqS0pbZMp7cy2dnbreTuvBwudsU-njvIM,1210
-media_manager-0.8.0.dist-info/METADATA,sha256=UQnPqbJQiC7UEDBoQxRhGjgcopjv_8bebeEiwHmKCno,2293
-media_manager-0.8.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-media_manager-0.8.0.dist-info/entry_points.txt,sha256=Mop8uN2V808fwZvAR5gfhUXx8VP0Hk7MCGsApn-n63c,68
-media_manager-0.8.0.dist-info/top_level.txt,sha256=VWivzu4oIY90-Ii-ffwrpRPLKsh3lOAtKXirt3jHtVY,14
-media_manager-0.8.0.dist-info/RECORD,,
+media_manager/media_manager.py,sha256=tVLrgWglWimYi1z3puoj4XucJswcKiBrjpX874DoKzU,18728
+media_manager/version.py,sha256=swhRnSKFIqDu9_CTMLtKcx393Adi5vpxEYYazFr8kkE,116
+media_manager-0.9.0.dist-info/LICENSE,sha256=yiq99pWITHfqS0pbZMp7cy2dnbreTuvBwudsU-njvIM,1210
+media_manager-0.9.0.dist-info/METADATA,sha256=oOQhXqiKSbEyORBjoDFTLwqtLFXF-uVe2tb0qMyLJSw,2293
+media_manager-0.9.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+media_manager-0.9.0.dist-info/entry_points.txt,sha256=Mop8uN2V808fwZvAR5gfhUXx8VP0Hk7MCGsApn-n63c,68
+media_manager-0.9.0.dist-info/top_level.txt,sha256=VWivzu4oIY90-Ii-ffwrpRPLKsh3lOAtKXirt3jHtVY,14
+media_manager-0.9.0.dist-info/RECORD,,
```

