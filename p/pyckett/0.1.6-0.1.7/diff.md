# Comparing `tmp/pyckett-0.1.6.tar.gz` & `tmp/pyckett-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyckett-0.1.6.tar", last modified: Tue Sep 20 15:31:15 2022, max compression
+gzip compressed data, was "pyckett-0.1.7.tar", last modified: Sun Apr 23 10:00:48 2023, max compression
```

## Comparing `pyckett-0.1.6.tar` & `pyckett-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,24 @@
-drwxrwxrwx   0        0        0        0 2022-09-20 15:31:15.487019 pyckett-0.1.6/
--rw-rw-rw-   0        0        0     1055 2022-09-20 15:18:29.000000 pyckett-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     2492 2022-09-20 15:31:15.487019 pyckett-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2053 2022-09-20 15:29:27.000000 pyckett-0.1.6/README.md
--rw-rw-rw-   0        0        0      568 2022-09-20 15:30:46.000000 pyckett-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-09-20 15:31:15.487019 pyckett-0.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-09-20 15:31:15.455770 pyckett-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2022-09-20 15:31:15.471394 pyckett-0.1.6/src/pyckett/
--rw-rw-rw-   0        0        0       22 2022-09-20 15:18:30.000000 pyckett-0.1.6/src/pyckett/__init__.py
--rw-rw-rw-   0        0        0    24510 2022-09-20 15:20:02.000000 pyckett-0.1.6/src/pyckett/pyckett.py
-drwxrwxrwx   0        0        0        0 2022-09-20 15:31:15.471394 pyckett-0.1.6/src/pyckett.egg-info/
--rw-rw-rw-   0        0        0     2492 2022-09-20 15:31:15.000000 pyckett-0.1.6/src/pyckett.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2022-09-20 15:31:15.000000 pyckett-0.1.6/src/pyckett.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-20 15:31:15.000000 pyckett-0.1.6/src/pyckett.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2022-09-20 15:31:15.000000 pyckett-0.1.6/src/pyckett.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-09-20 15:31:15.000000 pyckett-0.1.6/src/pyckett.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 10:00:48.322937 pyckett-0.1.7/
+-rw-rw-rw-   0        0        0     1055 2023-02-26 19:47:50.000000 pyckett-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     3221 2023-04-23 10:00:48.322937 pyckett-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2718 2023-04-23 09:56:22.000000 pyckett-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 10:00:48.300938 pyckett-0.1.7/pyckett/
+-rw-rw-rw-   0        0        0       23 2023-03-09 18:14:18.000000 pyckett-0.1.7/pyckett/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:00:48.320937 pyckett-0.1.7/pyckett/clitools/
+-rw-rw-rw-   0        0        0      176 2023-03-16 20:38:05.000000 pyckett-0.1.7/pyckett/clitools/__init__.py
+-rw-rw-rw-   0        0        0     7730 2023-04-02 19:00:27.000000 pyckett-0.1.7/pyckett/clitools/addparameters.py
+-rw-rw-rw-   0        0        0     7722 2023-04-04 09:42:11.000000 pyckett-0.1.7/pyckett/clitools/automaticfit.py
+-rw-rw-rw-   0        0        0     2625 2023-04-02 18:07:15.000000 pyckett-0.1.7/pyckett/clitools/omitparameters.py
+-rw-rw-rw-   0        0        0     2892 2023-03-09 18:36:05.000000 pyckett-0.1.7/pyckett/clitools/partitionfunction.py
+-rw-rw-rw-   0        0        0     4569 2023-04-04 09:37:24.000000 pyckett-0.1.7/pyckett/clitools/separatefits.py
+-rw-rw-rw-   0        0        0     2388 2023-04-05 08:23:32.000000 pyckett-0.1.7/pyckett/clitools/uncertainties.py
+-rw-rw-rw-   0        0        0    30442 2023-04-16 12:03:16.000000 pyckett-0.1.7/pyckett/pyckett.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:00:48.313937 pyckett-0.1.7/pyckett.egg-info/
+-rw-rw-rw-   0        0        0     3221 2023-04-23 10:00:48.000000 pyckett-0.1.7/pyckett.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      495 2023-04-23 10:00:48.000000 pyckett-0.1.7/pyckett.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 10:00:48.000000 pyckett-0.1.7/pyckett.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      326 2023-04-23 10:00:48.000000 pyckett-0.1.7/pyckett.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       24 2023-04-23 10:00:48.000000 pyckett-0.1.7/pyckett.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-23 10:00:48.000000 pyckett-0.1.7/pyckett.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      989 2023-04-23 10:00:23.000000 pyckett-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-23 10:00:48.322937 pyckett-0.1.7/setup.cfg
```

### Comparing `pyckett-0.1.6/LICENSE` & `pyckett-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyckett-0.1.6/PKG-INFO` & `pyckett-0.1.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,48 @@
 Metadata-Version: 2.1
 Name: pyckett
-Version: 0.1.6
+Version: 0.1.7
 Summary: A wrapper around Pickett's SPFIT and SPCAT
-Project-URL: Homepage, https://github.com/Ltotheois/Pyckett
-Keywords: Pickett,Spectroscopy
+Author-email: Luis Bonah <bonah@ph1.uni-koeln.de>
+Project-URL: Homepage, https://github.com/Ltotheois/Pyckett/
+Keywords: pickett,spectroscopy,spfit,spcat
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pyckett
 
 Pyckett is a python wrapper around the SPFIT/SPCAT package (*H. M. Pickett, "The Fitting and Prediction of Vibration-Rotation Spectra with Spin Interactions," **J. Mol. Spectrosc. 148,** 371-377 (1991)*).
 
 Install the package with pip by using the following command
 
 ```
 pip install pyckett
 ```
 
+# CLI Tools
+
+Pyckett provides a set of command line utilities which perform common steps of an iterative fitting process.
+
+*pyckett_add* helps adding new parameters to the fit, *pyckett_omit* is used for evaluating which parameters can be omitted.
+*pyckett_separatefits* can be used to separate a global fit into separate fits for each state.
+*pyckett_uncertainties* evaluates the uncertainties of the parameters.
+*pyckett_partitionfunction* calculates the partition function for different temperatures.
+*pyckett_auto* automatically builds up the Hamiltonian step by step.
+
+See the respective help functions (by adding *--help* after the command) to see their syntax.
+
 # Examples
 
 You can read files from the SPFIT/SPCAT universe with the following syntax
 
 ```python
-import pyckett
 var_dict = pyckett.parvar_to_dict(r"path/to/your/project/molecule.var")
 par_dict = pyckett.parvar_to_dict(r"path/to/your/project/molecule.par")
 int_dict = pyckett.int_to_dict(r"path/to/your/project/molecule.int")
 lin_df = pyckett.lin_to_df(r"path/to/your/project/molecule.lin")
 cat_df = pyckett.cat_to_df(r"path/to/your/project/molecule.cat")
 egy_df = pyckett.egy_to_df(r"path/to/your/project/molecule.egy")
 
@@ -44,26 +56,26 @@
 pyckett.add_parameter(par_dict, lin_df, cands, r"SPFIT_SPCAT")
 ```
 
 ## Best Candidate to neglect from Fit
 
 ```python
 cands = [320101, 230101]
-pyckett.ommit_parameter(par_dict, lin_df, cands, r"SPFIT_SPCAT")
+pyckett.omit_parameter(par_dict, lin_df, cands, r"SPFIT_SPCAT")
 ```
 
 ## Finalize cat file
 
 This function merges the cat and lin dataframes, sums up duplicate values in the cat file and allows to translate quantum numbers:
 
 ```python
 fin_cat_df, fin_lin_df = pyckett.finalize(cat_df, lin_df, qn_tdict, qn)
 ```
 
-## Find candidates for double-resonance measurement
+## Find candidates for double-resonance measurements
 
 This function finds possible transition arrangements for double-resonance measurements.
 Input two cat dataframes with the transitions that are in the range of your probe and pump source.
 
 ```python
 results_df = pyckett.get_dr_candidates(cat_df1, cat_df2)
 ```
```

### Comparing `pyckett-0.1.6/src/pyckett.egg-info/PKG-INFO` & `pyckett-0.1.7/pyckett.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,48 @@
 Metadata-Version: 2.1
 Name: pyckett
-Version: 0.1.6
+Version: 0.1.7
 Summary: A wrapper around Pickett's SPFIT and SPCAT
-Project-URL: Homepage, https://github.com/Ltotheois/Pyckett
-Keywords: Pickett,Spectroscopy
+Author-email: Luis Bonah <bonah@ph1.uni-koeln.de>
+Project-URL: Homepage, https://github.com/Ltotheois/Pyckett/
+Keywords: pickett,spectroscopy,spfit,spcat
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pyckett
 
 Pyckett is a python wrapper around the SPFIT/SPCAT package (*H. M. Pickett, "The Fitting and Prediction of Vibration-Rotation Spectra with Spin Interactions," **J. Mol. Spectrosc. 148,** 371-377 (1991)*).
 
 Install the package with pip by using the following command
 
 ```
 pip install pyckett
 ```
 
+# CLI Tools
+
+Pyckett provides a set of command line utilities which perform common steps of an iterative fitting process.
+
+*pyckett_add* helps adding new parameters to the fit, *pyckett_omit* is used for evaluating which parameters can be omitted.
+*pyckett_separatefits* can be used to separate a global fit into separate fits for each state.
+*pyckett_uncertainties* evaluates the uncertainties of the parameters.
+*pyckett_partitionfunction* calculates the partition function for different temperatures.
+*pyckett_auto* automatically builds up the Hamiltonian step by step.
+
+See the respective help functions (by adding *--help* after the command) to see their syntax.
+
 # Examples
 
 You can read files from the SPFIT/SPCAT universe with the following syntax
 
 ```python
-import pyckett
 var_dict = pyckett.parvar_to_dict(r"path/to/your/project/molecule.var")
 par_dict = pyckett.parvar_to_dict(r"path/to/your/project/molecule.par")
 int_dict = pyckett.int_to_dict(r"path/to/your/project/molecule.int")
 lin_df = pyckett.lin_to_df(r"path/to/your/project/molecule.lin")
 cat_df = pyckett.cat_to_df(r"path/to/your/project/molecule.cat")
 egy_df = pyckett.egy_to_df(r"path/to/your/project/molecule.egy")
 
@@ -44,26 +56,26 @@
 pyckett.add_parameter(par_dict, lin_df, cands, r"SPFIT_SPCAT")
 ```
 
 ## Best Candidate to neglect from Fit
 
 ```python
 cands = [320101, 230101]
-pyckett.ommit_parameter(par_dict, lin_df, cands, r"SPFIT_SPCAT")
+pyckett.omit_parameter(par_dict, lin_df, cands, r"SPFIT_SPCAT")
 ```
 
 ## Finalize cat file
 
 This function merges the cat and lin dataframes, sums up duplicate values in the cat file and allows to translate quantum numbers:
 
 ```python
 fin_cat_df, fin_lin_df = pyckett.finalize(cat_df, lin_df, qn_tdict, qn)
 ```
 
-## Find candidates for double-resonance measurement
+## Find candidates for double-resonance measurements
 
 This function finds possible transition arrangements for double-resonance measurements.
 Input two cat dataframes with the transitions that are in the range of your probe and pump source.
 
 ```python
 results_df = pyckett.get_dr_candidates(cat_df1, cat_df2)
 ```
```

