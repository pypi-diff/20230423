# Comparing `tmp/pyHRM-0.1.6.tar.gz` & `tmp/pyHRM-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyHRM-0.1.6.tar", last modified: Sun Apr 23 13:00:47 2023, max compression
+gzip compressed data, was "pyHRM-0.1.7.tar", last modified: Sun Apr 23 13:29:15 2023, max compression
```

## Comparing `pyHRM-0.1.6.tar` & `pyHRM-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 13:00:47.015982 pyHRM-0.1.6/
--rw-rw-rw-   0        0        0     1087 2023-04-22 11:02:58.000000 pyHRM-0.1.6/LICENSE.txt
--rw-rw-rw-   0        0        0    13614 2023-04-23 13:00:47.015982 pyHRM-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0    12874 2023-04-23 12:40:18.000000 pyHRM-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2023-04-23 13:00:47.015982 pyHRM-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1586 2023-04-23 13:00:23.000000 pyHRM-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-23 13:00:46.980225 pyHRM-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-23 13:00:46.995846 pyHRM-0.1.6/src/pyHRM/
--rw-rw-rw-   0        0        0        0 2023-04-23 12:40:18.000000 pyHRM-0.1.6/src/pyHRM/__init__.py
--rw-rw-rw-   0        0        0    21545 2023-04-23 12:40:18.000000 pyHRM-0.1.6/src/pyHRM/melt.py
--rw-rw-rw-   0        0        0   240704 2023-04-23 12:40:18.000000 pyHRM-0.1.6/src/pyHRM/tar.h5
-drwxrwxrwx   0        0        0        0 2023-04-23 13:00:47.011471 pyHRM-0.1.6/src/pyHRM.egg-info/
--rw-rw-rw-   0        0        0    13614 2023-04-23 13:00:46.000000 pyHRM-0.1.6/src/pyHRM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-04-23 13:00:46.000000 pyHRM-0.1.6/src/pyHRM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 13:00:46.000000 pyHRM-0.1.6/src/pyHRM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      216 2023-04-23 13:00:46.000000 pyHRM-0.1.6/src/pyHRM.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-23 13:00:46.000000 pyHRM-0.1.6/src/pyHRM.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 13:29:15.722220 pyHRM-0.1.7/
+-rw-rw-rw-   0        0        0     1087 2023-04-22 11:02:58.000000 pyHRM-0.1.7/LICENSE.txt
+-rw-rw-rw-   0        0        0    13614 2023-04-23 13:29:15.722220 pyHRM-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0    12874 2023-04-23 12:40:18.000000 pyHRM-0.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-23 13:29:15.722220 pyHRM-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1569 2023-04-23 13:28:53.000000 pyHRM-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 13:29:15.674894 pyHRM-0.1.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-23 13:29:15.674894 pyHRM-0.1.7/src/pyHRM/
+-rw-rw-rw-   0        0        0        0 2023-04-23 12:40:18.000000 pyHRM-0.1.7/src/pyHRM/__init__.py
+-rw-rw-rw-   0        0        0    21535 2023-04-23 13:27:39.000000 pyHRM-0.1.7/src/pyHRM/melt.py
+-rw-rw-rw-   0        0        0   240704 2023-04-23 12:40:18.000000 pyHRM-0.1.7/src/pyHRM/tar.h5
+drwxrwxrwx   0        0        0        0 2023-04-23 13:29:15.722220 pyHRM-0.1.7/src/pyHRM.egg-info/
+-rw-rw-rw-   0        0        0    13614 2023-04-23 13:29:15.000000 pyHRM-0.1.7/src/pyHRM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-04-23 13:29:15.000000 pyHRM-0.1.7/src/pyHRM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 13:29:15.000000 pyHRM-0.1.7/src/pyHRM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      216 2023-04-23 13:29:15.000000 pyHRM-0.1.7/src/pyHRM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-23 13:29:15.000000 pyHRM-0.1.7/src/pyHRM.egg-info/top_level.txt
```

### Comparing `pyHRM-0.1.6/LICENSE.txt` & `pyHRM-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyHRM-0.1.6/PKG-INFO` & `pyHRM-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyHRM
-Version: 0.1.6
+Version: 0.1.7
 Summary: A library for processing DNA Melting signal with feature extraction and thresholding.
 Home-page: 
 Author: RajagopalS
 Author-email: rajag2001416@gmail.com
 Maintainer: ['RajagopalS rajag2001416@gmail.com', 'Vignesh_R mail2vikivignesh06@gmail.com', 'SenthilKumarN senthilkumarnallendran@gmail.com']
 License: MIT
 Keywords: HRM,Melt,PCR
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyHRM Version: 0.1.6 Summary: A library for
+Metadata-Version: 2.1 Name: pyHRM Version: 0.1.7 Summary: A library for
 processing DNA Melting signal with feature extraction and thresholding. Home-
 page: Author: RajagopalS Author-email: rajag2001416@gmail.com Maintainer:
 ['RajagopalS rajag2001416@gmail.com', 'Vignesh_R mail2vikivignesh06@gmail.com',
 'SenthilKumarN senthilkumarnallendran@gmail.com'] License: MIT Keywords:
 HRM,Melt,PCR Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education Classifier: Operating System ::
 Microsoft :: Windows :: Windows 10 Classifier: License :: OSI Approved :: MIT
```

### Comparing `pyHRM-0.1.6/README.md` & `pyHRM-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pyHRM-0.1.6/setup.py` & `pyHRM-0.1.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from setuptools import setup, find_packages
 import os
-import pypandoc
 
 dir_path = os.path.dirname(os.path.abspath(__file__))
 
 rd_file = os.path.join(dir_path,'README.md')
 
 import io
 with io.open(rd_file, encoding="utf-8") as f:
@@ -16,15 +15,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='pyHRM',
-  version='0.1.6',
+  version='0.1.7',
   description='A library for processing DNA Melting signal with feature extraction and thresholding.',
   long_description=long_description,
   long_description_content_type='text/markdown',
   url='',  
   author='RajagopalS',
   author_email='rajag2001416@gmail.com',
   maintainer=['RajagopalS rajag2001416@gmail.com','Vignesh_R mail2vikivignesh06@gmail.com','SenthilKumarN senthilkumarnallendran@gmail.com'],
```

### Comparing `pyHRM-0.1.6/src/pyHRM/melt.py` & `pyHRM-0.1.7/src/pyHRM/melt.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 import matplotlib.pyplot as plt
 from matplotlib.backends.backend_agg import FigureCanvasAgg as FigureCanvas
 from fpdf import FPDF
 import tempfile
 import plotly.graph_objects as go
 import plotly.express as px
 import plotly.io as pio
-pio.renderers.default = 'notebook_connected'
+pio.renderers.default = 'notebook'
 for j in tqdm(range(5), desc=f'Setup Complete', leave=False):
     time.sleep(0.2)
 
 
 
 class MeltcurveInterpreter:
```

### Comparing `pyHRM-0.1.6/src/pyHRM/tar.h5` & `pyHRM-0.1.7/src/pyHRM/tar.h5`

 * *Files identical despite different names*

### Comparing `pyHRM-0.1.6/src/pyHRM.egg-info/PKG-INFO` & `pyHRM-0.1.7/src/pyHRM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyHRM
-Version: 0.1.6
+Version: 0.1.7
 Summary: A library for processing DNA Melting signal with feature extraction and thresholding.
 Home-page: 
 Author: RajagopalS
 Author-email: rajag2001416@gmail.com
 Maintainer: ['RajagopalS rajag2001416@gmail.com', 'Vignesh_R mail2vikivignesh06@gmail.com', 'SenthilKumarN senthilkumarnallendran@gmail.com']
 License: MIT
 Keywords: HRM,Melt,PCR
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyHRM Version: 0.1.6 Summary: A library for
+Metadata-Version: 2.1 Name: pyHRM Version: 0.1.7 Summary: A library for
 processing DNA Melting signal with feature extraction and thresholding. Home-
 page: Author: RajagopalS Author-email: rajag2001416@gmail.com Maintainer:
 ['RajagopalS rajag2001416@gmail.com', 'Vignesh_R mail2vikivignesh06@gmail.com',
 'SenthilKumarN senthilkumarnallendran@gmail.com'] License: MIT Keywords:
 HRM,Melt,PCR Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education Classifier: Operating System ::
 Microsoft :: Windows :: Windows 10 Classifier: License :: OSI Approved :: MIT
```

