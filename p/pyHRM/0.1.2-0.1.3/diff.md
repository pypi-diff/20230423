# Comparing `tmp/pyHRM-0.1.2.tar.gz` & `tmp/pyHRM-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyHRM-0.1.2.tar", last modified: Sun Apr 23 05:16:07 2023, max compression
+gzip compressed data, was "pyHRM-0.1.3.tar", last modified: Sun Apr 23 05:19:45 2023, max compression
```

## Comparing `pyHRM-0.1.2.tar` & `pyHRM-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 05:16:07.892145 pyHRM-0.1.2/
--rw-rw-rw-   0        0        0     1087 2023-04-22 11:02:58.000000 pyHRM-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0      703 2023-04-23 05:16:07.876521 pyHRM-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-04-22 11:00:11.000000 pyHRM-0.1.2/README.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 05:16:07.892145 pyHRM-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1241 2023-04-23 05:15:49.000000 pyHRM-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-23 05:16:07.860886 pyHRM-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-23 05:16:07.860886 pyHRM-0.1.2/src/pyHRM/
--rw-rw-rw-   0        0        0   240704 2023-04-22 10:50:41.000000 pyHRM-0.1.2/src/pyHRM/Melt2_0.h5
--rw-rw-rw-   0        0        0        0 2023-04-22 10:50:41.000000 pyHRM-0.1.2/src/pyHRM/__init__.py
--rw-rw-rw-   0        0        0    21670 2023-04-23 05:14:59.000000 pyHRM-0.1.2/src/pyHRM/melt.py
-drwxrwxrwx   0        0        0        0 2023-04-23 05:16:07.876521 pyHRM-0.1.2/src/pyHRM.egg-info/
--rw-rw-rw-   0        0        0      703 2023-04-23 05:16:07.000000 pyHRM-0.1.2/src/pyHRM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-04-23 05:16:07.000000 pyHRM-0.1.2/src/pyHRM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 05:16:07.000000 pyHRM-0.1.2/src/pyHRM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      216 2023-04-23 05:16:07.000000 pyHRM-0.1.2/src/pyHRM.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-23 05:16:07.000000 pyHRM-0.1.2/src/pyHRM.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 05:19:45.982238 pyHRM-0.1.3/
+-rw-rw-rw-   0        0        0     1087 2023-04-22 11:02:58.000000 pyHRM-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      703 2023-04-23 05:19:45.982238 pyHRM-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-04-22 11:00:11.000000 pyHRM-0.1.3/README.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 05:19:45.982238 pyHRM-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1271 2023-04-23 05:19:36.000000 pyHRM-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 05:19:45.955932 pyHRM-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-23 05:19:45.963441 pyHRM-0.1.3/src/pyHRM/
+-rw-rw-rw-   0        0        0   240704 2023-04-22 10:50:41.000000 pyHRM-0.1.3/src/pyHRM/Melt2_0.h5
+-rw-rw-rw-   0        0        0        0 2023-04-22 10:50:41.000000 pyHRM-0.1.3/src/pyHRM/__init__.py
+-rw-rw-rw-   0        0        0    21670 2023-04-23 05:14:59.000000 pyHRM-0.1.3/src/pyHRM/melt.py
+drwxrwxrwx   0        0        0        0 2023-04-23 05:19:45.982238 pyHRM-0.1.3/src/pyHRM.egg-info/
+-rw-rw-rw-   0        0        0      703 2023-04-23 05:19:45.000000 pyHRM-0.1.3/src/pyHRM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2023-04-23 05:19:45.000000 pyHRM-0.1.3/src/pyHRM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 05:19:45.000000 pyHRM-0.1.3/src/pyHRM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      216 2023-04-23 05:19:45.000000 pyHRM-0.1.3/src/pyHRM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-23 05:19:45.000000 pyHRM-0.1.3/src/pyHRM.egg-info/top_level.txt
```

### Comparing `pyHRM-0.1.2/LICENSE.txt` & `pyHRM-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyHRM-0.1.2/PKG-INFO` & `pyHRM-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyHRM
-Version: 0.1.2
+Version: 0.1.3
 Summary: A novel library for processing DNA Melting signal with feature extraction and thresholding.
 Home-page: 
 Author: RajagopalS
 Author-email: rajag2001416@gmail.com
 Maintainer: ['RajagopalS rajag2001416@gmail.com', 'Vignesh_R mail2vikivignesh06@gmail.com', 'SenthilKumarN senthilkumarnallendran@gmail.com']
 License: MIT
 Keywords: HRM,Melt,PCR
```

### Comparing `pyHRM-0.1.2/setup.py` & `pyHRM-0.1.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,26 +6,27 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='pyHRM',
-  version='0.1.2',
+  version='0.1.3',
   description='A novel library for processing DNA Melting signal with feature extraction and thresholding.',
   url='',  
   author='RajagopalS',
   author_email='rajag2001416@gmail.com',
   maintainer=['RajagopalS rajag2001416@gmail.com','Vignesh_R mail2vikivignesh06@gmail.com','SenthilKumarN senthilkumarnallendran@gmail.com'],
   license='MIT', 
   classifiers=classifiers,
   keywords=['HRM','Melt','PCR'], 
   packages=find_packages(where='src'),
   package_dir={"":"src"},
-  package_data={'pyHRM':["*.py","*.h5"]},
+  package_data={"pyHRM":["*.py","*.h5"]},
+  include_package_data=True,
   install_requires=[
     'fpdf==1.7.2',
     'kaleido==0.2.1',
     'keras==2.12.0',
     'matplotlib==3.6.3',
     'numpy==1.23.5',
     'openpyxl==3.1.0',
```

### Comparing `pyHRM-0.1.2/src/pyHRM/Melt2_0.h5` & `pyHRM-0.1.3/src/pyHRM/Melt2_0.h5`

 * *Files identical despite different names*

### Comparing `pyHRM-0.1.2/src/pyHRM/melt.py` & `pyHRM-0.1.3/src/pyHRM/melt.py`

 * *Files identical despite different names*

### Comparing `pyHRM-0.1.2/src/pyHRM.egg-info/PKG-INFO` & `pyHRM-0.1.3/src/pyHRM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyHRM
-Version: 0.1.2
+Version: 0.1.3
 Summary: A novel library for processing DNA Melting signal with feature extraction and thresholding.
 Home-page: 
 Author: RajagopalS
 Author-email: rajag2001416@gmail.com
 Maintainer: ['RajagopalS rajag2001416@gmail.com', 'Vignesh_R mail2vikivignesh06@gmail.com', 'SenthilKumarN senthilkumarnallendran@gmail.com']
 License: MIT
 Keywords: HRM,Melt,PCR
```

