# Comparing `tmp/cv2_collage_v2-0.10.tar.gz` & `tmp/cv2_collage_v2-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cv2_collage_v2-0.10.tar", last modified: Sun Apr 23 12:04:34 2023, max compression
+gzip compressed data, was "cv2_collage_v2-0.11.tar", last modified: Sun Apr 23 12:05:40 2023, max compression
```

## Comparing `cv2_collage_v2-0.10.tar` & `cv2_collage_v2-0.11.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 12:04:34.350990 cv2_collage_v2-0.10/
--rw-rw-rw-   0        0        0     1148 2023-04-23 12:04:24.000000 cv2_collage_v2-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      145 2023-04-23 12:04:23.000000 cv2_collage_v2-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     2022 2023-04-23 12:04:34.351987 cv2_collage_v2-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     1404 2023-04-23 12:03:24.000000 cv2_collage_v2-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 12:04:34.346001 cv2_collage_v2-0.10/cv2_collage_v2/
--rw-rw-rw-   0        0        0     1148 2023-04-15 00:23:59.000000 cv2_collage_v2-0.10/cv2_collage_v2/LICENSE
--rw-rw-rw-   0        0        0     1404 2023-04-23 12:03:24.000000 cv2_collage_v2-0.10/cv2_collage_v2/README.md
--rw-rw-rw-   0        0        0     2929 2023-04-23 12:02:21.000000 cv2_collage_v2-0.10/cv2_collage_v2/__init__.py
--rw-rw-rw-   0        0        0      103 2023-04-23 12:04:33.000000 cv2_collage_v2-0.10/cv2_collage_v2/requirements.txt
--rw-rw-rw-   0        0        0    49102 2023-04-23 12:04:33.000000 cv2_collage_v2-0.10/cv2_collage_v2/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-04-23 12:04:34.350990 cv2_collage_v2-0.10/cv2_collage_v2.egg-info/
--rw-rw-rw-   0        0        0     2022 2023-04-23 12:04:34.000000 cv2_collage_v2-0.10/cv2_collage_v2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      379 2023-04-23 12:04:34.000000 cv2_collage_v2-0.10/cv2_collage_v2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 12:04:34.000000 cv2_collage_v2-0.10/cv2_collage_v2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2023-04-23 12:04:34.000000 cv2_collage_v2-0.10/cv2_collage_v2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-23 12:04:34.000000 cv2_collage_v2-0.10/cv2_collage_v2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-04-23 12:04:34.351987 cv2_collage_v2-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1504 2023-04-23 12:04:33.000000 cv2_collage_v2-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 12:05:40.615054 cv2_collage_v2-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-04-23 12:05:30.000000 cv2_collage_v2-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      145 2023-04-23 12:05:29.000000 cv2_collage_v2-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     2019 2023-04-23 12:05:40.615054 cv2_collage_v2-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     1401 2023-04-23 12:05:18.000000 cv2_collage_v2-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 12:05:40.611065 cv2_collage_v2-0.11/cv2_collage_v2/
+-rw-rw-rw-   0        0        0     1148 2023-04-15 00:23:59.000000 cv2_collage_v2-0.11/cv2_collage_v2/LICENSE
+-rw-rw-rw-   0        0        0     1401 2023-04-23 12:05:18.000000 cv2_collage_v2-0.11/cv2_collage_v2/README.md
+-rw-rw-rw-   0        0        0     2929 2023-04-23 12:02:21.000000 cv2_collage_v2-0.11/cv2_collage_v2/__init__.py
+-rw-rw-rw-   0        0        0      103 2023-04-23 12:05:39.000000 cv2_collage_v2-0.11/cv2_collage_v2/requirements.txt
+-rw-rw-rw-   0        0        0    49102 2023-04-23 12:05:39.000000 cv2_collage_v2-0.11/cv2_collage_v2/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-04-23 12:05:40.614057 cv2_collage_v2-0.11/cv2_collage_v2.egg-info/
+-rw-rw-rw-   0        0        0     2019 2023-04-23 12:05:40.000000 cv2_collage_v2-0.11/cv2_collage_v2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2023-04-23 12:05:40.000000 cv2_collage_v2-0.11/cv2_collage_v2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 12:05:40.000000 cv2_collage_v2-0.11/cv2_collage_v2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2023-04-23 12:05:40.000000 cv2_collage_v2-0.11/cv2_collage_v2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-23 12:05:40.000000 cv2_collage_v2-0.11/cv2_collage_v2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-04-23 12:05:40.616052 cv2_collage_v2-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1504 2023-04-23 12:05:39.000000 cv2_collage_v2-0.11/setup.py
```

### Comparing `cv2_collage_v2-0.10/LICENSE.rst` & `cv2_collage_v2-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `cv2_collage_v2-0.10/PKG-INFO` & `cv2_collage_v2-0.11/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cv2_collage_v2
-Version: 0.10
+Version: 0.11
 Summary: Creates a collage from images with OpenCV
 Home-page: https://github.com/hansalemaos/cv2_collage_v2
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: collage,opencv
 Classifier: Development Status :: 4 - Beta
@@ -13,15 +13,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
 # Creates a collage from images with OpenCV
 
-## pip install create-collage-v2 
+## pip install cv2-collage-v2 
 
 # Tested against Windows 10 / Python 3.10 / Anaconda
 
 ## How to use it
 
 ```python
 from cv2_collage_v2 import create_collage_v2
```

### Comparing `cv2_collage_v2-0.10/README.md` & `cv2_collage_v2-0.11/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Creates a collage from images with OpenCV
 
-## pip install create-collage-v2 
+## pip install cv2-collage-v2 
 
 # Tested against Windows 10 / Python 3.10 / Anaconda
 
 ## How to use it
 
 ```python
 from cv2_collage_v2 import create_collage_v2
```

### Comparing `cv2_collage_v2-0.10/cv2_collage_v2/LICENSE` & `cv2_collage_v2-0.11/cv2_collage_v2/LICENSE`

 * *Files identical despite different names*

### Comparing `cv2_collage_v2-0.10/cv2_collage_v2/README.md` & `cv2_collage_v2-0.11/cv2_collage_v2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Creates a collage from images with OpenCV
 
-## pip install create-collage-v2 
+## pip install cv2-collage-v2 
 
 # Tested against Windows 10 / Python 3.10 / Anaconda
 
 ## How to use it
 
 ```python
 from cv2_collage_v2 import create_collage_v2
```

### Comparing `cv2_collage_v2-0.10/cv2_collage_v2/__init__.py` & `cv2_collage_v2-0.11/cv2_collage_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `cv2_collage_v2-0.10/cv2_collage_v2/thirdparty.json` & `cv2_collage_v2-0.11/cv2_collage_v2/thirdparty.json`

 * *Files identical despite different names*

### Comparing `cv2_collage_v2-0.10/cv2_collage_v2.egg-info/PKG-INFO` & `cv2_collage_v2-0.11/cv2_collage_v2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cv2-collage-v2
-Version: 0.10
+Version: 0.11
 Summary: Creates a collage from images with OpenCV
 Home-page: https://github.com/hansalemaos/cv2_collage_v2
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: collage,opencv
 Classifier: Development Status :: 4 - Beta
@@ -13,15 +13,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
 # Creates a collage from images with OpenCV
 
-## pip install create-collage-v2 
+## pip install cv2-collage-v2 
 
 # Tested against Windows 10 / Python 3.10 / Anaconda
 
 ## How to use it
 
 ```python
 from cv2_collage_v2 import create_collage_v2
```

### Comparing `cv2_collage_v2-0.10/setup.py` & `cv2_collage_v2-0.11/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
+VERSION = '''0.11'''
 DESCRIPTION = '''Creates a collage from images with OpenCV'''
 
 # Setting up
 setup(
     name="cv2_collage_v2",
     version=VERSION,
     license='MIT',
```

