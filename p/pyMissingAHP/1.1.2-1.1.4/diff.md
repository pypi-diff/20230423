# Comparing `tmp/pyMissingAHP-1.1.2.tar.gz` & `tmp/pyMissingAHP-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyMissingAHP-1.1.2.tar", last modified: Fri Jan 13 20:13:25 2023, max compression
+gzip compressed data, was "dist\pyMissingAHP-1.1.4.tar", last modified: Sat Apr 22 22:35:19 2023, max compression
```

## Comparing `pyMissingAHP-1.1.2.tar` & `pyMissingAHP-1.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-01-13 20:13:25.000000 pyMissingAHP-1.1.2/
--rw-rw-rw-   0        0        0      668 2022-03-22 11:51:01.000000 pyMissingAHP-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     5527 2023-01-13 20:13:25.000000 pyMissingAHP-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     5116 2023-01-13 20:13:08.000000 pyMissingAHP-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-01-13 20:13:25.000000 pyMissingAHP-1.1.2/pyMissingAHP/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyMissingAHP-1.1.2/pyMissingAHP/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-13 20:13:25.000000 pyMissingAHP-1.1.2/pyMissingAHP/algorithm/
--rw-rw-rw-   0        0        0       26 2022-12-09 22:45:24.000000 pyMissingAHP-1.1.2/pyMissingAHP/algorithm/__init__.py
--rw-rw-rw-   0        0        0    36327 2022-12-15 13:33:03.000000 pyMissingAHP-1.1.2/pyMissingAHP/algorithm/src.py
-drwxrwxrwx   0        0        0        0 2023-01-13 20:13:25.000000 pyMissingAHP-1.1.2/pyMissingAHP/util/
--rw-rw-rw-   0        0        0      115 2022-12-14 14:13:58.000000 pyMissingAHP-1.1.2/pyMissingAHP/util/__init__.py
--rw-rw-rw-   0        0        0     1043 2020-08-25 19:15:07.000000 pyMissingAHP-1.1.2/pyMissingAHP/util/ahp.py
--rw-rw-rw-   0        0        0     1789 2022-03-24 20:40:39.000000 pyMissingAHP-1.1.2/pyMissingAHP/util/fuzzy_ahp.py
--rw-rw-rw-   0        0        0     6165 2022-10-13 19:13:26.000000 pyMissingAHP-1.1.2/pyMissingAHP/util/ga.py
--rw-rw-rw-   0        0        0    12079 2022-10-13 22:21:45.000000 pyMissingAHP-1.1.2/pyMissingAHP/util/u_n_iii.py
-drwxrwxrwx   0        0        0        0 2023-01-13 20:13:25.000000 pyMissingAHP-1.1.2/pyMissingAHP.egg-info/
--rw-rw-rw-   0        0        0     5527 2023-01-13 20:13:25.000000 pyMissingAHP-1.1.2/pyMissingAHP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2023-01-13 20:13:25.000000 pyMissingAHP-1.1.2/pyMissingAHP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-13 20:13:25.000000 pyMissingAHP-1.1.2/pyMissingAHP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-01-13 20:13:25.000000 pyMissingAHP-1.1.2/pyMissingAHP.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-01-13 20:13:25.000000 pyMissingAHP-1.1.2/pyMissingAHP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-01-13 20:13:25.000000 pyMissingAHP-1.1.2/pyMissingAHP.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-01-13 20:13:25.000000 pyMissingAHP-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      733 2023-01-13 20:12:38.000000 pyMissingAHP-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 22:35:19.000000 pyMissingAHP-1.1.4/
+-rw-rw-rw-   0        0        0      668 2022-03-22 11:51:01.000000 pyMissingAHP-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0     5504 2023-04-22 22:35:19.000000 pyMissingAHP-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5116 2023-01-13 20:13:08.000000 pyMissingAHP-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 22:35:19.000000 pyMissingAHP-1.1.4/pyMissingAHP/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyMissingAHP-1.1.4/pyMissingAHP/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 22:35:19.000000 pyMissingAHP-1.1.4/pyMissingAHP/algorithm/
+-rw-rw-rw-   0        0        0       26 2022-12-09 22:45:24.000000 pyMissingAHP-1.1.4/pyMissingAHP/algorithm/__init__.py
+-rw-rw-rw-   0        0        0    36335 2023-04-22 22:32:35.000000 pyMissingAHP-1.1.4/pyMissingAHP/algorithm/src.py
+drwxrwxrwx   0        0        0        0 2023-04-22 22:35:19.000000 pyMissingAHP-1.1.4/pyMissingAHP/util/
+-rw-rw-rw-   0        0        0      115 2022-12-14 14:13:58.000000 pyMissingAHP-1.1.4/pyMissingAHP/util/__init__.py
+-rw-rw-rw-   0        0        0     1079 2023-01-23 22:53:10.000000 pyMissingAHP-1.1.4/pyMissingAHP/util/ahp.py
+-rw-rw-rw-   0        0        0     1825 2023-01-23 22:53:23.000000 pyMissingAHP-1.1.4/pyMissingAHP/util/fuzzy_ahp.py
+-rw-rw-rw-   0        0        0     6165 2022-10-13 19:13:26.000000 pyMissingAHP-1.1.4/pyMissingAHP/util/ga.py
+-rw-rw-rw-   0        0        0    12079 2022-10-13 22:21:45.000000 pyMissingAHP-1.1.4/pyMissingAHP/util/u_n_iii.py
+drwxrwxrwx   0        0        0        0 2023-04-22 22:35:19.000000 pyMissingAHP-1.1.4/pyMissingAHP.egg-info/
+-rw-rw-rw-   0        0        0     5504 2023-04-22 22:35:18.000000 pyMissingAHP-1.1.4/pyMissingAHP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2023-04-22 22:35:18.000000 pyMissingAHP-1.1.4/pyMissingAHP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 22:35:18.000000 pyMissingAHP-1.1.4/pyMissingAHP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-04-22 22:35:18.000000 pyMissingAHP-1.1.4/pyMissingAHP.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-22 22:35:18.000000 pyMissingAHP-1.1.4/pyMissingAHP.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-22 22:35:18.000000 pyMissingAHP-1.1.4/pyMissingAHP.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-04-22 22:35:19.000000 pyMissingAHP-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      733 2023-04-22 22:34:06.000000 pyMissingAHP-1.1.4/setup.py
```

### Comparing `pyMissingAHP-1.1.2/LICENSE` & `pyMissingAHP-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyMissingAHP-1.1.2/PKG-INFO` & `pyMissingAHP-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pyMissingAHP
-Version: 1.1.2
+Version: 1.1.4
 Summary: A Method to Infer AHP Missing Pairwise Comparisons
 Home-page: https://github.com/Valdecy/pyMissingAHP
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyMissingAHP
 
 ## Introduction
 The multi-criteria technique Analytic Hierarchy Process (AHP) needs a complete Pairwise Comparison Matrix (PCM) to generate results. With an incomplete PCM, our algorithm can infer the best (continuous or discrete) values to complete the missing data. The values can be calculated based on the minimum inconsistency (f0), target rank preservation (f1), or both (f0_f1). The target rank preservation can be total (when all criteria are ranked) or partial (when only a set of criteria are ranked). We also allow ties in ranks (criteria with the same rank). For small problems with discrete scale, we offer a brute force method that can find all available solutions.
@@ -76,9 +75,7 @@
 
 3. Others
 
 - [pyDecision](https://github.com/Valdecy/pyDecision) - A library for many MCDA methods
 - [3MOAHP](https://github.com/Valdecy/Method_3MOAHP) - Inconsistency Reduction Technique for AHP and Fuzzy-AHP Methods
 - [ELECTRE-Tree](https://github.com/Valdecy/ELECTRE-Tree) - Algorithm to infer the ELECTRE Tri-B method parameters
 - [Ranking-Trees](https://github.com/Valdecy/Ranking-Trees) - Algorithm to infer the ELECTRE II, III, IV and PROMETHEE I, II, III, IV method parameters
-
-
```

### Comparing `pyMissingAHP-1.1.2/README.md` & `pyMissingAHP-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyMissingAHP-1.1.2/pyMissingAHP/algorithm/src.py` & `pyMissingAHP-1.1.4/pyMissingAHP/algorithm/src.py`

 * *Files 0% similar despite different names*

```diff
@@ -539,15 +539,15 @@
         for i in range(0, w1.shape[0]):
             if (i <= len(self.order)):
                 if (self.order[i] != -1):
                     w2.append(self.order[i])
                 else:
                     w2.append(w1[i])
             else:
-                w2.append(w1[i])
+                w2.append(len(self.order))
         w2             = np.array(w2)
         kendall_tau, _ = stats.kendalltau(w1, w2)
         if (math.isnan(kendall_tau)):
             kendall_tau = -1
         return -kendall_tau
 
     # Function: Objective Function 1 - Kendall Tau (KT) Solutions from Brute Force  
@@ -568,15 +568,15 @@
         kendall_tau, _ = stats.kendalltau(w1, w2)
         if (math.isnan(kendall_tau)):
             kendall_tau = -1
         return kendall_tau    
 
     # Function: MultiObjective Function - Consistency Ratio (MI) & Kendall Tau (KT)
     def f0_f1(self, variables):
-        result = self.alpha*self.f0(variables)/1 + (1 - self.alpha)*self.f1(variables)/10
+        result = self.alpha*self.f0(variables)/1 + (1 - self.alpha)*self.f1(variables)/1
         return result
         
     ################################################################################
 
     # Function: GA
     def run(self):
         self.solution = genetic_algorithm(target_function = self.lof[0],
@@ -590,15 +590,15 @@
                                           eta             = self.eta,
                                           verbose         = self.vbs
                                           )
         return self.solution
 
     ################################################################################
 
-    # Function: Get Solutions
+    # Function: Get Solution
     def get_solution(self):
         self.indicators = []
         self.solutions  = []
         category        = 'inconsistent'
         count_con       = 0
         count_inc       = 0
         sol             = self.solution[0:int( ( (self.dataset.shape[0]**2 - self.dataset.shape[0])/2 ) + 1)]
```

### Comparing `pyMissingAHP-1.1.2/pyMissingAHP/util/fuzzy_ahp.py` & `pyMissingAHP-1.1.4/pyMissingAHP/util/fuzzy_ahp.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     X       = [(item[0] + 4*item[1] + item[2])/6 for i in range(0, len(data)) for item in data[i] ]
     X       = np.asarray(X)
     X       = np.reshape(X, (len(data), len(data)))
     row_sum = []
     s_row   = []
     f_w     = []
     d_w     = []
-    inc_rat = np.array([0, 0, 0, 0.58, 0.9, 1.12, 1.24, 1.32, 1.41, 1.45])
+    inc_rat = np.array([0, 0, 0, 0.58, 0.9, 1.12, 1.24, 1.32, 1.41, 1.45, 1.49, 1.51, 1.48, 1.56, 1.57, 1.59])
     for i in range(0, len(data)):
         a, b, c = 1, 1, 1
         for j in range(0, len(data[i])):
             d, e, f = data[i][j]
             a, b, c = a*d, b*e, c*f
         row_sum.append( (a, b, c) )
     L, M, U = 0, 0, 0
```

### Comparing `pyMissingAHP-1.1.2/pyMissingAHP/util/ga.py` & `pyMissingAHP-1.1.4/pyMissingAHP/util/ga.py`

 * *Files identical despite different names*

### Comparing `pyMissingAHP-1.1.2/pyMissingAHP/util/u_n_iii.py` & `pyMissingAHP-1.1.4/pyMissingAHP/util/u_n_iii.py`

 * *Files identical despite different names*

### Comparing `pyMissingAHP-1.1.2/pyMissingAHP.egg-info/PKG-INFO` & `pyMissingAHP-1.1.4/pyMissingAHP.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pyMissingAHP
-Version: 1.1.2
+Version: 1.1.4
 Summary: A Method to Infer AHP Missing Pairwise Comparisons
 Home-page: https://github.com/Valdecy/pyMissingAHP
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyMissingAHP
 
 ## Introduction
 The multi-criteria technique Analytic Hierarchy Process (AHP) needs a complete Pairwise Comparison Matrix (PCM) to generate results. With an incomplete PCM, our algorithm can infer the best (continuous or discrete) values to complete the missing data. The values can be calculated based on the minimum inconsistency (f0), target rank preservation (f1), or both (f0_f1). The target rank preservation can be total (when all criteria are ranked) or partial (when only a set of criteria are ranked). We also allow ties in ranks (criteria with the same rank). For small problems with discrete scale, we offer a brute force method that can find all available solutions.
@@ -76,9 +75,7 @@
 
 3. Others
 
 - [pyDecision](https://github.com/Valdecy/pyDecision) - A library for many MCDA methods
 - [3MOAHP](https://github.com/Valdecy/Method_3MOAHP) - Inconsistency Reduction Technique for AHP and Fuzzy-AHP Methods
 - [ELECTRE-Tree](https://github.com/Valdecy/ELECTRE-Tree) - Algorithm to infer the ELECTRE Tri-B method parameters
 - [Ranking-Trees](https://github.com/Valdecy/Ranking-Trees) - Algorithm to infer the ELECTRE II, III, IV and PROMETHEE I, II, III, IV method parameters
-
-
```

### Comparing `pyMissingAHP-1.1.2/setup.py` & `pyMissingAHP-1.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='pyMissingAHP',
-    version='1.1.2',
+    version='1.1.4',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/pyMissingAHP',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
```

