# Comparing `tmp/Bgolearn-1.5.1.tar.gz` & `tmp/Bgolearn-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Bgolearn-1.5.1.tar", last modified: Sat Apr  8 12:19:38 2023, max compression
+gzip compressed data, was "Bgolearn-2.0.0.tar", last modified: Sun Apr 23 02:21:21 2023, max compression
```

## Comparing `Bgolearn-1.5.1.tar` & `Bgolearn-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-04-08 12:19:38.257979 Bgolearn-1.5.1/
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-04-08 12:19:38.257083 Bgolearn-1.5.1/Bgolearn/
--rwxr-xr-x   0 jacob      (501) staff       (20)    24205 2023-04-06 12:56:14.000000 Bgolearn-1.5.1/Bgolearn/BGO_eval.py
--rwxr-xr-x   0 jacob      (501) staff       (20)     3933 2022-11-06 07:11:02.000000 Bgolearn-1.5.1/Bgolearn/BGOclf.py
--rwxr-xr-x   0 jacob      (501) staff       (20)    18438 2022-10-13 07:31:41.000000 Bgolearn-1.5.1/Bgolearn/BGOmax.py
--rwxr-xr-x   0 jacob      (501) staff       (20)    18412 2022-10-14 04:10:19.000000 Bgolearn-1.5.1/Bgolearn/BGOmin.py
--rwxr-xr-x   0 jacob      (501) staff       (20)    20046 2023-04-07 02:02:09.000000 Bgolearn-1.5.1/Bgolearn/BGOsampling.py
--rwxr-xr-x   0 jacob      (501) staff       (20)      401 2023-04-07 02:04:26.000000 Bgolearn-1.5.1/Bgolearn/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-04-08 12:19:38.257694 Bgolearn-1.5.1/Bgolearn.egg-info/
--rw-r--r--   0 jacob      (501) staff       (20)     2478 2023-04-08 12:19:38.000000 Bgolearn-1.5.1/Bgolearn.egg-info/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      300 2023-04-08 12:19:38.000000 Bgolearn-1.5.1/Bgolearn.egg-info/SOURCES.txt
--rw-r--r--   0 jacob      (501) staff       (20)        1 2023-04-08 12:19:38.000000 Bgolearn-1.5.1/Bgolearn.egg-info/dependency_links.txt
--rw-r--r--   0 jacob      (501) staff       (20)       43 2023-04-08 12:19:38.000000 Bgolearn-1.5.1/Bgolearn.egg-info/requires.txt
--rw-r--r--   0 jacob      (501) staff       (20)        9 2023-04-08 12:19:38.000000 Bgolearn-1.5.1/Bgolearn.egg-info/top_level.txt
--rw-r--r--   0 jacob      (501) staff       (20)     2478 2023-04-08 12:19:38.257855 Bgolearn-1.5.1/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)     1917 2022-11-06 12:06:03.000000 Bgolearn-1.5.1/README.md
--rw-r--r--   0 jacob      (501) staff       (20)       38 2023-04-08 12:19:38.258017 Bgolearn-1.5.1/setup.cfg
--rw-r--r--   0 jacob      (501) staff       (20)     1366 2023-04-08 12:19:07.000000 Bgolearn-1.5.1/setup.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-04-23 02:21:21.588804 Bgolearn-2.0.0/
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-04-23 02:21:21.587920 Bgolearn-2.0.0/Bgolearn/
+-rwxr-xr-x   0 jacob      (501) staff       (20)    24205 2023-04-06 12:56:14.000000 Bgolearn-2.0.0/Bgolearn/BGO_eval.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)     3932 2023-04-23 02:14:51.000000 Bgolearn-2.0.0/Bgolearn/BGOclf.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)    18438 2022-10-13 07:31:41.000000 Bgolearn-2.0.0/Bgolearn/BGOmax.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)    18412 2022-10-14 04:10:19.000000 Bgolearn-2.0.0/Bgolearn/BGOmin.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)    19956 2023-04-23 02:19:14.000000 Bgolearn-2.0.0/Bgolearn/BGOsampling.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)      401 2023-04-07 02:04:26.000000 Bgolearn-2.0.0/Bgolearn/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-04-23 02:21:21.588523 Bgolearn-2.0.0/Bgolearn.egg-info/
+-rw-r--r--   0 jacob      (501) staff       (20)     2478 2023-04-23 02:21:21.000000 Bgolearn-2.0.0/Bgolearn.egg-info/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      300 2023-04-23 02:21:21.000000 Bgolearn-2.0.0/Bgolearn.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2023-04-23 02:21:21.000000 Bgolearn-2.0.0/Bgolearn.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       43 2023-04-23 02:21:21.000000 Bgolearn-2.0.0/Bgolearn.egg-info/requires.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        9 2023-04-23 02:21:21.000000 Bgolearn-2.0.0/Bgolearn.egg-info/top_level.txt
+-rw-r--r--   0 jacob      (501) staff       (20)     2478 2023-04-23 02:21:21.588681 Bgolearn-2.0.0/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)     1917 2022-11-06 12:06:03.000000 Bgolearn-2.0.0/README.md
+-rw-r--r--   0 jacob      (501) staff       (20)       38 2023-04-23 02:21:21.588843 Bgolearn-2.0.0/setup.cfg
+-rw-r--r--   0 jacob      (501) staff       (20)     1366 2023-04-23 02:19:25.000000 Bgolearn-2.0.0/setup.py
```

### Comparing `Bgolearn-1.5.1/Bgolearn/BGO_eval.py` & `Bgolearn-2.0.0/Bgolearn/BGO_eval.py`

 * *Files identical despite different names*

### Comparing `Bgolearn-1.5.1/Bgolearn/BGOclf.py` & `Bgolearn-2.0.0/Bgolearn/BGOclf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import warnings
 import numpy as np
 
 class Boundary(object):
     def __init__(self,model,data_matrix, Measured_response, virtual_samples, opt_num):
         warnings.filterwarnings('ignore')
         self.model = model
```

### Comparing `Bgolearn-1.5.1/Bgolearn/BGOmax.py` & `Bgolearn-2.0.0/Bgolearn/BGOmax.py`

 * *Files identical despite different names*

### Comparing `Bgolearn-1.5.1/Bgolearn/BGOmin.py` & `Bgolearn-2.0.0/Bgolearn/BGOmin.py`

 * *Files identical despite different names*

### Comparing `Bgolearn-1.5.1/Bgolearn/BGOsampling.py` & `Bgolearn-2.0.0/Bgolearn/BGOsampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import inspect
 import os
 import time
 import warnings
-import copy
-from tkinter import N
 import numpy as np
 import pandas as pd
 from .BGOmax import Global_max
 from .BGOmin import Global_min
 from .BGOclf import Boundary
 from .BGO_eval import BGO_Efficient
 from sklearn.model_selection import LeaveOneOut
-from sklearn.model_selection import cross_val_predict
 from sklearn.metrics import r2_score
 from sklearn.metrics import mean_absolute_error
 from sklearn.metrics import mean_squared_error
 from sklearn.gaussian_process import GaussianProcessRegressor
 from sklearn.gaussian_process.kernels import  RBF, WhiteKernel
 from sklearn.model_selection import KFold
 
@@ -131,16 +128,14 @@
                 BGOmodel = Boundary(model,data_matrix, Measured_response, virtual_samples, opt_num)
                 return BGOmodel
             else:
                 print('Type Error! Classifier should be one of the following:')
                 print('GaussianProcess; LogisticRegression;NaiveBayes;SVM;RandomForest')
 
 
-
-
         elif Mission == 'Regression':
         
             if Kriging_model == None:
                 kernel = RBF() + WhiteKernel()
                 if type(noise_std) == float:
                     # call the default model;
                     class Kriging_model(object):
```

### Comparing `Bgolearn-1.5.1/Bgolearn.egg-info/PKG-INFO` & `Bgolearn-2.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: Bgolearn
-Version: 1.5.1
-Summary: A Bayesian global optimization package for material design
-Home-page: https://github.com/Bin-Cao/Bgolearn
-Author: CaoBin
-Author-email: bcao@shu.edu.com
-Maintainer: CaoBin
-Maintainer-email: binjacobcao@gmail.com
-License: MIT License
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-
 
 [![](https://img.shields.io/badge/PyPI-caobin-blue)](https://pypi.org/project/Bgolearn/)
 # Python package - Bgolearn 
 
 
 
 ![Screen Shot 2022-07-11 at 9 13 28 AM](https://user-images.githubusercontent.com/86995074/178176016-8a79db81-fcfb-4af0-9b1c-aa4e6a113b5e.png)
```

### Comparing `Bgolearn-1.5.1/PKG-INFO` & `Bgolearn-2.0.0/Bgolearn.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: Bgolearn
-Version: 1.5.1
+Version: 2.0.0
 Summary: A Bayesian global optimization package for material design
 Home-page: https://github.com/Bin-Cao/Bgolearn
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.5
 
 
 [![](https://img.shields.io/badge/PyPI-caobin-blue)](https://pypi.org/project/Bgolearn/)
 # Python package - Bgolearn
```

### Comparing `Bgolearn-1.5.1/README.md` & `Bgolearn-2.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: Bgolearn
+Version: 2.0.0
+Summary: A Bayesian global optimization package for material design
+Home-page: https://github.com/Bin-Cao/Bgolearn
+Author: CaoBin
+Author-email: bcao@shu.edu.com
+Maintainer: CaoBin
+Maintainer-email: binjacobcao@gmail.com
+License: MIT License
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.5
+
 
 [![](https://img.shields.io/badge/PyPI-caobin-blue)](https://pypi.org/project/Bgolearn/)
 # Python package - Bgolearn 
 
 
 
 ![Screen Shot 2022-07-11 at 9 13 28 AM](https://user-images.githubusercontent.com/86995074/178176016-8a79db81-fcfb-4af0-9b1c-aa4e6a113b5e.png)
```

### Comparing `Bgolearn-1.5.1/setup.py` & `Bgolearn-2.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='Bgolearn',  # 包名
-    version='1.5.1',  # 版本
+    version='2.0.0',  # 版本
     description="A Bayesian global optimization package for material design",  # 包简介
     long_description=open('README.md',encoding='utf-8').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='CaoBin',  # 作者
     author_email='bcao@shu.edu.com',  # 作者邮件
     maintainer='CaoBin',  # 维护者
     maintainer_email='binjacobcao@gmail.com',  # 维护者邮件
@@ -15,15 +15,15 @@
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',  # 设置编写时的python版本
     ],
-    python_requires='>=3.7',  # 设置python版本要求
+    python_requires='>=3.5',  # 设置python版本要求
     install_requires=['scipy','scikit-learn','pandas','numpy','matplotlib'],  # 安装所需要的库
     entry_points={
         'console_scripts': [
             ''],
     },  # 设置命令行工具(可不使用就可以注释掉)
 
 )
```

