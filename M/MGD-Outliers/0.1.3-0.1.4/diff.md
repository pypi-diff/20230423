# Comparing `tmp/MGD_Outliers-0.1.3.tar.gz` & `tmp/MGD_Outliers-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MGD_Outliers-0.1.3.tar", last modified: Sat Apr 22 10:40:20 2023, max compression
+gzip compressed data, was "MGD_Outliers-0.1.4.tar", last modified: Sun Apr 23 06:18:24 2023, max compression
```

## Comparing `MGD_Outliers-0.1.3.tar` & `MGD_Outliers-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 mayurdushetwar   (501) staff       (20)        0 2023-04-22 10:40:20.793153 MGD_Outliers-0.1.3/
--rw-r--r--   0 mayurdushetwar   (501) staff       (20)    11357 2023-04-20 07:09:20.000000 MGD_Outliers-0.1.3/LICENSE
--rw-r--r--   0 mayurdushetwar   (501) staff       (20)     2249 2023-04-22 10:40:20.792981 MGD_Outliers-0.1.3/PKG-INFO
--rw-r--r--   0 mayurdushetwar   (501) staff       (20)     1498 2023-04-22 10:39:48.000000 MGD_Outliers-0.1.3/README.md
--rw-r--r--   0 mayurdushetwar   (501) staff       (20)       38 2023-04-22 10:40:20.793210 MGD_Outliers-0.1.3/setup.cfg
--rw-r--r--   0 mayurdushetwar   (501) staff       (20)     1288 2023-04-22 10:39:57.000000 MGD_Outliers-0.1.3/setup.py
-drwxr-xr-x   0 mayurdushetwar   (501) staff       (20)        0 2023-04-22 10:40:20.791933 MGD_Outliers-0.1.3/utils/
-drwxr-xr-x   0 mayurdushetwar   (501) staff       (20)        0 2023-04-22 10:40:20.792720 MGD_Outliers-0.1.3/utils/MGD_Outliers.egg-info/
--rw-r--r--   0 mayurdushetwar   (501) staff       (20)     2249 2023-04-22 10:40:20.000000 MGD_Outliers-0.1.3/utils/MGD_Outliers.egg-info/PKG-INFO
--rw-r--r--   0 mayurdushetwar   (501) staff       (20)      257 2023-04-22 10:40:20.000000 MGD_Outliers-0.1.3/utils/MGD_Outliers.egg-info/SOURCES.txt
--rw-r--r--   0 mayurdushetwar   (501) staff       (20)        1 2023-04-22 10:40:20.000000 MGD_Outliers-0.1.3/utils/MGD_Outliers.egg-info/dependency_links.txt
--rw-r--r--   0 mayurdushetwar   (501) staff       (20)       39 2023-04-22 10:40:20.000000 MGD_Outliers-0.1.3/utils/MGD_Outliers.egg-info/requires.txt
--rw-r--r--   0 mayurdushetwar   (501) staff       (20)       13 2023-04-22 10:40:20.000000 MGD_Outliers-0.1.3/utils/MGD_Outliers.egg-info/top_level.txt
--rw-r--r--   0 mayurdushetwar   (501) staff       (20)    16159 2023-04-22 10:16:16.000000 MGD_Outliers-0.1.3/utils/MGD_Outliers.py
+drwxr-xr-x   0 mayurdushetwar   (501) staff       (20)        0 2023-04-23 06:18:24.314452 MGD_Outliers-0.1.4/
+-rw-r--r--   0 mayurdushetwar   (501) staff       (20)    11357 2023-04-20 07:09:20.000000 MGD_Outliers-0.1.4/LICENSE
+-rw-r--r--   0 mayurdushetwar   (501) staff       (20)     2657 2023-04-23 06:18:24.314288 MGD_Outliers-0.1.4/PKG-INFO
+-rw-r--r--   0 mayurdushetwar   (501) staff       (20)     1906 2023-04-23 06:17:32.000000 MGD_Outliers-0.1.4/README.md
+-rw-r--r--   0 mayurdushetwar   (501) staff       (20)       38 2023-04-23 06:18:24.314514 MGD_Outliers-0.1.4/setup.cfg
+-rw-r--r--   0 mayurdushetwar   (501) staff       (20)     1288 2023-04-23 06:17:39.000000 MGD_Outliers-0.1.4/setup.py
+drwxr-xr-x   0 mayurdushetwar   (501) staff       (20)        0 2023-04-23 06:18:24.313388 MGD_Outliers-0.1.4/utils/
+drwxr-xr-x   0 mayurdushetwar   (501) staff       (20)        0 2023-04-23 06:18:24.314078 MGD_Outliers-0.1.4/utils/MGD_Outliers.egg-info/
+-rw-r--r--   0 mayurdushetwar   (501) staff       (20)     2657 2023-04-23 06:18:24.000000 MGD_Outliers-0.1.4/utils/MGD_Outliers.egg-info/PKG-INFO
+-rw-r--r--   0 mayurdushetwar   (501) staff       (20)      257 2023-04-23 06:18:24.000000 MGD_Outliers-0.1.4/utils/MGD_Outliers.egg-info/SOURCES.txt
+-rw-r--r--   0 mayurdushetwar   (501) staff       (20)        1 2023-04-23 06:18:24.000000 MGD_Outliers-0.1.4/utils/MGD_Outliers.egg-info/dependency_links.txt
+-rw-r--r--   0 mayurdushetwar   (501) staff       (20)       39 2023-04-23 06:18:24.000000 MGD_Outliers-0.1.4/utils/MGD_Outliers.egg-info/requires.txt
+-rw-r--r--   0 mayurdushetwar   (501) staff       (20)       13 2023-04-23 06:18:24.000000 MGD_Outliers-0.1.4/utils/MGD_Outliers.egg-info/top_level.txt
+-rw-r--r--   0 mayurdushetwar   (501) staff       (20)    16181 2023-04-23 06:17:24.000000 MGD_Outliers-0.1.4/utils/MGD_Outliers.py
```

### Comparing `MGD_Outliers-0.1.3/LICENSE` & `MGD_Outliers-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `MGD_Outliers-0.1.3/PKG-INFO` & `MGD_Outliers-0.1.4/utils/MGD_Outliers.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: MGD_Outliers
-Version: 0.1.3
+Name: MGD-Outliers
+Version: 0.1.4
 Summary: MGD_Outliers is a Pypyththon package for identifying and visualizing outliers in a DataFrame.
 Home-page: UNKNOWN
 Author: Mayur Dushetwar
 Author-email: <mdushetwar@gmail.com>
 License: Apache License 2.0
 Keywords: python,dataframe,outlier,outliers,inter quartile range,plot outliers,count outliers,data processing,drop outliers
 Platform: UNKNOWN
@@ -15,54 +15,61 @@
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >= 3.9.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # MGD_Outliers
-MGD_Outliers is an open-source Python package for detecting and analyzing outliers in data. The package provides a class, Outliers, which can be used to detect outliers in numerical data, and provides several methods to analyze and visualize the detected outliers.
+MGD_Outliers is an open-source Python package for detecting and analyzing outliers in data. The package provides a class, OutlierNinja, which can be used to detect outliers in numerical data, and provides several methods to analyze and visualize the detected outliers in quick and efficient manner.
 
 # Current version
- version 0.1.3
+ version 0.1.4
 
 # Installation
 
 You can install MGD_Outliers using pip:
 
     pip install MGD_Outliers
     
 
 # Usage
 
-To use the Outliers class in MGD_Outliers, you first need to import the package:
+To use the OutlierNinja class in MGD_Outliers, you first need to import the package:
 
-    from MGD_Outliers import Outliers
+    from MGD_Outliers import OutlierNinja
     
 
-Then, you can create an instance of the Outliers class and pass your data to it:
+Then, you have to create an instance of the OutlierNinja class:
 
-    outliers = Outliers(data)
+    outliers = OutlierNinja(limit_factor=1.5)   # 1.5 is a default value, you can change it as per your project requirement
  
 
-Once you have an instance of the Outliers class, you can use its methods to detect and analyze outliers. For example, you can use the detect_outliers method to detect outliers in the data:
+Then, you need to train this object using a dataframe object
 
-    outliers.get_outliers()
+    outliers.fit(data)
+
+
+Once the OutlierNinja object is trained, you can sit back, relax with your favorite drink and call its methods and attributes like a true data ninja. 
+For example, you can use the detect_outliers method to locate outliers in the data:
+
+    outliers.detect_outliers(column_name='age')
    
 
-You can also use the plot_outlier_count method to plot barplot of the columns with the detected outliers highlighted:
+You can also use the plot_outlier_count method to plot barplot of the columns:
 
     outliers.plot_outlier_count()
 
 
-For a full list of methods available in the Outliers class, see the documentation.
+For a full list of methods available in the OutlierNinja class, see the documentation. I hope you find this package helpful. So, let the OutlierNinja package do the hard work, while you sip on your drink and reap the benefits of a well-optimized dataset.
+
 
 # License
 This package is licensed under the Apache License 2.0. See the LICENSE file for more information.
 
 
-Contributing
+# Contributing
 If you find any bugs or issues with MGD_Outliers, or if you have any suggestions for new features, please open an issue on GitHub. If you would like to contribute to the development of MGD_Outliers, please fork the repository and submit a pull request.
```

### Comparing `MGD_Outliers-0.1.3/README.md` & `MGD_Outliers-0.1.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,53 @@
 # MGD_Outliers
-MGD_Outliers is an open-source Python package for detecting and analyzing outliers in data. The package provides a class, Outliers, which can be used to detect outliers in numerical data, and provides several methods to analyze and visualize the detected outliers.
+MGD_Outliers is an open-source Python package for detecting and analyzing outliers in data. The package provides a class, OutlierNinja, which can be used to detect outliers in numerical data, and provides several methods to analyze and visualize the detected outliers in quick and efficient manner.
 
 # Current version
- version 0.1.3
+ version 0.1.4
 
 # Installation
 
 You can install MGD_Outliers using pip:
 
     pip install MGD_Outliers
     
 
 # Usage
 
-To use the Outliers class in MGD_Outliers, you first need to import the package:
+To use the OutlierNinja class in MGD_Outliers, you first need to import the package:
 
-    from MGD_Outliers import Outliers
+    from MGD_Outliers import OutlierNinja
     
 
-Then, you can create an instance of the Outliers class and pass your data to it:
+Then, you have to create an instance of the OutlierNinja class:
 
-    outliers = Outliers(data)
+    outliers = OutlierNinja(limit_factor=1.5)   # 1.5 is a default value, you can change it as per your project requirement
  
 
-Once you have an instance of the Outliers class, you can use its methods to detect and analyze outliers. For example, you can use the detect_outliers method to detect outliers in the data:
+Then, you need to train this object using a dataframe object
 
-    outliers.get_outliers()
+    outliers.fit(data)
+
+
+Once the OutlierNinja object is trained, you can sit back, relax with your favorite drink and call its methods and attributes like a true data ninja. 
+For example, you can use the detect_outliers method to locate outliers in the data:
+
+    outliers.detect_outliers(column_name='age')
    
 
-You can also use the plot_outlier_count method to plot barplot of the columns with the detected outliers highlighted:
+You can also use the plot_outlier_count method to plot barplot of the columns:
 
     outliers.plot_outlier_count()
 
 
-For a full list of methods available in the Outliers class, see the documentation.
+For a full list of methods available in the OutlierNinja class, see the documentation. I hope you find this package helpful. So, let the OutlierNinja package do the hard work, while you sip on your drink and reap the benefits of a well-optimized dataset.
+
 
 # License
 This package is licensed under the Apache License 2.0. See the LICENSE file for more information.
 
 
-Contributing
+# Contributing
 If you find any bugs or issues with MGD_Outliers, or if you have any suggestions for new features, please open an issue on GitHub. If you would like to contribute to the development of MGD_Outliers, please fork the repository and submit a pull request.
```

### Comparing `MGD_Outliers-0.1.3/setup.py` & `MGD_Outliers-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 DESCRIPTION = 'MGD_Outliers is a Pypyththon package for identifying and visualizing outliers in a DataFrame.'
 
 
 # Setting up
 setup(
     name="MGD_Outliers",
     version=VERSION,
```

### Comparing `MGD_Outliers-0.1.3/utils/MGD_Outliers.egg-info/PKG-INFO` & `MGD_Outliers-0.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: MGD-Outliers
-Version: 0.1.3
+Name: MGD_Outliers
+Version: 0.1.4
 Summary: MGD_Outliers is a Pypyththon package for identifying and visualizing outliers in a DataFrame.
 Home-page: UNKNOWN
 Author: Mayur Dushetwar
 Author-email: <mdushetwar@gmail.com>
 License: Apache License 2.0
 Keywords: python,dataframe,outlier,outliers,inter quartile range,plot outliers,count outliers,data processing,drop outliers
 Platform: UNKNOWN
@@ -15,54 +15,61 @@
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >= 3.9.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # MGD_Outliers
-MGD_Outliers is an open-source Python package for detecting and analyzing outliers in data. The package provides a class, Outliers, which can be used to detect outliers in numerical data, and provides several methods to analyze and visualize the detected outliers.
+MGD_Outliers is an open-source Python package for detecting and analyzing outliers in data. The package provides a class, OutlierNinja, which can be used to detect outliers in numerical data, and provides several methods to analyze and visualize the detected outliers in quick and efficient manner.
 
 # Current version
- version 0.1.3
+ version 0.1.4
 
 # Installation
 
 You can install MGD_Outliers using pip:
 
     pip install MGD_Outliers
     
 
 # Usage
 
-To use the Outliers class in MGD_Outliers, you first need to import the package:
+To use the OutlierNinja class in MGD_Outliers, you first need to import the package:
 
-    from MGD_Outliers import Outliers
+    from MGD_Outliers import OutlierNinja
     
 
-Then, you can create an instance of the Outliers class and pass your data to it:
+Then, you have to create an instance of the OutlierNinja class:
 
-    outliers = Outliers(data)
+    outliers = OutlierNinja(limit_factor=1.5)   # 1.5 is a default value, you can change it as per your project requirement
  
 
-Once you have an instance of the Outliers class, you can use its methods to detect and analyze outliers. For example, you can use the detect_outliers method to detect outliers in the data:
+Then, you need to train this object using a dataframe object
 
-    outliers.get_outliers()
+    outliers.fit(data)
+
+
+Once the OutlierNinja object is trained, you can sit back, relax with your favorite drink and call its methods and attributes like a true data ninja. 
+For example, you can use the detect_outliers method to locate outliers in the data:
+
+    outliers.detect_outliers(column_name='age')
    
 
-You can also use the plot_outlier_count method to plot barplot of the columns with the detected outliers highlighted:
+You can also use the plot_outlier_count method to plot barplot of the columns:
 
     outliers.plot_outlier_count()
 
 
-For a full list of methods available in the Outliers class, see the documentation.
+For a full list of methods available in the OutlierNinja class, see the documentation. I hope you find this package helpful. So, let the OutlierNinja package do the hard work, while you sip on your drink and reap the benefits of a well-optimized dataset.
+
 
 # License
 This package is licensed under the Apache License 2.0. See the LICENSE file for more information.
 
 
-Contributing
+# Contributing
 If you find any bugs or issues with MGD_Outliers, or if you have any suggestions for new features, please open an issue on GitHub. If you would like to contribute to the development of MGD_Outliers, please fork the repository and submit a pull request.
```

### Comparing `MGD_Outliers-0.1.3/utils/MGD_Outliers.py` & `MGD_Outliers-0.1.4/utils/MGD_Outliers.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 
         Parameters:
         -----------
         data (pd.DataFrame): The input DataFrame containing the data to analyze.
         limit_factor (float, optional): The threshold value to use for identifying outliers based on the IQR.
         """
 
-        self.limit_factor = limit_factor
+        self.limit_factor_ = limit_factor
         self.__data = None
-        self.numeric_columns = None
+        self.numeric_columns_ = None
         self.__lower_limit_dict = {}
         self.__upper_limit_dict = {}
         self.__iqr = {}
         
     def fit(self, data):
 
         '''
@@ -62,21 +62,21 @@
         >>> outlier = Outliers(limit_factor=1.5)
         >>> outlier.fit(df)
         'Upper and lower limits identified successfully!'
         '''
 
         try:
             self.__data = data 
-            self.numeric_columns = self.__data.select_dtypes(include=[np.number]).columns
+            self.numeric_columns_ = self.__data.select_dtypes(include=[np.number]).columns
             
-            for col in self.numeric_columns:
+            for col in self.numeric_columns_:
                 q1, q3 = self.__data[col].quantile([0.25, 0.75])
                 val_iqr = q3 - q1
-                self.__lower_limit_dict[col] = q1 - self.limit_factor * val_iqr
-                self.__upper_limit_dict[col] = q3 + self.limit_factor * val_iqr
+                self.__lower_limit_dict[col] = q1 - self.limit_factor_ * val_iqr
+                self.__upper_limit_dict[col] = q3 + self.limit_factor_ * val_iqr
                 self.__iqr[col] = val_iqr
 
             return 'Upper and lower limits identified successfully!'
         
         except Exception as e:
             return f"Error occurred in fit(): {e}"
 
@@ -107,23 +107,23 @@
             >>> outliers.fit(data)
             >>> outliers.get_iqr()
             >>> outliers.get_iqr(['age'])
         """
 
         
         if column_names is None:
-            column_names = self.numeric_columns
+            column_names = self.numeric_columns_
 
         elif not isinstance(column_names, list):
                 raise ValueError("column_names must be a list")
         for col in column_names:
-            if col not in self.numeric_columns:
+            if col not in self.numeric_columns_:
                 raise ValueError(f"Column name {col} does not exist or is not numerical")
         else:
-            column_names = [col for col in column_names if col in self.numeric_columns]
+            column_names = [col for col in column_names if col in self.numeric_columns_]
         
         iqr_dict={}
         for key, value in self.__iqr.items():
             if key in column_names:
                 iqr_dict[key]=value
         return pd.Series(iqr_dict)
 
@@ -161,23 +161,23 @@
             >>> outliers.fit(data)
             >>> outliers.get_limits()
             >>> outliers.get_limits(['age'], decimal=2)
 
         """
         
         if column_names is None:
-            column_names = self.numeric_columns
+            column_names = self.numeric_columns_
 
         elif not isinstance(column_names, list):
                 raise ValueError("column_names must be a list")
         for col in column_names:
-            if col not in self.numeric_columns:
+            if col not in self.numeric_columns_:
                 raise ValueError(f"Column name {col} does not exist or is not numerical")
         else:
-            column_names = [col for col in column_names if col in self.numeric_columns]
+            column_names = [col for col in column_names if col in self.numeric_columns_]
             
         limits = {}
         for name in column_names:
             try:
                 limits[name] = [round(self.__lower_limit_dict[name], decimal), round(self.__upper_limit_dict[name], decimal)]
             except KeyError:
                 return f"Column name {name} does not exist or is not numeric"
@@ -220,15 +220,15 @@
             >>> outliers.detect_outliers('age', styler=False)
 
         """
         
         if not isinstance(column_name, str):
                 raise ValueError("column_name must be a single string")
         
-        if column_name not in self.numeric_columns:
+        if column_name not in self.numeric_columns_:
             raise ValueError(f"Column name {column_name} does not exist or is not numerical")
 
     
         try:
             filtered_df = self.__data[(self.__data[column_name] < self.__lower_limit_dict[column_name]) |
                                     (self.__data[column_name] > self.__upper_limit_dict[column_name])]
 
@@ -280,23 +280,23 @@
             >>> outliers.fit(data)
             >>> outliers.get_outlier_count()
             >>> outliers.get_outlier_count(['age'])
 
         """
         
         if column_names is None:
-            column_names = self.numeric_columns
+            column_names = self.numeric_columns_
 
         elif not isinstance(column_names, list):
                 raise ValueError("column_names must be a list")
         for col in column_names:
-            if col not in self.numeric_columns:
+            if col not in self.numeric_columns_:
                 raise ValueError(f"Column name {col} does not exist or is not numerical")
         else:
-            column_names = [col for col in column_names if col in self.numeric_columns]
+            column_names = [col for col in column_names if col in self.numeric_columns_]
 
 
         outlier_counts = {}
         for name in column_names:
             filtered_df = self.detect_outliers(name, styler=False)
             if isinstance(filtered_df, pd.DataFrame):
                 outlier_counts[name] = filtered_df.shape[0]
@@ -347,23 +347,23 @@
             >>> from MGD_Outliers import Outliers
             >>> outliers = Outliers()
             >>> outliers.fit(data)
             >>> outliers.plot_outlier_count(column_names=['Age', 'Income'], figsize=(12, 6), threshold_percent=10)
         '''
         
         if column_names is None:
-            column_names = self.numeric_columns
+            column_names = self.numeric_columns_
 
         elif not isinstance(column_names, list):
                 raise ValueError("column_names must be a list")
         for col in column_names:
-            if col not in self.numeric_columns:
+            if col not in self.numeric_columns_:
                 raise ValueError(f"Column name {col} does not exist or is not numerical")
         else:
-            column_names = [col for col in column_names if col in self.numeric_columns]
+            column_names = [col for col in column_names if col in self.numeric_columns_]
 
         outlier_counts={}
         for name in column_names:
             filtered_df = self.detect_outliers(name, styler=False)
             if isinstance(filtered_df, pd.DataFrame):
                 outlier_counts[name] = filtered_df.shape[0]
 
@@ -414,22 +414,22 @@
             >>> outliers.drop_outliers(['age'])
             # Drop outliers from all numeric columns and return the updated DataFrame
             >>> outliers.drop_outliers()
 
         '''
 
         if column_names is None:
-            column_names=self.numeric_columns
+            column_names=self.numeric_columns_
         elif not isinstance(column_names, list):
                     raise ValueError("column_names must be a list")
         for col in column_names:
-            if col not in self.numeric_columns:
+            if col not in self.numeric_columns_:
                 raise ValueError(f"Column name {col} does not exist or is not numerical")
         else:
-            column_names = [col for col in column_names if col in self.numeric_columns]
+            column_names = [col for col in column_names if col in self.numeric_columns_]
 
         index=[]
 
         for name in column_names:
             filtered_df = self.detect_outliers(name, styler=False)
             if isinstance(filtered_df, pd.DataFrame):
                 index = index + list(filtered_df.index)
```

