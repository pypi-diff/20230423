# Comparing `tmp/PyHRM-0.0.1.tar.gz` & `tmp/PyHRM-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyHRM-0.0.1.tar", last modified: Sun Apr 23 15:41:20 2023, max compression
+gzip compressed data, was "PyHRM-0.0.2.tar", last modified: Sun Apr 23 15:55:12 2023, max compression
```

## Comparing `PyHRM-0.0.1.tar` & `PyHRM-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 15:41:20.515723 PyHRM-0.0.1/
--rw-rw-rw-   0        0        0     1087 2023-04-22 11:02:58.000000 PyHRM-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0    13765 2023-04-23 15:41:20.515723 PyHRM-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    13015 2023-04-23 15:38:37.000000 PyHRM-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-23 15:41:20.515723 PyHRM-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-04-23 15:41:05.000000 PyHRM-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-23 15:41:20.468458 PyHRM-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-23 15:41:20.484077 PyHRM-0.0.1/src/PyHRM/
--rw-rw-rw-   0        0        0        0 2023-04-23 15:38:37.000000 PyHRM-0.0.1/src/PyHRM/__init__.py
--rw-rw-rw-   0        0        0    21543 2023-04-23 15:38:37.000000 PyHRM-0.0.1/src/PyHRM/melt.py
--rw-rw-rw-   0        0        0   240704 2023-04-23 15:38:37.000000 PyHRM-0.0.1/src/PyHRM/tar.h5
-drwxrwxrwx   0        0        0        0 2023-04-23 15:41:20.515723 PyHRM-0.0.1/src/PyHRM.egg-info/
--rw-rw-rw-   0        0        0    13765 2023-04-23 15:41:20.000000 PyHRM-0.0.1/src/PyHRM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-04-23 15:41:20.000000 PyHRM-0.0.1/src/PyHRM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 15:41:20.000000 PyHRM-0.0.1/src/PyHRM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      216 2023-04-23 15:41:20.000000 PyHRM-0.0.1/src/PyHRM.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-23 15:41:20.000000 PyHRM-0.0.1/src/PyHRM.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 15:55:12.016508 PyHRM-0.0.2/
+-rw-rw-rw-   0        0        0     1089 2023-04-23 15:53:47.000000 PyHRM-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0    13797 2023-04-23 15:55:12.016508 PyHRM-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    13015 2023-04-23 15:38:37.000000 PyHRM-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-23 15:55:12.016508 PyHRM-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1611 2023-04-23 15:54:45.000000 PyHRM-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 15:55:11.985245 PyHRM-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-23 15:55:12.000884 PyHRM-0.0.2/src/PyHRM/
+-rw-rw-rw-   0        0        0        0 2023-04-23 15:38:37.000000 PyHRM-0.0.2/src/PyHRM/__init__.py
+-rw-rw-rw-   0        0        0    21543 2023-04-23 15:38:37.000000 PyHRM-0.0.2/src/PyHRM/melt.py
+-rw-rw-rw-   0        0        0   240704 2023-04-23 15:38:37.000000 PyHRM-0.0.2/src/PyHRM/tar.h5
+drwxrwxrwx   0        0        0        0 2023-04-23 15:55:12.016508 PyHRM-0.0.2/src/PyHRM.egg-info/
+-rw-rw-rw-   0        0        0    13797 2023-04-23 15:55:11.000000 PyHRM-0.0.2/src/PyHRM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-04-23 15:55:11.000000 PyHRM-0.0.2/src/PyHRM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 15:55:11.000000 PyHRM-0.0.2/src/PyHRM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      216 2023-04-23 15:55:11.000000 PyHRM-0.0.2/src/PyHRM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-23 15:55:11.000000 PyHRM-0.0.2/src/PyHRM.egg-info/top_level.txt
```

### Comparing `PyHRM-0.0.1/LICENSE.txt` & `PyHRM-0.0.2/LICENSE.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2023 RajagopalS SenthilKumarN Vignesh_R
+Copyright 2023 Rajagopal S SenthilKumar N Vignesh R
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `PyHRM-0.0.1/PKG-INFO` & `PyHRM-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: PyHRM
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library for processing DNA Melting signal with feature extraction and automatic thresholding.
-Home-page: 
+Home-page: https://github.com/FEUSION/PyHRM
 Author: RajagopalS
 Author-email: rajag2001416@gmail.com
 Maintainer: ['RajagopalS rajag2001416@gmail.com', 'Vignesh_R mail2vikivignesh06@gmail.com', 'SenthilKumarN senthilkumarnallendran@gmail.com']
 License: MIT
 Keywords: HRM,Melt,PCR
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: PyHRM Version: 0.0.1 Summary: A library for
+Metadata-Version: 2.1 Name: PyHRM Version: 0.0.2 Summary: A library for
 processing DNA Melting signal with feature extraction and automatic
-thresholding. Home-page: Author: RajagopalS Author-email:
-rajag2001416@gmail.com Maintainer: ['RajagopalS rajag2001416@gmail.com',
-'Vignesh_R mail2vikivignesh06@gmail.com', 'SenthilKumarN
-senthilkumarnallendran@gmail.com'] License: MIT Keywords: HRM,Melt,PCR
-Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
-Audience :: Education Classifier: Operating System :: Microsoft :: Windows ::
-Windows 10 Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python :: 3 Description-Content-Type: text/markdown
-License-File: LICENSE.txt ![pyHRM](https://user-images.githubusercontent.com/
-80576855/233845390-87e32c95-b170-44b3-b1fb-82baaadea8e6.png)
+thresholding. Home-page: https://github.com/FEUSION/PyHRM Author: RajagopalS
+Author-email: rajag2001416@gmail.com Maintainer: ['RajagopalS
+rajag2001416@gmail.com', 'Vignesh_R mail2vikivignesh06@gmail.com',
+'SenthilKumarN senthilkumarnallendran@gmail.com'] License: MIT Keywords:
+HRM,Melt,PCR Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Education Classifier: Operating System ::
+Microsoft :: Windows :: Windows 10 Classifier: License :: OSI Approved :: MIT
+License Classifier: Programming Language :: Python :: 3 Description-Content-
+Type: text/markdown License-File: LICENSE.txt ![pyHRM](https://user-
+images.githubusercontent.com/80576855/233845390-87e32c95-b170-44b3-b1fb-
+82baaadea8e6.png)
 
 
                               ****** PyHRM ******
  ***** A library for processing DNA Melting signal with feature extraction and
                               thresholding. *****
          *** Installation â¢ Features â¢ Documentation â¢ Help ***
   **** [PyPI] [Release] [python] [https://img.shields.io/github/last-commit/
```

### Comparing `PyHRM-0.0.1/README.md` & `PyHRM-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `PyHRM-0.0.1/setup.py` & `PyHRM-0.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,19 +15,19 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='PyHRM',
-  version='0.0.1',
+  version='0.0.2',
   description='A library for processing DNA Melting signal with feature extraction and automatic thresholding.',
   long_description=long_description,
   long_description_content_type='text/markdown',
-  url='',  
+  url='https://github.com/FEUSION/PyHRM',  
   author='RajagopalS',
   author_email='rajag2001416@gmail.com',
   maintainer=['RajagopalS rajag2001416@gmail.com','Vignesh_R mail2vikivignesh06@gmail.com','SenthilKumarN senthilkumarnallendran@gmail.com'],
   license='MIT', 
   classifiers=classifiers,
   keywords=['HRM','Melt','PCR'], 
   packages=find_packages(where='src'),
```

### Comparing `PyHRM-0.0.1/src/PyHRM/melt.py` & `PyHRM-0.0.2/src/PyHRM/melt.py`

 * *Files identical despite different names*

### Comparing `PyHRM-0.0.1/src/PyHRM/tar.h5` & `PyHRM-0.0.2/src/PyHRM/tar.h5`

 * *Files identical despite different names*

### Comparing `PyHRM-0.0.1/src/PyHRM.egg-info/PKG-INFO` & `PyHRM-0.0.2/src/PyHRM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: PyHRM
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library for processing DNA Melting signal with feature extraction and automatic thresholding.
-Home-page: 
+Home-page: https://github.com/FEUSION/PyHRM
 Author: RajagopalS
 Author-email: rajag2001416@gmail.com
 Maintainer: ['RajagopalS rajag2001416@gmail.com', 'Vignesh_R mail2vikivignesh06@gmail.com', 'SenthilKumarN senthilkumarnallendran@gmail.com']
 License: MIT
 Keywords: HRM,Melt,PCR
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: PyHRM Version: 0.0.1 Summary: A library for
+Metadata-Version: 2.1 Name: PyHRM Version: 0.0.2 Summary: A library for
 processing DNA Melting signal with feature extraction and automatic
-thresholding. Home-page: Author: RajagopalS Author-email:
-rajag2001416@gmail.com Maintainer: ['RajagopalS rajag2001416@gmail.com',
-'Vignesh_R mail2vikivignesh06@gmail.com', 'SenthilKumarN
-senthilkumarnallendran@gmail.com'] License: MIT Keywords: HRM,Melt,PCR
-Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
-Audience :: Education Classifier: Operating System :: Microsoft :: Windows ::
-Windows 10 Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python :: 3 Description-Content-Type: text/markdown
-License-File: LICENSE.txt ![pyHRM](https://user-images.githubusercontent.com/
-80576855/233845390-87e32c95-b170-44b3-b1fb-82baaadea8e6.png)
+thresholding. Home-page: https://github.com/FEUSION/PyHRM Author: RajagopalS
+Author-email: rajag2001416@gmail.com Maintainer: ['RajagopalS
+rajag2001416@gmail.com', 'Vignesh_R mail2vikivignesh06@gmail.com',
+'SenthilKumarN senthilkumarnallendran@gmail.com'] License: MIT Keywords:
+HRM,Melt,PCR Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Education Classifier: Operating System ::
+Microsoft :: Windows :: Windows 10 Classifier: License :: OSI Approved :: MIT
+License Classifier: Programming Language :: Python :: 3 Description-Content-
+Type: text/markdown License-File: LICENSE.txt ![pyHRM](https://user-
+images.githubusercontent.com/80576855/233845390-87e32c95-b170-44b3-b1fb-
+82baaadea8e6.png)
 
 
                               ****** PyHRM ******
  ***** A library for processing DNA Melting signal with feature extraction and
                               thresholding. *****
          *** Installation â¢ Features â¢ Documentation â¢ Help ***
   **** [PyPI] [Release] [python] [https://img.shields.io/github/last-commit/
```

