# Comparing `tmp/mlsuite-2.1.3.tar.gz` & `tmp/mlsuite-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlsuite-2.1.3.tar", last modified: Fri Apr  7 03:43:14 2023, max compression
+gzip compressed data, was "mlsuite-2.1.4.tar", last modified: Sun Apr 23 08:48:48 2023, max compression
```

## Comparing `mlsuite-2.1.3.tar` & `mlsuite-2.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)        0 2023-04-07 03:43:14.876309 mlsuite-2.1.3/
--rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)     1067 2022-08-30 02:42:20.000000 mlsuite-2.1.3/LICENSE
-drwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)        0 2023-04-07 03:43:14.861553 mlsuite-2.1.3/MLsuite/
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     7701 2023-04-07 02:12:17.000000 mlsuite-2.1.3/MLsuite/MLArguments.py
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)    26629 2023-02-15 07:37:37.000000 mlsuite-2.1.3/MLsuite/MLEstimators.py
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     1931 2022-07-07 10:04:52.000000 mlsuite-2.1.3/MLsuite/MLLogging.py
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     2197 2023-04-07 02:10:21.000000 mlsuite-2.1.3/MLsuite/MLOpenWrite.py
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)      836 2022-09-06 09:45:06.000000 mlsuite-2.1.3/MLsuite/MLPipeline.py
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     4438 2022-09-13 08:33:47.000000 mlsuite-2.1.3/MLsuite/MLPredicting.py
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)    26637 2022-11-07 04:09:30.000000 mlsuite-2.1.3/MLsuite/MLSupervising.py
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     3424 2022-07-07 10:04:52.000000 mlsuite-2.1.3/MLsuite/MLUtilities.py
--rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)       17 2022-09-06 06:29:23.000000 mlsuite-2.1.3/MLsuite/__init__.py
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     2118 2022-12-14 01:57:48.000000 mlsuite-2.1.3/MLsuite/main.py
--rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)     1285 2023-04-07 03:43:14.874685 mlsuite-2.1.3/PKG-INFO
--rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)     2980 2023-04-07 03:40:56.000000 mlsuite-2.1.3/README.md
-drwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)        0 2023-04-07 03:43:14.872000 mlsuite-2.1.3/mlsuite.egg-info/
--rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)     1285 2023-04-07 03:43:14.000000 mlsuite-2.1.3/mlsuite.egg-info/PKG-INFO
--rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)      414 2023-04-07 03:43:14.000000 mlsuite-2.1.3/mlsuite.egg-info/SOURCES.txt
--rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)        1 2023-04-07 03:43:14.000000 mlsuite-2.1.3/mlsuite.egg-info/dependency_links.txt
--rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)      115 2023-04-07 03:43:14.000000 mlsuite-2.1.3/mlsuite.egg-info/requires.txt
--rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)        8 2023-04-07 03:43:14.000000 mlsuite-2.1.3/mlsuite.egg-info/top_level.txt
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)      455 2022-09-06 10:51:20.000000 mlsuite-2.1.3/mlsuite.py
--rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)       38 2023-04-07 03:43:14.876929 mlsuite-2.1.3/setup.cfg
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     1823 2023-04-07 03:42:00.000000 mlsuite-2.1.3/setup.py
+drwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)        0 2023-04-23 08:48:48.148092 mlsuite-2.1.4/
+-rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)     1067 2022-08-30 02:42:20.000000 mlsuite-2.1.4/LICENSE
+drwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)        0 2023-04-23 08:48:48.133675 mlsuite-2.1.4/MLsuite/
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     8137 2023-04-23 08:21:53.000000 mlsuite-2.1.4/MLsuite/MLArguments.py
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)    26629 2023-02-15 07:37:37.000000 mlsuite-2.1.4/MLsuite/MLEstimators.py
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     1931 2022-07-07 10:04:52.000000 mlsuite-2.1.4/MLsuite/MLLogging.py
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     2197 2023-04-07 02:10:21.000000 mlsuite-2.1.4/MLsuite/MLOpenWrite.py
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)      836 2022-09-06 09:45:06.000000 mlsuite-2.1.4/MLsuite/MLPipeline.py
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     4438 2022-09-13 08:33:47.000000 mlsuite-2.1.4/MLsuite/MLPredicting.py
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)    26665 2023-04-23 08:05:06.000000 mlsuite-2.1.4/MLsuite/MLSupervising.py
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     3424 2022-07-07 10:04:52.000000 mlsuite-2.1.4/MLsuite/MLUtilities.py
+-rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)       17 2022-09-06 06:29:23.000000 mlsuite-2.1.4/MLsuite/__init__.py
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     2118 2022-12-14 01:57:48.000000 mlsuite-2.1.4/MLsuite/main.py
+-rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)     1285 2023-04-23 08:48:48.146534 mlsuite-2.1.4/PKG-INFO
+-rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)     3421 2023-04-23 08:21:06.000000 mlsuite-2.1.4/README.md
+drwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)        0 2023-04-23 08:48:48.143899 mlsuite-2.1.4/mlsuite.egg-info/
+-rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)     1285 2023-04-23 08:48:47.000000 mlsuite-2.1.4/mlsuite.egg-info/PKG-INFO
+-rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)      414 2023-04-23 08:48:47.000000 mlsuite-2.1.4/mlsuite.egg-info/SOURCES.txt
+-rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)        1 2023-04-23 08:48:47.000000 mlsuite-2.1.4/mlsuite.egg-info/dependency_links.txt
+-rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)      115 2023-04-23 08:48:47.000000 mlsuite-2.1.4/mlsuite.egg-info/requires.txt
+-rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)        8 2023-04-23 08:48:47.000000 mlsuite-2.1.4/mlsuite.egg-info/top_level.txt
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)      455 2022-09-06 10:51:20.000000 mlsuite-2.1.4/mlsuite.py
+-rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)       38 2023-04-23 08:48:48.148654 mlsuite-2.1.4/setup.cfg
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     1823 2023-04-23 08:12:39.000000 mlsuite-2.1.4/setup.py
```

### Comparing `mlsuite-2.1.3/LICENSE` & `mlsuite-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mlsuite-2.1.3/MLsuite/MLArguments.py` & `mlsuite-2.1.4/MLsuite/MLArguments.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,24 +17,28 @@
                 formatter_class=argparse.RawDescriptionHelpFormatter,
                 prefix_chars='-+',
                 conflict_handler='resolve',
                 description="\nThe traditional machine learning analysis based on sklearn package:\n",
                 epilog='''\
 Example:
 1. python mlsuite.py Auto    -i data.traintest.txt -g group.new.txt -p data.predict.txt -o testdt/ -m DT
-2. python mlsuite.py Auto    -i data.traintest.txt -g group.new.txt -o testdt/ -m DT
-3. python mlsuite.py Fitting -i data.traintest.txt -g group.new.txt -o testdt/ -m DT
-4. python mlsuite.py Predict -p data.predict.txt   -g group.new.txt -x modelpath/ -y predictdt/ -m DT.''')
+2. python mlsuite.py Auto    -i data.traintest.txt -g group.new.txt -p data.predict.txt -o testdt/ -m DT -f (10 times sample grouping and 10 models)
+3. python mlsuite.py Auto    -i data.traintest.txt -g group.new.txt -o testdt/ -m DT
+4. python mlsuite.py Fitting -i data.traintest.txt -g group.new.txt -o testdt/ -m DT
+5. python mlsuite.py Fitting -i data.traintest.txt -g group.new.txt -o testdt/ -m DT -f (10 times sample grouping and 10 models)
+6. python mlsuite.py Predict -p data.predict.txt   -g group.new.txt -x modelpath/ -y predictdt/ -m DT.''')
 
     parser.add_argument('-V','--version',action ='version',
-                version='mlsuite version 2.1.3')
+                version='mlsuite version 2.1.4')
     subparsers = parser.add_subparsers(dest="commands",
                     help='machine learning models help.')
     ### Fitting module
     P_fitting  = subparsers.add_parser('Fitting',conflict_handler='resolve', add_help=False)
+    P_fitting.add_argument("-f", "--fit_10", action="store_true", default=False,
+                    help='''fitting modeling by 10 times sample spliting''')
     P_fitting.add_argument("-i", "--input",type=str,
                     help='''the input train and test data file with dataframe format  by row(samples) x columns (features and Y). the sample column name must be Sample.
 ''')
     P_fitting.add_argument("-g", "--group",type=str,required=True,
                     help='''the group file tell the featues, groups and variable type, which has Variables, Group, Type columns. Only continuous and discrete variables are supported in variable type. Onehot variables is coming.''')
     P_fitting.add_argument("-o", "--outdir",type=str,default=os.getcwd(),
                     help="output file dir, default=current dir.")
```

### Comparing `mlsuite-2.1.3/MLsuite/MLEstimators.py` & `mlsuite-2.1.4/MLsuite/MLEstimators.py`

 * *Files identical despite different names*

### Comparing `mlsuite-2.1.3/MLsuite/MLLogging.py` & `mlsuite-2.1.4/MLsuite/MLLogging.py`

 * *Files identical despite different names*

### Comparing `mlsuite-2.1.3/MLsuite/MLOpenWrite.py` & `mlsuite-2.1.4/MLsuite/MLOpenWrite.py`

 * *Files identical despite different names*

### Comparing `mlsuite-2.1.3/MLsuite/MLPipeline.py` & `mlsuite-2.1.4/MLsuite/MLPipeline.py`

 * *Files identical despite different names*

### Comparing `mlsuite-2.1.3/MLsuite/MLPredicting.py` & `mlsuite-2.1.4/MLsuite/MLPredicting.py`

 * *Files identical despite different names*

### Comparing `mlsuite-2.1.3/MLsuite/MLSupervising.py` & `mlsuite-2.1.4/MLsuite/MLSupervising.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                 n_splits=self.arg.crossV, test_size=self.arg.testS, CVt=self.arg.CVfit, n_repeats=2, leavP=self.arg.leavP, random_state=self.arg.random)
             SFA = CrossvalidationSplit(
                 n_splits=self.arg.crossV, test_size=self.arg.testS, CVt='SFA', n_repeats=2, leavP=self.arg.leavP, random_state=self.arg.random)
             for train_index, test_index in CVS.split(Xdf, Ydf):
                 all_test.extend(test_index)
                 all_split.append([train_index.tolist(), test_index.tolist()])
             # if the unique of all test sample is not equal to input sample, add other 3 sets data by SFA method spliting
-            if self.arg.CVfit == 'SSA':
+            if self.arg.CVfit == 'SSA' and not self.arg.fit_10:
                 if len(set(all_test)) < len(Ydf):
                     all_add = [[tr.tolist(), te.tolist()]
                                for tr, te in SFA.split(Xdf, Ydf)]
                     all_split += all_add
         return(all_split)
 
 
@@ -412,15 +412,15 @@
  
 ### define some functions
 def modeling(arg, x_train, x_test, y_train, y_test, Typi, mclass, _k, _n, allGroup):
     log = ''
     hyper = HyperparamOptimal(arg, log, model=arg.model, y_variable_type=Typi, y_variable_class=mclass)
     hyper.Hyperparemet(x_train, x_test, y_train, y_test)
     predict, coef, Best_MD = hyper.getModelResult()
-    Openf('%s%s_Class_%s_predict.xls'%(arg.output, 'Group', str(_n)), (predict), index=True, index_label='sample').openv()
+    Openf('%s%s_Class_%s_predict.xls'%(arg.output, 'Group', str(_n+1)), (predict), index=True, index_label='sample').openv()
     logText = hyper.log
     # addmodel
     if (arg.model in ['GBDT', 'XGB', 'RF']) and (arg.Addmode !='N'):
         log_add = ''
         x_train_add, OHE = HyperparamOptimal.OneHot(model=arg.model, clf=hyper.clf, x_matrix=x_train)
         x_test_add,  OHE = HyperparamOptimal.OneHot(model=arg.model, clf=hyper.clf, x_matrix=x_test, OHE=OHE)
         x_matrix_add, OHE_merge = HyperparamOptimal.OneHot(model=arg.model, clf=hyper.new_clf, x_matrix=hyper.x)
@@ -458,15 +458,15 @@
         Log.NIF('%s Value Counts:\n%s' % (Yi, DFall[Yi].value_counts().to_string())) 
         DFall[Yi] = Check_Label(DFall[Yi])
         # sample was splited into 13 groups
         sample_split = sampleSplit(args)
         sample_group_index = sample_split.CVSplit(Xdf=DFall[Xi], Ydf=DFall[Yi])
         # hyperparameter optimization (use the first set of data)
         allPredict, allCoef, allScore, allMD = [], [], [], []
-        threads = []
+        # threads = []
         for repeat in range(args.Repeatime):
             for i in range(len(sample_group_index)):
                 train_index, test_index = sample_group_index[i]
                 train , test = DFall.iloc[train_index, :], DFall.iloc[test_index, :]
                 x_train, y_train = train[Xi], train[Yi]
                 x_test , y_test  = test[Xi], test[Yi]
             #    t = MyThread(modeling, (args, x_train, x_test, y_train, y_test, Typi, DFall[Yi].nunique(), repeat, i, len(sample_group_index)))
```

### Comparing `mlsuite-2.1.3/MLsuite/MLUtilities.py` & `mlsuite-2.1.4/MLsuite/MLUtilities.py`

 * *Files identical despite different names*

### Comparing `mlsuite-2.1.3/MLsuite/main.py` & `mlsuite-2.1.4/MLsuite/main.py`

 * *Files identical despite different names*

### Comparing `mlsuite-2.1.3/PKG-INFO` & `mlsuite-2.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlsuite
-Version: 2.1.3
+Version: 2.1.4
 Summary: The traditional machine learning analysis based on sklearn package
 Home-page: https://git.genecast.com.cn/narwhal/mlsuite
 Author: suxing li
 Author-email: li.suxing@genecast.com.cn
 Maintainer: suxing li
 Maintainer-email: li.suxing@genecast.com.cn
 Platform: all
```

### Comparing `mlsuite-2.1.3/README.md` & `mlsuite-2.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # mlsuite
 
 ## Install
 
 ```
-pip install mlsuite==2.1.3
+pip install mlsuite==2.1.4
 pip install https://github.com/JamesRitchie/scikit-rvm/archive/master.zip
 ```
 
 ## Usage
 
 Notice: used pyhton3, not python2
 
@@ -25,19 +25,24 @@
 optional arguments:
   -h, --help            show this help message and exit
   -V, --version         show program's version number and exit
 
 Example:
 
 1. python mlsuite.py Auto    -i data.traintest.txt -g group.new.txt -p data.predict.txt -o testdt/ -m DT
-2. python mlsuite.py Auto    -i data.traintest.txt -g group.new.txt -o testdt/ -m DT
-3. python mlsuite.py Fitting -i data.traintest.txt -g group.new.txt -o testdt/ -m DT
-4. python mlsuite.py Predict -p data.predict.txt   -g group.new.txt -x modelpath/ -y predictdt/ -m DT.
+2. python mlsuite.py Auto    -i data.traintest.txt -g group.new.txt -p data.predict.txt -o testdt/ -m DT -f (10 times sample grouping and 10 models)
+3. python mlsuite.py Auto    -i data.traintest.txt -g group.new.txt -o testdt/ -m DT
+4. python mlsuite.py Fitting -i data.traintest.txt -g group.new.txt -o testdt/ -m DT
+5. python mlsuite.py Fitting -i data.traintest.txt -g group.new.txt -o testdt/ -m DT -f (10 times sample grouping and 10 models)
+6. python mlsuite.py Predict -p data.predict.txt   -g group.new.txt -x modelpath/ -y predictdt/ -m DT.
 
 ## Update log
+### v2.1.4
+1. "Fitting" module has been added "-f|--fit_10" arguments, which the input training dataset was splited into 10 train/test groups, and got 10 models.
+
 ### v2.1.3
 1. pandas's parameter "line_terminator" had changed into "lineterminator" in the 2.0.0 version, so drop "line_terminator" in "MLOpenWrite.py" script.
 2. fixed same packages' version:
 ```
     lightgbm == 3.3.3,
     joblib == 1.2.0,
     numpy == 1.21.4,
```

### Comparing `mlsuite-2.1.3/mlsuite.egg-info/PKG-INFO` & `mlsuite-2.1.4/mlsuite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlsuite
-Version: 2.1.3
+Version: 2.1.4
 Summary: The traditional machine learning analysis based on sklearn package
 Home-page: https://git.genecast.com.cn/narwhal/mlsuite
 Author: suxing li
 Author-email: li.suxing@genecast.com.cn
 Maintainer: suxing li
 Maintainer-email: li.suxing@genecast.com.cn
 Platform: all
```

### Comparing `mlsuite-2.1.3/setup.py` & `mlsuite-2.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages, setup
 from glob import glob
 from os.path import dirname, join
 import os
 
 setup(
     name='mlsuite',
-    version='2.1.3',
+    version='2.1.4',
     description='The traditional machine learning analysis based on sklearn package',
     author='suxing li',
     author_email='li.suxing@genecast.com.cn',
     maintainer='suxing li',
     maintainer_email='li.suxing@genecast.com.cn',
     packages=find_packages(where='.', exclude=(), include=('*',)),
     include_package_data=True,
```

