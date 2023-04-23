# Comparing `tmp/evalAIRR-0.0.8.tar.gz` & `tmp/evalAIRR-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evalAIRR-0.0.8.tar", last modified: Sun Feb  5 22:54:00 2023, max compression
+gzip compressed data, was "evalAIRR-0.0.9.tar", last modified: Mon Feb 13 23:19:00 2023, max compression
```

## Comparing `evalAIRR-0.0.8.tar` & `evalAIRR-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 22:54:00.413193 evalAIRR-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-02-05 22:54:00.413193 evalAIRR-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7408 2023-02-05 22:53:46.000000 evalAIRR-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 22:54:00.409193 evalAIRR-0.0.8/evalAIRR/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-05 22:53:47.000000 evalAIRR-0.0.8/evalAIRR/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-02-05 22:53:47.000000 evalAIRR-0.0.8/evalAIRR/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 22:54:00.413193 evalAIRR-0.0.8/evalAIRR/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-05 22:53:47.000000 evalAIRR-0.0.8/evalAIRR/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-02-05 22:53:47.000000 evalAIRR-0.0.8/evalAIRR/util/copula.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-02-05 22:53:47.000000 evalAIRR-0.0.8/evalAIRR/util/corr.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-02-05 22:53:47.000000 evalAIRR-0.0.8/evalAIRR/util/input.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-05 22:53:47.000000 evalAIRR-0.0.8/evalAIRR/util/ml.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-02-05 22:53:47.000000 evalAIRR-0.0.8/evalAIRR/util/pca.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-02-05 22:53:47.000000 evalAIRR-0.0.8/evalAIRR/util/report.py
--rw-r--r--   0 runner    (1001) docker     (123)    17560 2023-02-05 22:53:47.000000 evalAIRR-0.0.8/evalAIRR/util/univar.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-05 22:53:47.000000 evalAIRR-0.0.8/evalAIRR/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 22:54:00.413193 evalAIRR-0.0.8/evalAIRR.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-02-05 22:54:00.000000 evalAIRR-0.0.8/evalAIRR.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-02-05 22:54:00.000000 evalAIRR-0.0.8/evalAIRR.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-05 22:54:00.000000 evalAIRR-0.0.8/evalAIRR.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-05 22:54:00.000000 evalAIRR-0.0.8/evalAIRR.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-05 22:54:00.000000 evalAIRR-0.0.8/evalAIRR.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-05 22:54:00.413193 evalAIRR-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-02-05 22:53:47.000000 evalAIRR-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-13 23:19:00.635579 evalAIRR-0.0.9/
+-rw-rw-rw-   0        0        0     8489 2023-02-13 23:19:00.630581 evalAIRR-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     7565 2023-02-05 22:22:19.000000 evalAIRR-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-02-13 23:19:00.495577 evalAIRR-0.0.9/evalAIRR/
+-rw-rw-rw-   0        0        0        0 2023-02-05 21:33:51.000000 evalAIRR-0.0.9/evalAIRR/__init__.py
+-rw-rw-rw-   0        0        0     8768 2023-02-13 23:14:49.000000 evalAIRR-0.0.9/evalAIRR/main.py
+drwxrwxrwx   0        0        0        0 2023-02-13 23:19:00.622578 evalAIRR-0.0.9/evalAIRR/util/
+-rw-rw-rw-   0        0        0        0 2023-02-05 21:39:17.000000 evalAIRR-0.0.9/evalAIRR/util/__init__.py
+-rw-rw-rw-   0        0        0     4590 2023-02-05 21:47:45.000000 evalAIRR-0.0.9/evalAIRR/util/copula.py
+-rw-rw-rw-   0        0        0     1682 2023-02-05 21:47:21.000000 evalAIRR-0.0.9/evalAIRR/util/corr.py
+-rw-rw-rw-   0        0        0      579 2023-02-05 20:14:10.000000 evalAIRR-0.0.9/evalAIRR/util/input.py
+-rw-rw-rw-   0        0        0      437 2023-02-13 23:11:22.000000 evalAIRR-0.0.9/evalAIRR/util/ml.py
+-rw-rw-rw-   0        0        0      830 2023-02-05 20:14:10.000000 evalAIRR-0.0.9/evalAIRR/util/pca.py
+-rw-rw-rw-   0        0        0     3117 2023-02-05 20:14:10.000000 evalAIRR-0.0.9/evalAIRR/util/report.py
+-rw-rw-rw-   0        0        0    17946 2023-02-05 20:14:10.000000 evalAIRR-0.0.9/evalAIRR/util/univar.py
+-rw-rw-rw-   0        0        0       19 2023-02-06 10:26:39.000000 evalAIRR-0.0.9/evalAIRR/version.py
+drwxrwxrwx   0        0        0        0 2023-02-13 23:19:00.524577 evalAIRR-0.0.9/evalAIRR.egg-info/
+-rw-rw-rw-   0        0        0     8489 2023-02-13 23:19:00.000000 evalAIRR-0.0.9/evalAIRR.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      423 2023-02-13 23:19:00.000000 evalAIRR-0.0.9/evalAIRR.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-13 23:19:00.000000 evalAIRR-0.0.9/evalAIRR.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-02-13 23:19:00.000000 evalAIRR-0.0.9/evalAIRR.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-02-13 23:19:00.000000 evalAIRR-0.0.9/evalAIRR.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-02-13 23:19:00.635579 evalAIRR-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1288 2023-02-05 22:52:39.000000 evalAIRR-0.0.9/setup.py
```

### Comparing `evalAIRR-0.0.8/PKG-INFO` & `evalAIRR-0.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,177 +1,181 @@
-Metadata-Version: 2.1
-Name: evalAIRR
-Version: 0.0.8
-Summary: Comparison of real and simulated AIRR datasets
-Author: Lukas Sparnauskas
-Author-email: <lukas.11sp@gmail.com>
-License: MIT
-Keywords: python,airr,simulated data,ml,machine learning
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Environment :: Console
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-
-
-# evalAIRR
-
-A tool that allows comparison of real and simulated datasets by providing different statistical indicators and dataset visualizations in one report.
-
-## Installation
-
-It is recommended to use a virtual python environment to run evalAIRR if another python environment is used. Here is a quick guide on how you can set up a virtual environment:
-
-`https://docs.python.org/3/tutorial/venv.html#creating-virtual-environments`
-
-### Install using pip
-
-Run this command to install the evalAIRR package:
-
-`pip install evalairr`
-
-## Quickstart
-
-evalAIRR uses a YAML file for configuration. If you are unfamiliar with how YAML files are structured, read this guide to the syntax:
-
-`https://docs.fileformat.com/programming/yaml/#syntax`
-
-This is the stucture of a sample report configuration file you can use to start off with (it is included in the repository location ./yaml_files/quickstart.yaml):
-
-```
-datasets:
-  real:
-    path: ./data/encoded_real_1000_200.csv
-  sim:
-    path: ./data/encoded_sim_1000_200.csv
-reports:
-  feature_based:
-    report1:
-      features:
-        - TGT
-        - ANV
-      report_types:
-        - ks
-        - distr_densityplot
-output:
-  path: './output/report.html'
-
-```
-
-This report will process the two provided datasets (real and simulated), and create an HTML report with feature-based report types - Kolmogorov–Smirnov test (indicated by `ks`) and a feature distribution density plot (indicated by `distr_densityplot`) for the features `TGT` and `ANV`. It will then export the report to the path `./output/report.html`. More details on what reports can be created can be found in the *YAML Configuration Guidelines* secion.
-
-You can run the program by running this command within the installation directory:
-
-`evalairr -i ./yaml_files/quickstart.yaml`
-
-The report will be generated in the specified output path in the configuration file or, if a specific path is not provided, in `<CURRENT_DIRECTORY>/output/report.html`. The report is exported in the HTML format.
-
-## YAML Configuration Guidelines
-
-The configuration YAML file consists of 3 main sections: `datasets`, `reports` and `output`.
-
-### Datasets
-
-In the `datasets` section, you have to provide paths to a real and a simulated datasets that you are comparing. This can be done by specifying the file path of each file in the `path` variable under the sections `real` and `sim` respectively. Here is an example of how a configured `datasets` section looks like:
-
-```
-datasets:
-  real:
-    path: ./data/encoded_real_1000_200.csv
-  sim:
-    path: ./data/encoded_sim_1000_200.csv
-```
-
-### Reports
-
-In the `reports` section, you can provide the list of report types you want to create and their parameters. There are three types of report groups depending on the different parameters: `feature_based`, `observation_based` and `generic`. Here is the list of reports you can create that compare the features of the real dataset with the simulated dataset:
-
-#### Feature-based reports
-- `ks` - Kolmogorov–Smirnov statistic. Parameters: list of features you are creating the report for.
-- `distr_histogram` - feature distribution histogram. Parameters: list of features you are creating the report for.
-- `distr_boxplot` - feature distribution boxplot. Parameters: list of features you are creating the report for.
-- `distr_violinplot` - feature distribution violin plot. Parameters: list of features you are creating the report for.
-- `distr_densityplot` - feature distribution density plot. Parameters: list of features you are creating the report for.
-- `distance` - Euclidean distance between the real and simulated feature. Parameters: list of features you are creating the report for.
-- `statistics` - statistical indicators (average, median, standard deviation and variance) of a feature in both real and simulated datasets. Parameters: list of features you are creating the report for.
-
-#### Observation-based reports
-- `observation_distr_histogram` - observation distribution histogram. Parameters: list of observations you are creating the report for.
-- `observation_distr_boxplot` - observation distribution boxplot. Parameters: list of observations you are creating the report for.
-- `observation_distr_violinplot` - observation distribution violin plot. Parameters: list of observations you are creating the report for.
-- `observation_distr_densityplot` - observation distribution density plot. Parameters: list of observations you are creating the report for. The observation index 'all' can be used to report on all observations in one plot.
-- `observation_distance` - Euclidean distance between the real and simulated observation. Parameters: list of observations you are creating the report for.
-- `observation_statistics` - statistical indicators (average, median, standard deviation and variance) of an observation in both real and simulated datasets. Parameters: list of observations you are creating the report for.
-
-#### General reports
-- `copula_2d` - a 2D scatter plot that displays two features in a Gausian Multivariate copula space. Parameters: a report section of any name, under which the compared features are specified.
-- `copula_3d` - a 3D scatter plot that displays three features in a Gausian Multivariate copula space. Parameters: a report section of any name, under which the compared features are specified.
-- `feature_average_vs_variance` - a scatter plot that displays the average value of every feature on one axis and the variance of every feature on the other axis.
-- `observation_average_vs_variance` - a scatter plot that displays the average value of every observation on one axis and the variance of every observation on the other axis.
-- `corr` - correlation matrix heatmaps of the real and simulated datasets. Parameters: `percent_features` - an optional parameter for dimensionality reduction using PCA. A float value corresponding with the ratio of feature reduction (e.g. `percent_features` equal to 0.5 would reduce the feature count by half). 
-- `pca_2d` - two scatter plots with both datasets reduced to two dimensions using PCA.
-
-Here is a sample `reports` section of a configuration file containing all of the reports:
-
-```
-reports:
-  feature_based:
-    report1:
-      features:
-        - TGT
-        - ANV
-      report_types:
-        - ks
-        - distr_histogram
-        - distr_boxplot
-        - distr_violinplot
-        - distr_densityplot
-        - distance
-        - statistics
-  observation_based:
-    report1:
-      observations:
-        - 0
-      report_types:
-        - observation_distr_histogram
-        - observation_distr_boxplot
-        - observation_distr_violinplot
-        - observation_distr_densityplot
-        - observation_distance
-        - observation_statistics
-    report2:
-      observations:
-        - all
-      report_types:
-        - observation_distr_densityplot
-  general:
-    copula_2d:
-      report1:
-        - TGT
-        - ANV
-    copula_3d:
-      report1:
-        - TGT
-        - ANV
-        - CAS
-    feature_average_vs_variance:
-    observation_average_vs_variance:
-    corr:
-      percent_features: 0.6
-    pca_2d:
-```
-
-### Output
-
-An optional section where you can specify the file path of the generated report. The default path of the generated report is `<INSTALL_DIRECTORY>/output/report.html`. The report is exported in the HTML format.
-
-An example output section:
-
-```
-output:
-  path: './output/report.html'
-```
+Metadata-Version: 2.1
+Name: evalAIRR
+Version: 0.0.9
+Summary: Comparison of real and simulated AIRR datasets
+Home-page: UNKNOWN
+Author: Lukas Sparnauskas
+Author-email: <lukas.11sp@gmail.com>
+License: MIT
+Keywords: python,airr,simulated data,ml,machine learning
+Platform: UNKNOWN
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Environment :: Console
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+
+
+# evalAIRR
+
+A tool that allows comparison of real and simulated datasets by providing different statistical indicators and dataset visualizations in one report.
+
+## Installation
+
+It is recommended to use a virtual python environment to run evalAIRR if another python environment is used. Here is a quick guide on how you can set up a virtual environment:
+
+`https://docs.python.org/3/tutorial/venv.html#creating-virtual-environments`
+
+### Install using pip
+
+Run this command to install the evalAIRR package:
+
+`pip install evalairr`
+
+## Quickstart
+
+evalAIRR uses a YAML file for configuration. If you are unfamiliar with how YAML files are structured, read this guide to the syntax:
+
+`https://docs.fileformat.com/programming/yaml/#syntax`
+
+This is the stucture of a sample report configuration file you can use to start off with (it is included in the repository location ./yaml_files/quickstart.yaml):
+
+```
+datasets:
+  real:
+    path: ./data/encoded_real_1000_200.csv
+  sim:
+    path: ./data/encoded_sim_1000_200.csv
+reports:
+  feature_based:
+    report1:
+      features:
+        - TGT
+        - ANV
+      report_types:
+        - ks
+        - distr_densityplot
+output:
+  path: './output/report.html'
+
+```
+
+This report will process the two provided datasets (real and simulated), and create an HTML report with feature-based report types - Kolmogorov–Smirnov test (indicated by `ks`) and a feature distribution density plot (indicated by `distr_densityplot`) for the features `TGT` and `ANV`. It will then export the report to the path `./output/report.html`. More details on what reports can be created can be found in the *YAML Configuration Guidelines* secion.
+
+You can run the program by running this command within the installation directory:
+
+`evalairr -i ./yaml_files/quickstart.yaml`
+
+The report will be generated in the specified output path in the configuration file or, if a specific path is not provided, in `<CURRENT_DIRECTORY>/output/report.html`. The report is exported in the HTML format.
+
+## YAML Configuration Guidelines
+
+The configuration YAML file consists of 3 main sections: `datasets`, `reports` and `output`.
+
+### Datasets
+
+In the `datasets` section, you have to provide paths to a real and a simulated datasets that you are comparing. This can be done by specifying the file path of each file in the `path` variable under the sections `real` and `sim` respectively. Here is an example of how a configured `datasets` section looks like:
+
+```
+datasets:
+  real:
+    path: ./data/encoded_real_1000_200.csv
+  sim:
+    path: ./data/encoded_sim_1000_200.csv
+```
+
+### Reports
+
+In the `reports` section, you can provide the list of report types you want to create and their parameters. There are three types of report groups depending on the different parameters: `feature_based`, `observation_based` and `generic`. Here is the list of reports you can create that compare the features of the real dataset with the simulated dataset:
+
+#### Feature-based reports
+- `ks` - Kolmogorov–Smirnov statistic. Parameters: list of features you are creating the report for.
+- `distr_histogram` - feature distribution histogram. Parameters: list of features you are creating the report for.
+- `distr_boxplot` - feature distribution boxplot. Parameters: list of features you are creating the report for.
+- `distr_violinplot` - feature distribution violin plot. Parameters: list of features you are creating the report for.
+- `distr_densityplot` - feature distribution density plot. Parameters: list of features you are creating the report for.
+- `distance` - Euclidean distance between the real and simulated feature. Parameters: list of features you are creating the report for.
+- `statistics` - statistical indicators (average, median, standard deviation and variance) of a feature in both real and simulated datasets. Parameters: list of features you are creating the report for.
+
+#### Observation-based reports
+- `observation_distr_histogram` - observation distribution histogram. Parameters: list of observations you are creating the report for.
+- `observation_distr_boxplot` - observation distribution boxplot. Parameters: list of observations you are creating the report for.
+- `observation_distr_violinplot` - observation distribution violin plot. Parameters: list of observations you are creating the report for.
+- `observation_distr_densityplot` - observation distribution density plot. Parameters: list of observations you are creating the report for. The observation index 'all' can be used to report on all observations in one plot.
+- `observation_distance` - Euclidean distance between the real and simulated observation. Parameters: list of observations you are creating the report for.
+- `observation_statistics` - statistical indicators (average, median, standard deviation and variance) of an observation in both real and simulated datasets. Parameters: list of observations you are creating the report for.
+
+#### General reports
+- `copula_2d` - a 2D scatter plot that displays two features in a Gausian Multivariate copula space. Parameters: a report section of any name, under which the compared features are specified.
+- `copula_3d` - a 3D scatter plot that displays three features in a Gausian Multivariate copula space. Parameters: a report section of any name, under which the compared features are specified.
+- `feature_average_vs_variance` - a scatter plot that displays the average value of every feature on one axis and the variance of every feature on the other axis.
+- `observation_average_vs_variance` - a scatter plot that displays the average value of every observation on one axis and the variance of every observation on the other axis.
+- `corr` - correlation matrix heatmaps of the real and simulated datasets. Parameters: `percent_features` - an optional parameter for dimensionality reduction using PCA. A float value corresponding with the ratio of feature reduction (e.g. `percent_features` equal to 0.5 would reduce the feature count by half). 
+- `pca_2d` - two scatter plots with both datasets reduced to two dimensions using PCA.
+
+Here is a sample `reports` section of a configuration file containing all of the reports:
+
+```
+reports:
+  feature_based:
+    report1:
+      features:
+        - TGT
+        - ANV
+      report_types:
+        - ks
+        - distr_histogram
+        - distr_boxplot
+        - distr_violinplot
+        - distr_densityplot
+        - distance
+        - statistics
+  observation_based:
+    report1:
+      observations:
+        - 0
+      report_types:
+        - observation_distr_histogram
+        - observation_distr_boxplot
+        - observation_distr_violinplot
+        - observation_distr_densityplot
+        - observation_distance
+        - observation_statistics
+    report2:
+      observations:
+        - all
+      report_types:
+        - observation_distr_densityplot
+  general:
+    copula_2d:
+      report1:
+        - TGT
+        - ANV
+    copula_3d:
+      report1:
+        - TGT
+        - ANV
+        - CAS
+    feature_average_vs_variance:
+    observation_average_vs_variance:
+    corr:
+      percent_features: 0.6
+    pca_2d:
+```
+
+### Output
+
+An optional section where you can specify the file path of the generated report. The default path of the generated report is `<INSTALL_DIRECTORY>/output/report.html`. The report is exported in the HTML format.
+
+An example output section:
+
+```
+output:
+  path: './output/report.html'
+```
+
+
```

### Comparing `evalAIRR-0.0.8/README.md` & `evalAIRR-0.0.9/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,157 +1,157 @@
-# evalAIRR
-
-A tool that allows comparison of real and simulated datasets by providing different statistical indicators and dataset visualizations in one report.
-
-## Installation
-
-It is recommended to use a virtual python environment to run evalAIRR if another python environment is used. Here is a quick guide on how you can set up a virtual environment:
-
-`https://docs.python.org/3/tutorial/venv.html#creating-virtual-environments`
-
-### Install using pip
-
-Run this command to install the evalAIRR package:
-
-`pip install evalairr`
-
-## Quickstart
-
-evalAIRR uses a YAML file for configuration. If you are unfamiliar with how YAML files are structured, read this guide to the syntax:
-
-`https://docs.fileformat.com/programming/yaml/#syntax`
-
-This is the stucture of a sample report configuration file you can use to start off with (it is included in the repository location ./yaml_files/quickstart.yaml):
-
-```
-datasets:
-  real:
-    path: ./data/encoded_real_1000_200.csv
-  sim:
-    path: ./data/encoded_sim_1000_200.csv
-reports:
-  feature_based:
-    report1:
-      features:
-        - TGT
-        - ANV
-      report_types:
-        - ks
-        - distr_densityplot
-output:
-  path: './output/report.html'
-
-```
-
-This report will process the two provided datasets (real and simulated), and create an HTML report with feature-based report types - Kolmogorov–Smirnov test (indicated by `ks`) and a feature distribution density plot (indicated by `distr_densityplot`) for the features `TGT` and `ANV`. It will then export the report to the path `./output/report.html`. More details on what reports can be created can be found in the *YAML Configuration Guidelines* secion.
-
-You can run the program by running this command within the installation directory:
-
-`evalairr -i ./yaml_files/quickstart.yaml`
-
-The report will be generated in the specified output path in the configuration file or, if a specific path is not provided, in `<CURRENT_DIRECTORY>/output/report.html`. The report is exported in the HTML format.
-
-## YAML Configuration Guidelines
-
-The configuration YAML file consists of 3 main sections: `datasets`, `reports` and `output`.
-
-### Datasets
-
-In the `datasets` section, you have to provide paths to a real and a simulated datasets that you are comparing. This can be done by specifying the file path of each file in the `path` variable under the sections `real` and `sim` respectively. Here is an example of how a configured `datasets` section looks like:
-
-```
-datasets:
-  real:
-    path: ./data/encoded_real_1000_200.csv
-  sim:
-    path: ./data/encoded_sim_1000_200.csv
-```
-
-### Reports
-
-In the `reports` section, you can provide the list of report types you want to create and their parameters. There are three types of report groups depending on the different parameters: `feature_based`, `observation_based` and `generic`. Here is the list of reports you can create that compare the features of the real dataset with the simulated dataset:
-
-#### Feature-based reports
-- `ks` - Kolmogorov–Smirnov statistic. Parameters: list of features you are creating the report for.
-- `distr_histogram` - feature distribution histogram. Parameters: list of features you are creating the report for.
-- `distr_boxplot` - feature distribution boxplot. Parameters: list of features you are creating the report for.
-- `distr_violinplot` - feature distribution violin plot. Parameters: list of features you are creating the report for.
-- `distr_densityplot` - feature distribution density plot. Parameters: list of features you are creating the report for.
-- `distance` - Euclidean distance between the real and simulated feature. Parameters: list of features you are creating the report for.
-- `statistics` - statistical indicators (average, median, standard deviation and variance) of a feature in both real and simulated datasets. Parameters: list of features you are creating the report for.
-
-#### Observation-based reports
-- `observation_distr_histogram` - observation distribution histogram. Parameters: list of observations you are creating the report for.
-- `observation_distr_boxplot` - observation distribution boxplot. Parameters: list of observations you are creating the report for.
-- `observation_distr_violinplot` - observation distribution violin plot. Parameters: list of observations you are creating the report for.
-- `observation_distr_densityplot` - observation distribution density plot. Parameters: list of observations you are creating the report for. The observation index 'all' can be used to report on all observations in one plot.
-- `observation_distance` - Euclidean distance between the real and simulated observation. Parameters: list of observations you are creating the report for.
-- `observation_statistics` - statistical indicators (average, median, standard deviation and variance) of an observation in both real and simulated datasets. Parameters: list of observations you are creating the report for.
-
-#### General reports
-- `copula_2d` - a 2D scatter plot that displays two features in a Gausian Multivariate copula space. Parameters: a report section of any name, under which the compared features are specified.
-- `copula_3d` - a 3D scatter plot that displays three features in a Gausian Multivariate copula space. Parameters: a report section of any name, under which the compared features are specified.
-- `feature_average_vs_variance` - a scatter plot that displays the average value of every feature on one axis and the variance of every feature on the other axis.
-- `observation_average_vs_variance` - a scatter plot that displays the average value of every observation on one axis and the variance of every observation on the other axis.
-- `corr` - correlation matrix heatmaps of the real and simulated datasets. Parameters: `percent_features` - an optional parameter for dimensionality reduction using PCA. A float value corresponding with the ratio of feature reduction (e.g. `percent_features` equal to 0.5 would reduce the feature count by half). 
-- `pca_2d` - two scatter plots with both datasets reduced to two dimensions using PCA.
-
-Here is a sample `reports` section of a configuration file containing all of the reports:
-
-```
-reports:
-  feature_based:
-    report1:
-      features:
-        - TGT
-        - ANV
-      report_types:
-        - ks
-        - distr_histogram
-        - distr_boxplot
-        - distr_violinplot
-        - distr_densityplot
-        - distance
-        - statistics
-  observation_based:
-    report1:
-      observations:
-        - 0
-      report_types:
-        - observation_distr_histogram
-        - observation_distr_boxplot
-        - observation_distr_violinplot
-        - observation_distr_densityplot
-        - observation_distance
-        - observation_statistics
-    report2:
-      observations:
-        - all
-      report_types:
-        - observation_distr_densityplot
-  general:
-    copula_2d:
-      report1:
-        - TGT
-        - ANV
-    copula_3d:
-      report1:
-        - TGT
-        - ANV
-        - CAS
-    feature_average_vs_variance:
-    observation_average_vs_variance:
-    corr:
-      percent_features: 0.6
-    pca_2d:
-```
-
-### Output
-
-An optional section where you can specify the file path of the generated report. The default path of the generated report is `<INSTALL_DIRECTORY>/output/report.html`. The report is exported in the HTML format.
-
-An example output section:
-
-```
-output:
-  path: './output/report.html'
-```
+# evalAIRR
+
+A tool that allows comparison of real and simulated datasets by providing different statistical indicators and dataset visualizations in one report.
+
+## Installation
+
+It is recommended to use a virtual python environment to run evalAIRR if another python environment is used. Here is a quick guide on how you can set up a virtual environment:
+
+`https://docs.python.org/3/tutorial/venv.html#creating-virtual-environments`
+
+### Install using pip
+
+Run this command to install the evalAIRR package:
+
+`pip install evalairr`
+
+## Quickstart
+
+evalAIRR uses a YAML file for configuration. If you are unfamiliar with how YAML files are structured, read this guide to the syntax:
+
+`https://docs.fileformat.com/programming/yaml/#syntax`
+
+This is the stucture of a sample report configuration file you can use to start off with (it is included in the repository location ./yaml_files/quickstart.yaml):
+
+```
+datasets:
+  real:
+    path: ./data/encoded_real_1000_200.csv
+  sim:
+    path: ./data/encoded_sim_1000_200.csv
+reports:
+  feature_based:
+    report1:
+      features:
+        - TGT
+        - ANV
+      report_types:
+        - ks
+        - distr_densityplot
+output:
+  path: './output/report.html'
+
+```
+
+This report will process the two provided datasets (real and simulated), and create an HTML report with feature-based report types - Kolmogorov–Smirnov test (indicated by `ks`) and a feature distribution density plot (indicated by `distr_densityplot`) for the features `TGT` and `ANV`. It will then export the report to the path `./output/report.html`. More details on what reports can be created can be found in the *YAML Configuration Guidelines* secion.
+
+You can run the program by running this command within the installation directory:
+
+`evalairr -i ./yaml_files/quickstart.yaml`
+
+The report will be generated in the specified output path in the configuration file or, if a specific path is not provided, in `<CURRENT_DIRECTORY>/output/report.html`. The report is exported in the HTML format.
+
+## YAML Configuration Guidelines
+
+The configuration YAML file consists of 3 main sections: `datasets`, `reports` and `output`.
+
+### Datasets
+
+In the `datasets` section, you have to provide paths to a real and a simulated datasets that you are comparing. This can be done by specifying the file path of each file in the `path` variable under the sections `real` and `sim` respectively. Here is an example of how a configured `datasets` section looks like:
+
+```
+datasets:
+  real:
+    path: ./data/encoded_real_1000_200.csv
+  sim:
+    path: ./data/encoded_sim_1000_200.csv
+```
+
+### Reports
+
+In the `reports` section, you can provide the list of report types you want to create and their parameters. There are three types of report groups depending on the different parameters: `feature_based`, `observation_based` and `generic`. Here is the list of reports you can create that compare the features of the real dataset with the simulated dataset:
+
+#### Feature-based reports
+- `ks` - Kolmogorov–Smirnov statistic. Parameters: list of features you are creating the report for.
+- `distr_histogram` - feature distribution histogram. Parameters: list of features you are creating the report for.
+- `distr_boxplot` - feature distribution boxplot. Parameters: list of features you are creating the report for.
+- `distr_violinplot` - feature distribution violin plot. Parameters: list of features you are creating the report for.
+- `distr_densityplot` - feature distribution density plot. Parameters: list of features you are creating the report for.
+- `distance` - Euclidean distance between the real and simulated feature. Parameters: list of features you are creating the report for.
+- `statistics` - statistical indicators (average, median, standard deviation and variance) of a feature in both real and simulated datasets. Parameters: list of features you are creating the report for.
+
+#### Observation-based reports
+- `observation_distr_histogram` - observation distribution histogram. Parameters: list of observations you are creating the report for.
+- `observation_distr_boxplot` - observation distribution boxplot. Parameters: list of observations you are creating the report for.
+- `observation_distr_violinplot` - observation distribution violin plot. Parameters: list of observations you are creating the report for.
+- `observation_distr_densityplot` - observation distribution density plot. Parameters: list of observations you are creating the report for. The observation index 'all' can be used to report on all observations in one plot.
+- `observation_distance` - Euclidean distance between the real and simulated observation. Parameters: list of observations you are creating the report for.
+- `observation_statistics` - statistical indicators (average, median, standard deviation and variance) of an observation in both real and simulated datasets. Parameters: list of observations you are creating the report for.
+
+#### General reports
+- `copula_2d` - a 2D scatter plot that displays two features in a Gausian Multivariate copula space. Parameters: a report section of any name, under which the compared features are specified.
+- `copula_3d` - a 3D scatter plot that displays three features in a Gausian Multivariate copula space. Parameters: a report section of any name, under which the compared features are specified.
+- `feature_average_vs_variance` - a scatter plot that displays the average value of every feature on one axis and the variance of every feature on the other axis.
+- `observation_average_vs_variance` - a scatter plot that displays the average value of every observation on one axis and the variance of every observation on the other axis.
+- `corr` - correlation matrix heatmaps of the real and simulated datasets. Parameters: `percent_features` - an optional parameter for dimensionality reduction using PCA. A float value corresponding with the ratio of feature reduction (e.g. `percent_features` equal to 0.5 would reduce the feature count by half). 
+- `pca_2d` - two scatter plots with both datasets reduced to two dimensions using PCA.
+
+Here is a sample `reports` section of a configuration file containing all of the reports:
+
+```
+reports:
+  feature_based:
+    report1:
+      features:
+        - TGT
+        - ANV
+      report_types:
+        - ks
+        - distr_histogram
+        - distr_boxplot
+        - distr_violinplot
+        - distr_densityplot
+        - distance
+        - statistics
+  observation_based:
+    report1:
+      observations:
+        - 0
+      report_types:
+        - observation_distr_histogram
+        - observation_distr_boxplot
+        - observation_distr_violinplot
+        - observation_distr_densityplot
+        - observation_distance
+        - observation_statistics
+    report2:
+      observations:
+        - all
+      report_types:
+        - observation_distr_densityplot
+  general:
+    copula_2d:
+      report1:
+        - TGT
+        - ANV
+    copula_3d:
+      report1:
+        - TGT
+        - ANV
+        - CAS
+    feature_average_vs_variance:
+    observation_average_vs_variance:
+    corr:
+      percent_features: 0.6
+    pca_2d:
+```
+
+### Output
+
+An optional section where you can specify the file path of the generated report. The default path of the generated report is `<INSTALL_DIRECTORY>/output/report.html`. The report is exported in the HTML format.
+
+An example output section:
+
+```
+output:
+  path: './output/report.html'
+```
```

### Comparing `evalAIRR-0.0.8/evalAIRR/main.py` & `evalAIRR-0.0.9/evalAIRR/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,191 +1,201 @@
-import os
-import yaml
-import argparse
-
-from evalAIRR.util.input import read_encoded_csv
-from evalAIRR.util.corr import export_corr_heatmap
-from evalAIRR.util.pca import export_pca_2d_comparison
-from evalAIRR.util.univar import export_ks_test
-from evalAIRR.util.univar import export_distr_histogram, export_obs_distr_histogram
-from evalAIRR.util.univar import export_distr_boxplot, export_obs_distr_boxplot
-from evalAIRR.util.univar import export_distr_violinplot, export_obs_distr_violinplot
-from evalAIRR.util.univar import export_distr_densityplot, export_obs_distr_densityplot
-from evalAIRR.util.univar import export_avg_var_scatter_plot
-from evalAIRR.util.univar import export_distance, export_obs_distance
-from evalAIRR.util.univar import export_statistics, export_obs_statistics
-from evalAIRR.util.copula import export_copula_2d_scatter_plot, export_copula_3d_scatter_plot
-from evalAIRR.util.report import export_report
-
-#######################
-### PARSE ARGUMENTS ###
-#######################
-
-parser = argparse.ArgumentParser(prog='evalairr')
-parser.add_argument('-i', '--config', help='path to YAML confuguration file', required=True)
-
-def run():
-
-    #################
-    ### READ YAML ###
-    #################
-
-    YAML_FILE = parser.parse_args().config
-    CONFIG = []
-    with open(YAML_FILE, 'r') as stream:
-        try:
-            CONFIG = (yaml.safe_load(stream))
-        except yaml.YAMLError as exc:
-            print(exc)
-
-    REPORTS = CONFIG['reports']
-
-    try:
-        OUTPUT = CONFIG['output']['path']
-    except: 
-        OUTPUT = './output/report.html'
-        
-    #####################
-    ### READ DATASETS ###
-    #####################
-
-    features_R, data_R = read_encoded_csv(CONFIG['datasets']['real']['path'])
-    features_S, data_S = read_encoded_csv(CONFIG['datasets']['sim']['path'])
-
-    ##########################################
-    ### CREATE OUTPUT AND TEMP DIRECTORIES ###
-    ##########################################
-
-    if not os.path.exists('./output'):
-        os.makedirs('./output')
-    if not os.path.exists('./output/temp_figures'):
-        os.makedirs('./output/temp_figures')
-    if not os.path.exists('./output/temp_results'):
-        os.makedirs('./output/temp_results')
-    if not os.path.exists('./output/temp_statistics'):
-        os.makedirs('./output/temp_statistics')
-
-    #############################
-    ### FEATURE BASED REPORTS ###
-    #############################
-
-    if ('feature_based' in REPORTS):
-        reports_f = REPORTS['feature_based']
-        for report in reports_f:
-            features = reports_f[report]['features']
-            report_types = reports_f[report]['report_types']
-            for feature in features:
-
-                # KOLMOGOROV-SMIRNOV TEST REPORT
-                if 'ks' in report_types:
-                    export_ks_test(feature, data_R, data_S, features_R, features_S)
-
-                # DISTRIBUTION HISTOGRAM REPORT
-                if 'distr_histogram' in report_types:
-                    export_distr_histogram(feature, data_R, data_S, features_R, features_S)
-
-                # DISTRIBUTION BOX PLOT REPORT
-                if 'distr_boxplot' in report_types:
-                    export_distr_boxplot(feature, data_R, data_S, features_R, features_S)
-
-                # DISTRIBUTION VIOLIN PLOT REPORT
-                if 'distr_violinplot' in report_types:
-                    export_distr_violinplot(feature, data_R, data_S, features_R, features_S)
-
-                # DISTRIBUTION DENSITY PLOT REPORT
-                if 'distr_densityplot' in report_types:
-                    export_distr_densityplot(feature, data_R, data_S, features_R, features_S)
-
-                # EUCLIDEAN DISTANCE REPORT
-                if 'distance' in report_types:
-                    export_distance(feature, data_R, data_S, features_R, features_S)
-
-                # STATISTICS REPORT
-                if 'statistics' in report_types:
-                    export_statistics(feature, data_R, data_S, features_R, features_S)
-
-    #################################
-    ### OBSERVATION BASED REPORTS ###
-    #################################
-
-    if ('observation_based' in REPORTS):
-        reports_o = REPORTS['observation_based']
-        for report in reports_o:
-            observations = reports_o[report]['observations']
-            report_types = reports_o[report]['report_types']
-            for observation_index in observations:
-
-                # OBSERVATION DISTRIBUTION HISTOGRAM REPORT
-                if 'observation_distr_histogram' in report_types:
-                    export_obs_distr_histogram(observation_index, data_R, data_S)
-
-                # OBSERVATION DISTRIBUTION BOX PLOT REPORT
-                if 'observation_distr_boxplot' in report_types:
-                    export_obs_distr_boxplot(observation_index, data_R, data_S)
-
-                # OBSERVATION DISTRIBUTION VIOLIN PLOT REPORT
-                if 'observation_distr_violinplot' in report_types:
-                    export_obs_distr_violinplot(observation_index, data_R, data_S)
-
-                # OBSERVATION DISTRIBUTION DENSITY PLOT REPORT
-                if 'observation_distr_densityplot' in report_types:
-                    export_obs_distr_densityplot(observation_index, data_R, data_S)
-
-                # OBSERVATION EUCLIDEAN DISTANCE REPORT
-                if 'observation_distance' in report_types:
-                    export_obs_distance(observation_index, data_R, data_S)
-
-                # OBSERVATION STATISTICS REPORT
-                if 'observation_statistics' in report_types:
-                    export_obs_statistics(observation_index, data_R, data_S)
-
-    #######################
-    ### GENERAL REPORTS ###
-    #######################
-
-    if ('general' in REPORTS):
-        reports_g = REPORTS['general']
-
-        # CORRELATION MATRIX REPORT
-        if ('corr' in reports_g):
-            percent_features = reports_g['corr']['percent_features']
-            export_corr_heatmap(data_R, data_S, len(features_R), len(features_S), percent_features)
-
-        # PCA 2D REPORT
-        if ('pca_2d' in reports_g):
-            export_pca_2d_comparison(data_R, data_S)
-
-        # FEATURE AVERAGE VALUE VS VARIANCE REPORT
-        if ('feature_average_vs_variance' in reports_g):
-            export_avg_var_scatter_plot(data_R, data_S, axis=0)
-
-        # OBSERVATION AVERAGE VALUE VS VARIANCE REPORT
-        if ('observation_average_vs_variance' in reports_g):
-            export_avg_var_scatter_plot(data_R, data_S, axis=1)
-
-        # COPULA 2D REPORT
-        if ('copula_2d' in reports_g):
-            copula_reports = reports_g['copula_2d']
-            for copula_report in copula_reports:
-                if len(copula_reports[copula_report]) > 2:
-                    print(f'[WARNING] More than 2 features provided in \'{copula_report}\'! Using only the first 2 for calculations.')
-                elif len(copula_reports[copula_report]) < 2:
-                    print(f'[ERROR] 2D copula scatter plot report \'{copula_report}\' requires 2 features!')
-                    continue
-                export_copula_2d_scatter_plot(copula_reports[copula_report][0], copula_reports[copula_report][1], data_R, data_S, features_R, features_S)
-
-        # COPULA 3D REPORT
-        if ('copula_3d' in reports_g):
-            copula_reports = reports_g['copula_3d']
-            for copula_report in copula_reports:
-                if len(copula_reports[copula_report]) > 3:
-                    print(f'[WARNING] More than 3 features provided in \'{copula_report}\'! Using only the first 3 for calculations.')
-                elif len(copula_reports[copula_report]) < 3:
-                    print(f'[ERROR] 3D copula scatter plot report \'{copula_report}\' requires 3 features!')
-                    continue
-                export_copula_3d_scatter_plot(copula_reports[copula_report][0], copula_reports[copula_report][1], copula_reports[copula_report][2], data_R, data_S, features_R, features_S)
-
-    ##########################
-    ### EXPORT HTML REPORT ###
-    ##########################
-
+import os
+import yaml
+import argparse
+
+from evalAIRR.version import __version__
+from evalAIRR.util.input import read_encoded_csv
+from evalAIRR.util.corr import export_corr_heatmap
+from evalAIRR.util.pca import export_pca_2d_comparison
+from evalAIRR.util.univar import export_ks_test
+from evalAIRR.util.univar import export_distr_histogram, export_obs_distr_histogram
+from evalAIRR.util.univar import export_distr_boxplot, export_obs_distr_boxplot
+from evalAIRR.util.univar import export_distr_violinplot, export_obs_distr_violinplot
+from evalAIRR.util.univar import export_distr_densityplot, export_obs_distr_densityplot
+from evalAIRR.util.univar import export_avg_var_scatter_plot
+from evalAIRR.util.univar import export_distance, export_obs_distance
+from evalAIRR.util.univar import export_statistics, export_obs_statistics
+from evalAIRR.util.copula import export_copula_2d_scatter_plot, export_copula_3d_scatter_plot
+from evalAIRR.util.ml import export_ml_simulation
+from evalAIRR.util.report import export_report
+
+#######################
+### PARSE ARGUMENTS ###
+#######################
+
+parser = argparse.ArgumentParser(prog='evalairr')
+parser.add_argument('-i', '--config', help='path to YAML confuguration file', required=True)
+parser.add_argument('-v', '--version', action='version', version=__version__, help='check the version of evalAIRR')
+
+def run():
+
+    #################
+    ### READ YAML ###
+    #################
+
+    YAML_FILE = parser.parse_args().config
+    CONFIG = []
+    with open(YAML_FILE, 'r') as stream:
+        try:
+            CONFIG = (yaml.safe_load(stream))
+        except yaml.YAMLError as exc:
+            print(exc)
+
+    REPORTS = CONFIG['reports']
+
+    try:
+        OUTPUT = CONFIG['output']['path']
+    except: 
+        OUTPUT = './output/report.html'
+        
+    #####################
+    ### READ DATASETS ###
+    #####################
+
+    features_R, data_R = read_encoded_csv(CONFIG['datasets']['real']['path'])
+    features_S, data_S = read_encoded_csv(CONFIG['datasets']['sim']['path'])
+
+    ##########################################
+    ### CREATE OUTPUT AND TEMP DIRECTORIES ###
+    ##########################################
+
+    if not os.path.exists('./output'):
+        os.makedirs('./output')
+    if not os.path.exists('./output/temp_figures'):
+        os.makedirs('./output/temp_figures')
+    if not os.path.exists('./output/temp_results'):
+        os.makedirs('./output/temp_results')
+    if not os.path.exists('./output/temp_statistics'):
+        os.makedirs('./output/temp_statistics')
+
+    #############################
+    ### FEATURE BASED REPORTS ###
+    #############################
+
+    if ('feature_based' in REPORTS):
+        reports_f = REPORTS['feature_based']
+        for report in reports_f:
+            features = reports_f[report]['features']
+            report_types = reports_f[report]['report_types']
+            for feature in features:
+
+                # KOLMOGOROV-SMIRNOV TEST REPORT
+                if 'ks' in report_types:
+                    export_ks_test(feature, data_R, data_S, features_R, features_S)
+
+                # DISTRIBUTION HISTOGRAM REPORT
+                if 'distr_histogram' in report_types:
+                    export_distr_histogram(feature, data_R, data_S, features_R, features_S)
+
+                # DISTRIBUTION BOX PLOT REPORT
+                if 'distr_boxplot' in report_types:
+                    export_distr_boxplot(feature, data_R, data_S, features_R, features_S)
+
+                # DISTRIBUTION VIOLIN PLOT REPORT
+                if 'distr_violinplot' in report_types:
+                    export_distr_violinplot(feature, data_R, data_S, features_R, features_S)
+
+                # DISTRIBUTION DENSITY PLOT REPORT
+                if 'distr_densityplot' in report_types:
+                    export_distr_densityplot(feature, data_R, data_S, features_R, features_S)
+
+                # EUCLIDEAN DISTANCE REPORT
+                if 'distance' in report_types:
+                    export_distance(feature, data_R, data_S, features_R, features_S)
+
+                # STATISTICS REPORT
+                if 'statistics' in report_types:
+                    export_statistics(feature, data_R, data_S, features_R, features_S)
+
+    #################################
+    ### OBSERVATION BASED REPORTS ###
+    #################################
+
+    if ('observation_based' in REPORTS):
+        reports_o = REPORTS['observation_based']
+        for report in reports_o:
+            observations = reports_o[report]['observations']
+            report_types = reports_o[report]['report_types']
+            for observation_index in observations:
+
+                # OBSERVATION DISTRIBUTION HISTOGRAM REPORT
+                if 'observation_distr_histogram' in report_types:
+                    export_obs_distr_histogram(observation_index, data_R, data_S)
+
+                # OBSERVATION DISTRIBUTION BOX PLOT REPORT
+                if 'observation_distr_boxplot' in report_types:
+                    export_obs_distr_boxplot(observation_index, data_R, data_S)
+
+                # OBSERVATION DISTRIBUTION VIOLIN PLOT REPORT
+                if 'observation_distr_violinplot' in report_types:
+                    export_obs_distr_violinplot(observation_index, data_R, data_S)
+
+                # OBSERVATION DISTRIBUTION DENSITY PLOT REPORT
+                if 'observation_distr_densityplot' in report_types:
+                    export_obs_distr_densityplot(observation_index, data_R, data_S)
+
+                # OBSERVATION EUCLIDEAN DISTANCE REPORT
+                if 'observation_distance' in report_types:
+                    export_obs_distance(observation_index, data_R, data_S)
+
+                # OBSERVATION STATISTICS REPORT
+                if 'observation_statistics' in report_types:
+                    export_obs_statistics(observation_index, data_R, data_S)
+
+    #######################
+    ### GENERAL REPORTS ###
+    #######################
+
+    if ('general' in REPORTS):
+        reports_g = REPORTS['general']
+
+        # CORRELATION MATRIX REPORT
+        if ('corr' in reports_g):
+            percent_features = reports_g['corr']['percent_features']
+            export_corr_heatmap(data_R, data_S, len(features_R), len(features_S), percent_features)
+
+        # PCA 2D REPORT
+        if ('pca_2d' in reports_g):
+            export_pca_2d_comparison(data_R, data_S)
+
+        # FEATURE AVERAGE VALUE VS VARIANCE REPORT
+        if ('feature_average_vs_variance' in reports_g):
+            export_avg_var_scatter_plot(data_R, data_S, axis=0)
+
+        # OBSERVATION AVERAGE VALUE VS VARIANCE REPORT
+        if ('observation_average_vs_variance' in reports_g):
+            export_avg_var_scatter_plot(data_R, data_S, axis=1)
+
+        # COPULA 2D REPORT
+        if ('copula_2d' in reports_g):
+            copula_reports = reports_g['copula_2d']
+            for copula_report in copula_reports:
+                if len(copula_reports[copula_report]) > 2:
+                    print(f'[WARNING] More than 2 features provided in \'{copula_report}\'! Using only the first 2 for calculations.')
+                elif len(copula_reports[copula_report]) < 2:
+                    print(f'[ERROR] 2D copula scatter plot report \'{copula_report}\' requires 2 features!')
+                    continue
+                export_copula_2d_scatter_plot(copula_reports[copula_report][0], copula_reports[copula_report][1], data_R, data_S, features_R, features_S)
+
+        # COPULA 3D REPORT
+        if ('copula_3d' in reports_g):
+            copula_reports = reports_g['copula_3d']
+            for copula_report in copula_reports:
+                if len(copula_reports[copula_report]) > 3:
+                    print(f'[WARNING] More than 3 features provided in \'{copula_report}\'! Using only the first 3 for calculations.')
+                elif len(copula_reports[copula_report]) < 3:
+                    print(f'[ERROR] 3D copula scatter plot report \'{copula_report}\' requires 3 features!')
+                    continue
+                export_copula_3d_scatter_plot(copula_reports[copula_report][0], copula_reports[copula_report][1], copula_reports[copula_report][2], data_R, data_S, features_R, features_S)
+
+        # ML SIMULATION
+        if ('ml_sim' in reports_g):
+            print('ml_sim')
+            n_informative = reports_g['ml_sim']['n_informative']
+            print('n_informative')
+            export_ml_simulation(data_R, data_S, features_R, n_informative)
+
+    ##########################
+    ### EXPORT HTML REPORT ###
+    ##########################
+
     export_report(OUTPUT)
```

### Comparing `evalAIRR-0.0.8/evalAIRR/util/copula.py` & `evalAIRR-0.0.9/evalAIRR/util/copula.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,125 +1,125 @@
-import numpy as np
-import pandas as pd
-import matplotlib.pyplot as plt
-
-from evalAIRR.util.univar import get_feature_data
-
-from copulas.univariate import Univariate
-from copulas.multivariate import GaussianMultivariate
-from copulas.visualization import compare_2d, compare_3d
-
-import warnings
-warnings.filterwarnings("ignore")
-
-def export_copula_2d_scatter_plot(feature_1, feature_2, data_R, data_S, features_R, features_S):
-    data_R_f1 = get_feature_data(feature_1, data_R, features_R)
-    data_R_f2 = get_feature_data(feature_2, data_R, features_R)
-    if not any(data_R_f1) or not any(data_R_f2):
-        return
-
-    data_S_f1 = get_feature_data(feature_1, data_S, features_S)
-    data_S_f2 = get_feature_data(feature_2, data_S, features_S)
-    if not any(data_R_f2) or not any(data_S_f2):
-        return
-
-    data_R_join = np.stack((data_R_f1, data_R_f2)).T
-    data_S_join = np.stack((data_S_f1, data_S_f2)).T
-
-    univariate = Univariate()
-    univariate.fit(data_R_f1)
-    data_R_f1_dist = univariate.to_dict()['type']
-    univariate.fit(data_R_f2)
-    data_R_f2_dist = univariate.to_dict()['type']
-    univariate.fit(data_S_f1)
-    data_S_f1_dist = univariate.to_dict()['type']
-    univariate.fit(data_S_f2)
-    data_S_f2_dist = univariate.to_dict()['type']
-
-    dist_R = GaussianMultivariate(distribution={
-        feature_1: data_R_f1_dist,
-        feature_2: data_R_f2_dist
-    })
-    d_R = { feature_1: data_R_join[:, 0], feature_2: data_R_join[:, 1] }
-    df_R = pd.DataFrame(data=d_R)
-    dist_R.fit(df_R)
-
-    dist_S = GaussianMultivariate(distribution={
-        feature_1: data_S_f1_dist,
-        feature_2: data_S_f2_dist
-    })
-    d_S = { feature_1: data_S_join[:, 0], feature_2: data_S_join[:, 1] }
-    df_S = pd.DataFrame(data=d_S)
-    dist_S.fit(df_S)
-
-    compare_2d(df_R, df_S)
-    plt.suptitle(f'Distribution of {feature_1} and {feature_2} in copula space')
-    plt.savefig(f'./output/temp_figures/copula_2d_plot_{feature_1}_{feature_2}.svg')
-    plt.close()
-
-def export_copula_3d_scatter_plot(feature_1, feature_2, feature_3, data_R, data_S, features_R, features_S):
-    data_R_f1 = get_feature_data(feature_1, data_R, features_R)
-    data_R_f2 = get_feature_data(feature_2, data_R, features_R)
-    data_R_f3 = get_feature_data(feature_3, data_R, features_R)
-    if not any(data_R_f1) or not any(data_R_f2) or not any(data_R_f3):
-        return
-
-    data_S_f1 = get_feature_data(feature_1, data_S, features_S)
-    data_S_f2 = get_feature_data(feature_2, data_S, features_S)
-    data_S_f3 = get_feature_data(feature_3, data_S, features_S)
-    if not any(data_R_f2) or not any(data_S_f2) or not any(data_S_f3):
-        return
-
-    data_R_join = np.stack((data_R_f1, data_R_f2, data_R_f3)).T
-    data_S_join = np.stack((data_S_f1, data_S_f2, data_S_f3)).T
-
-    univariate = Univariate()
-    univariate.fit(data_R_f1)
-    data_R_f1_dist = univariate.to_dict()['type']
-    univariate.fit(data_R_f2)
-    data_R_f2_dist = univariate.to_dict()['type']
-    univariate.fit(data_R_f3)
-    data_R_f3_dist = univariate.to_dict()['type']
-    univariate.fit(data_S_f1)
-    data_S_f1_dist = univariate.to_dict()['type']
-    univariate.fit(data_S_f2)
-    data_S_f2_dist = univariate.to_dict()['type']
-    univariate.fit(data_S_f3)
-    data_S_f3_dist = univariate.to_dict()['type']
-
-    dist_R = GaussianMultivariate(distribution={
-        feature_1: data_R_f1_dist,
-        feature_2: data_R_f2_dist,
-        feature_3: data_R_f3_dist
-    })
-    d_R = { 
-        feature_1: data_R_join[:, 0], 
-        feature_2: data_R_join[:, 1], 
-        feature_3: data_R_join[:, 2] 
-    }
-    df_R = pd.DataFrame(data=d_R)
-    dist_R.fit(df_R)
-
-    dist_S = GaussianMultivariate(distribution={
-        feature_1: data_S_f1_dist,
-        feature_2: data_S_f2_dist,
-        feature_3: data_S_f3_dist
-    })
-    d_S = { 
-        feature_1: data_S_join[:, 0], 
-        feature_2: data_S_join[:, 1], 
-        feature_3: data_S_join[:, 2] 
-    }
-    df_S = pd.DataFrame(data=d_S)
-    dist_S.fit(df_S)
-
-    compare_3d(df_R, df_S, columns=[feature_1, feature_2, feature_3], figsize=(10, 5))
-    fig = plt.gcf()
-    fig.suptitle(f'Distribution of {feature_1}, {feature_2} and {feature_3} in copula space')
-    for ax in fig.axes:
-        ax.set_xlabel(feature_1)
-        ax.set_ylabel(feature_2)
-        ax.set_zlabel(feature_3)
-    fig.tight_layout()
-    fig.savefig(f'./output/temp_figures/copula_3d_plot_{feature_1}_{feature_2}_{feature_3}.svg')
-    del fig
+import numpy as np
+import pandas as pd
+import matplotlib.pyplot as plt
+
+from evalAIRR.util.univar import get_feature_data
+
+from copulas.univariate import Univariate
+from copulas.multivariate import GaussianMultivariate
+from copulas.visualization import compare_2d, compare_3d
+
+import warnings
+warnings.filterwarnings("ignore")
+
+def export_copula_2d_scatter_plot(feature_1, feature_2, data_R, data_S, features_R, features_S):
+    data_R_f1 = get_feature_data(feature_1, data_R, features_R)
+    data_R_f2 = get_feature_data(feature_2, data_R, features_R)
+    if not any(data_R_f1) or not any(data_R_f2):
+        return
+
+    data_S_f1 = get_feature_data(feature_1, data_S, features_S)
+    data_S_f2 = get_feature_data(feature_2, data_S, features_S)
+    if not any(data_R_f2) or not any(data_S_f2):
+        return
+
+    data_R_join = np.stack((data_R_f1, data_R_f2)).T
+    data_S_join = np.stack((data_S_f1, data_S_f2)).T
+
+    univariate = Univariate()
+    univariate.fit(data_R_f1)
+    data_R_f1_dist = univariate.to_dict()['type']
+    univariate.fit(data_R_f2)
+    data_R_f2_dist = univariate.to_dict()['type']
+    univariate.fit(data_S_f1)
+    data_S_f1_dist = univariate.to_dict()['type']
+    univariate.fit(data_S_f2)
+    data_S_f2_dist = univariate.to_dict()['type']
+
+    dist_R = GaussianMultivariate(distribution={
+        feature_1: data_R_f1_dist,
+        feature_2: data_R_f2_dist
+    })
+    d_R = { feature_1: data_R_join[:, 0], feature_2: data_R_join[:, 1] }
+    df_R = pd.DataFrame(data=d_R)
+    dist_R.fit(df_R)
+
+    dist_S = GaussianMultivariate(distribution={
+        feature_1: data_S_f1_dist,
+        feature_2: data_S_f2_dist
+    })
+    d_S = { feature_1: data_S_join[:, 0], feature_2: data_S_join[:, 1] }
+    df_S = pd.DataFrame(data=d_S)
+    dist_S.fit(df_S)
+
+    compare_2d(df_R, df_S)
+    plt.suptitle(f'Distribution of {feature_1} and {feature_2} in copula space')
+    plt.savefig(f'./output/temp_figures/copula_2d_plot_{feature_1}_{feature_2}.svg')
+    plt.close()
+
+def export_copula_3d_scatter_plot(feature_1, feature_2, feature_3, data_R, data_S, features_R, features_S):
+    data_R_f1 = get_feature_data(feature_1, data_R, features_R)
+    data_R_f2 = get_feature_data(feature_2, data_R, features_R)
+    data_R_f3 = get_feature_data(feature_3, data_R, features_R)
+    if not any(data_R_f1) or not any(data_R_f2) or not any(data_R_f3):
+        return
+
+    data_S_f1 = get_feature_data(feature_1, data_S, features_S)
+    data_S_f2 = get_feature_data(feature_2, data_S, features_S)
+    data_S_f3 = get_feature_data(feature_3, data_S, features_S)
+    if not any(data_R_f2) or not any(data_S_f2) or not any(data_S_f3):
+        return
+
+    data_R_join = np.stack((data_R_f1, data_R_f2, data_R_f3)).T
+    data_S_join = np.stack((data_S_f1, data_S_f2, data_S_f3)).T
+
+    univariate = Univariate()
+    univariate.fit(data_R_f1)
+    data_R_f1_dist = univariate.to_dict()['type']
+    univariate.fit(data_R_f2)
+    data_R_f2_dist = univariate.to_dict()['type']
+    univariate.fit(data_R_f3)
+    data_R_f3_dist = univariate.to_dict()['type']
+    univariate.fit(data_S_f1)
+    data_S_f1_dist = univariate.to_dict()['type']
+    univariate.fit(data_S_f2)
+    data_S_f2_dist = univariate.to_dict()['type']
+    univariate.fit(data_S_f3)
+    data_S_f3_dist = univariate.to_dict()['type']
+
+    dist_R = GaussianMultivariate(distribution={
+        feature_1: data_R_f1_dist,
+        feature_2: data_R_f2_dist,
+        feature_3: data_R_f3_dist
+    })
+    d_R = { 
+        feature_1: data_R_join[:, 0], 
+        feature_2: data_R_join[:, 1], 
+        feature_3: data_R_join[:, 2] 
+    }
+    df_R = pd.DataFrame(data=d_R)
+    dist_R.fit(df_R)
+
+    dist_S = GaussianMultivariate(distribution={
+        feature_1: data_S_f1_dist,
+        feature_2: data_S_f2_dist,
+        feature_3: data_S_f3_dist
+    })
+    d_S = { 
+        feature_1: data_S_join[:, 0], 
+        feature_2: data_S_join[:, 1], 
+        feature_3: data_S_join[:, 2] 
+    }
+    df_S = pd.DataFrame(data=d_S)
+    dist_S.fit(df_S)
+
+    compare_3d(df_R, df_S, columns=[feature_1, feature_2, feature_3], figsize=(10, 5))
+    fig = plt.gcf()
+    fig.suptitle(f'Distribution of {feature_1}, {feature_2} and {feature_3} in copula space')
+    for ax in fig.axes:
+        ax.set_xlabel(feature_1)
+        ax.set_ylabel(feature_2)
+        ax.set_zlabel(feature_3)
+    fig.tight_layout()
+    fig.savefig(f'./output/temp_figures/copula_3d_plot_{feature_1}_{feature_2}_{feature_3}.svg')
+    del fig
     plt.close()
```

### Comparing `evalAIRR-0.0.8/evalAIRR/util/corr.py` & `evalAIRR-0.0.9/evalAIRR/util/corr.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-import math
-import pandas as pd
-import seaborn as sns
-import matplotlib.pyplot as plt
-from evalAIRR.util.pca import pca
-
-def export_corr_heatmap(data_real, data_sim, n_real_feat = 0, n_sim_feat = 0, pca_ratio = 0):
-    print('[LOG] CORR: Exporting correlation matrix heatmap')
-    if n_real_feat != 0 and n_sim_feat != 0 and pca_ratio != 0:
-        print('[LOG] CORR: Reducing dimentions using PCA')
-        _, data_real = pca(data_real, math.floor(min(data_real.shape[0], data_real.shape[1]) * pca_ratio))
-        _, data_sim = pca(data_sim, math.floor(min(data_real.shape[0], data_real.shape[1]) * pca_ratio))
-
-    print('[LOG] CORR: Calculating correlation matrices')
-    corr_real = pd.DataFrame(data_real).corr()
-    corr_sim = pd.DataFrame(data_sim).corr()
-
-    diff_corrs = corr_real.sub(corr_sim).abs()
-
-    print('[LOG] CORR: Displaying correlation heatmaps')
-    f,(ax1,ax2,ax3, axcb) = plt.subplots(1,4,gridspec_kw={'width_ratios':[1,1,1,0.08]})
-    f.set_size_inches(15, 5)
-    f.suptitle('Correlation heatmaps')
-    ax1.get_shared_y_axes().join(ax2,ax3)
-    g1 = sns.heatmap(corr_real,cmap="YlGnBu",cbar=False,ax=ax1)
-    g1.set_title('Real dataset')
-    g1.set_ylabel('')
-    g1.set_xlabel('')
-    g2 = sns.heatmap(corr_sim,cmap="YlGnBu",cbar=False,ax=ax2)
-    g2.set_title('Simulated dataset')
-    g2.set_ylabel('')
-    g2.set_xlabel('')
-    g2.set_yticks([])
-    g3 = sns.heatmap(diff_corrs,cmap="YlGnBu",ax=ax3, cbar_ax=axcb)
-    g3.set_title('Difference in correlation')
-    g3.set_ylabel('')
-    g3.set_xlabel('')
-    g3.set_yticks([])
-    
-    f.savefig(f'./output/temp_figures/corr_matrix.svg')
-    del f
+import math
+import pandas as pd
+import seaborn as sns
+import matplotlib.pyplot as plt
+from evalAIRR.util.pca import pca
+
+def export_corr_heatmap(data_real, data_sim, n_real_feat = 0, n_sim_feat = 0, pca_ratio = 0):
+    print('[LOG] CORR: Exporting correlation matrix heatmap')
+    if n_real_feat != 0 and n_sim_feat != 0 and pca_ratio != 0:
+        print('[LOG] CORR: Reducing dimentions using PCA')
+        _, data_real = pca(data_real, math.floor(min(data_real.shape[0], data_real.shape[1]) * pca_ratio))
+        _, data_sim = pca(data_sim, math.floor(min(data_real.shape[0], data_real.shape[1]) * pca_ratio))
+
+    print('[LOG] CORR: Calculating correlation matrices')
+    corr_real = pd.DataFrame(data_real).corr()
+    corr_sim = pd.DataFrame(data_sim).corr()
+
+    diff_corrs = corr_real.sub(corr_sim).abs()
+
+    print('[LOG] CORR: Displaying correlation heatmaps')
+    f,(ax1,ax2,ax3, axcb) = plt.subplots(1,4,gridspec_kw={'width_ratios':[1,1,1,0.08]})
+    f.set_size_inches(15, 5)
+    f.suptitle('Correlation heatmaps')
+    ax1.get_shared_y_axes().join(ax2,ax3)
+    g1 = sns.heatmap(corr_real,cmap="YlGnBu",cbar=False,ax=ax1)
+    g1.set_title('Real dataset')
+    g1.set_ylabel('')
+    g1.set_xlabel('')
+    g2 = sns.heatmap(corr_sim,cmap="YlGnBu",cbar=False,ax=ax2)
+    g2.set_title('Simulated dataset')
+    g2.set_ylabel('')
+    g2.set_xlabel('')
+    g2.set_yticks([])
+    g3 = sns.heatmap(diff_corrs,cmap="YlGnBu",ax=ax3, cbar_ax=axcb)
+    g3.set_title('Difference in correlation')
+    g3.set_ylabel('')
+    g3.set_xlabel('')
+    g3.set_yticks([])
+    
+    f.savefig(f'./output/temp_figures/corr_matrix.svg')
+    del f
     plt.close()
```

### Comparing `evalAIRR-0.0.8/evalAIRR/util/input.py` & `evalAIRR-0.0.9/evalAIRR/util/input.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import numpy as np
-
-def read_encoded_csv(csv_path):
-
-    print('[LOG] Reading file: ' + csv_path)
-    data_file = open(csv_path, "r")
-    features = data_file.readline().split(',')
-    features = [f.replace('\n', '').strip() for f in features]
-    print(f'[LOG] Number of features in "{csv_path}" :', len(features))
-    data = []
-    for row in data_file:
-        row = row.replace('\n', '').split(',')
-        float_row = []
-        for x in row:
-            float_row.append(float(x))
-        data.append(float_row)
+import numpy as np
+
+def read_encoded_csv(csv_path):
+
+    print('[LOG] Reading file: ' + csv_path)
+    data_file = open(csv_path, "r")
+    features = data_file.readline().split(',')
+    features = [f.replace('\n', '').strip() for f in features]
+    print(f'[LOG] Number of features in "{csv_path}" :', len(features))
+    data = []
+    for row in data_file:
+        row = row.replace('\n', '').split(',')
+        float_row = []
+        for x in row:
+            float_row.append(float(x))
+        data.append(float_row)
     return np.array(features), np.array(data)
```

### Comparing `evalAIRR-0.0.8/evalAIRR/util/pca.py` & `evalAIRR-0.0.9/evalAIRR/util/pca.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import numpy as np
-import matplotlib.pyplot as plt
-from sklearn.decomposition import PCA
-
-def pca(A,m):
-    pca = PCA(n_components=m, copy=True)
-    pca.fit(A)
-    return pca.explained_variance_, pca.transform(A)
-
-def export_pca_2d_comparison(data_real, data_sim):
-    _, pca_R = pca(data_real, 2)
-    _, pca_S = pca(data_sim, 2)
-
-    f, ax = plt.subplots(1, 1)
-    f.set_size_inches(5, 5)
-    f.suptitle('Real and simulated dataset comparison\nin two dimensions using PCA')
-    ax.scatter(pca_R[:, 0], pca_R[:, 1], label='Real')
-    ax.scatter(pca_S[:, 0], pca_S[:, 1], c='red', label='Simulated')
-    ax.legend()
-    f.tight_layout()
-    # ax2.set_ylabel('')
-    # ax2.set_yticklabels([])
-    # ax2.set_yticks([])
-
-    f.savefig(f'./output/temp_figures/pca_2d_comparison.svg')
-    del f
+import numpy as np
+import matplotlib.pyplot as plt
+from sklearn.decomposition import PCA
+
+def pca(A,m):
+    pca = PCA(n_components=m, copy=True)
+    pca.fit(A)
+    return pca.explained_variance_, pca.transform(A)
+
+def export_pca_2d_comparison(data_real, data_sim):
+    _, pca_R = pca(data_real, 2)
+    _, pca_S = pca(data_sim, 2)
+
+    f, ax = plt.subplots(1, 1)
+    f.set_size_inches(5, 5)
+    f.suptitle('Real and simulated dataset comparison\nin two dimensions using PCA')
+    ax.scatter(pca_R[:, 0], pca_R[:, 1], label='Real')
+    ax.scatter(pca_S[:, 0], pca_S[:, 1], c='red', label='Simulated')
+    ax.legend()
+    f.tight_layout()
+    # ax2.set_ylabel('')
+    # ax2.set_yticklabels([])
+    # ax2.set_yticks([])
+
+    f.savefig(f'./output/temp_figures/pca_2d_comparison.svg')
+    del f
     plt.close()
```

### Comparing `evalAIRR-0.0.8/evalAIRR/util/report.py` & `evalAIRR-0.0.9/evalAIRR/util/report.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,192 +1,195 @@
-00000000: 696d 706f 7274 206f 730a 696d 706f 7274  import os.import
-00000010: 2062 6173 6536 340a 0a64 6566 2065 7870   base64..def exp
-00000020: 6f72 745f 7265 706f 7274 284f 5554 5055  ort_report(OUTPU
-00000030: 5429 3a0a 2020 2020 7072 696e 7428 275b  T):.    print('[
-00000040: 4c4f 475d 2045 7870 6f72 7469 6e67 2048  LOG] Exporting H
-00000050: 544d 4c20 7265 706f 7274 2729 0a20 2020  TML report').   
-00000060: 2074 7279 3a0a 2020 2020 2020 2020 7769   try:.        wi
-00000070: 7468 206f 7065 6e28 4f55 5450 5554 2c20  th open(OUTPUT, 
-00000080: 2777 272c 2065 6e63 6f64 696e 673d 2275  'w', encoding="u
-00000090: 7466 2d38 2229 2061 7320 6f75 7470 7574  tf-8") as output
-000000a0: 5f66 696c 653a 0a20 2020 2020 2020 2020  _file:.         
-000000b0: 2020 2069 6620 616e 7928 6f73 2e6c 6973     if any(os.lis
-000000c0: 7464 6972 2827 2e2f 6f75 7470 7574 2f74  tdir('./output/t
-000000d0: 656d 705f 7265 7375 6c74 7327 2929 3a0a  emp_results')):.
-000000e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000000f0: 6f75 7470 7574 5f66 696c 652e 7772 6974  output_file.writ
-00000100: 6528 273c 6469 7620 7374 796c 653d 2264  e('<div style="d
-00000110: 6973 706c 6179 3a20 666c 6578 3b20 6a75  isplay: flex; ju
-00000120: 7374 6966 792d 636f 6e74 656e 743a 2063  stify-content: c
-00000130: 656e 7465 723b 223e 3c68 333e 5265 7375  enter;"><h3>Resu
-00000140: 6c74 733c 2f68 333e 3c2f 6469 763e 2729  lts</h3></div>')
-00000150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000160: 206f 7574 7075 745f 6669 6c65 2e77 7269   output_file.wri
-00000170: 7465 2827 3c64 6976 2073 7479 6c65 3d22  te('<div style="
-00000180: 6469 7370 6c61 793a 2066 6c65 783b 206a  display: flex; j
-00000190: 7573 7469 6679 2d63 6f6e 7465 6e74 3a20  ustify-content: 
-000001a0: 6365 6e74 6572 3b22 3e5c 6e27 290a 2020  center;">\n').  
-000001b0: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
-000001c0: 7470 7574 5f66 696c 652e 7772 6974 6528  tput_file.write(
-000001d0: 275c 743c 7461 626c 6520 7374 796c 653d  '\t<table style=
-000001e0: 2262 6f72 6465 723a 6e6f 6e65 3b20 7769  "border:none; wi
-000001f0: 6474 683a 3330 253b 223e 5c6e 2729 0a20  dth:30%;">\n'). 
-00000200: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00000210: 6f72 2072 6573 756c 745f 6669 6c65 2069  or result_file i
-00000220: 6e20 6f73 2e6c 6973 7464 6972 2827 2e2f  n os.listdir('./
-00000230: 6f75 7470 7574 2f74 656d 705f 7265 7375  output/temp_resu
-00000240: 6c74 7327 293a 0a20 2020 2020 2020 2020  lts'):.         
-00000250: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-00000260: 6f70 656e 2827 2e2f 6f75 7470 7574 2f74  open('./output/t
-00000270: 656d 705f 7265 7375 6c74 732f 2720 2b20  emp_results/' + 
-00000280: 7265 7375 6c74 5f66 696c 652c 2027 7227  result_file, 'r'
-00000290: 2920 6173 2072 6573 3a0a 2020 2020 2020  ) as res:.      
-000002a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000002b0: 2020 6f75 7470 7574 5f66 696c 652e 7772    output_file.wr
-000002c0: 6974 6528 6627 7b72 6573 2e72 6561 6428  ite(f'{res.read(
-000002d0: 297d 2729 0a20 2020 2020 2020 2020 2020  )}').           
-000002e0: 2020 2020 2020 2020 206f 732e 7265 6d6f           os.remo
-000002f0: 7665 2827 2e2f 6f75 7470 7574 2f74 656d  ve('./output/tem
-00000300: 705f 7265 7375 6c74 732f 2720 2b20 7265  p_results/' + re
-00000310: 7375 6c74 5f66 696c 6529 0a20 2020 2020  sult_file).     
-00000320: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
-00000330: 745f 6669 6c65 2e77 7269 7465 2827 5c74  t_file.write('\t
-00000340: 3c2f 7461 626c 653e 5c6e 2729 0a20 2020  </table>\n').   
-00000350: 2020 2020 2020 2020 2020 2020 206f 7574               out
-00000360: 7075 745f 6669 6c65 2e77 7269 7465 2827  put_file.write('
-00000370: 3c2f 6469 763e 3c62 723e 3c62 723e 5c6e  </div><br><br>\n
-00000380: 2729 0a20 2020 2020 2020 2020 2020 2069  ').            i
-00000390: 6620 616e 7928 6f73 2e6c 6973 7464 6972  f any(os.listdir
-000003a0: 2827 2e2f 6f75 7470 7574 2f74 656d 705f  ('./output/temp_
-000003b0: 7374 6174 6973 7469 6373 2729 293a 0a20  statistics')):. 
-000003c0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-000003d0: 7574 7075 745f 6669 6c65 2e77 7269 7465  utput_file.write
-000003e0: 2827 3c64 6976 2073 7479 6c65 3d22 6469  ('<div style="di
-000003f0: 7370 6c61 793a 2066 6c65 783b 206a 7573  splay: flex; jus
-00000400: 7469 6679 2d63 6f6e 7465 6e74 3a20 6365  tify-content: ce
-00000410: 6e74 6572 3b22 3e3c 6833 3e53 7461 7469  nter;"><h3>Stati
-00000420: 7374 6963 733c 2f68 333e 3c2f 6469 763e  stics</h3></div>
-00000430: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
-00000440: 2020 206f 7574 7075 745f 6669 6c65 2e77     output_file.w
-00000450: 7269 7465 2827 3c64 6976 2073 7479 6c65  rite('<div style
-00000460: 3d22 6469 7370 6c61 793a 2066 6c65 783b  ="display: flex;
-00000470: 206a 7573 7469 6679 2d63 6f6e 7465 6e74   justify-content
-00000480: 3a20 6365 6e74 6572 3b22 3e5c 6e27 290a  : center;">\n').
-00000490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000004a0: 6f75 7470 7574 5f66 696c 652e 7772 6974  output_file.writ
-000004b0: 6528 275c 743c 7461 626c 6520 7374 796c  e('\t<table styl
-000004c0: 653d 2262 6f72 6465 723a 6e6f 6e65 3b20  e="border:none; 
-000004d0: 7769 6474 683a 3735 253b 223e 5c6e 2729  width:75%;">\n')
-000004e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000004f0: 206f 7574 7075 745f 6669 6c65 2e77 7269   output_file.wri
-00000500: 7465 2827 5c74 5c74 3c74 723e 5c6e 2729  te('\t\t<tr>\n')
-00000510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000520: 206f 7574 7075 745f 6669 6c65 2e77 7269   output_file.wri
-00000530: 7465 2827 5c74 5c74 5c74 3c74 6820 7374  te('\t\t\t<th st
-00000540: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
-00000550: 6c65 6674 3b22 3e53 7461 7469 7374 6963  left;">Statistic
-00000560: 3c2f 7468 3e5c 6e27 290a 2020 2020 2020  </th>\n').      
-00000570: 2020 2020 2020 2020 2020 6f75 7470 7574            output
-00000580: 5f66 696c 652e 7772 6974 6528 275c 745c  _file.write('\t\
-00000590: 745c 743c 7468 2073 7479 6c65 3d22 7465  t\t<th style="te
-000005a0: 7874 2d61 6c69 676e 3a6c 6566 743b 223e  xt-align:left;">
-000005b0: 5265 616c 2064 6174 6173 6574 3c2f 7468  Real dataset</th
-000005c0: 3e5c 6e27 290a 2020 2020 2020 2020 2020  >\n').          
-000005d0: 2020 2020 2020 6f75 7470 7574 5f66 696c        output_fil
-000005e0: 652e 7772 6974 6528 275c 745c 745c 743c  e.write('\t\t\t<
-000005f0: 7468 2073 7479 6c65 3d22 7465 7874 2d61  th style="text-a
-00000600: 6c69 676e 3a6c 6566 743b 223e 5369 6d75  lign:left;">Simu
-00000610: 6c61 7465 6420 6461 7461 7365 743c 2f74  lated dataset</t
-00000620: 683e 5c6e 2729 0a20 2020 2020 2020 2020  h>\n').         
-00000630: 2020 2020 2020 206f 7574 7075 745f 6669         output_fi
-00000640: 6c65 2e77 7269 7465 2827 5c74 5c74 3c2f  le.write('\t\t</
-00000650: 7472 3e5c 6e27 290a 2020 2020 2020 2020  tr>\n').        
-00000660: 2020 2020 2020 2020 666f 7220 7265 7375          for resu
-00000670: 6c74 5f66 696c 6520 696e 206f 732e 6c69  lt_file in os.li
-00000680: 7374 6469 7228 272e 2f6f 7574 7075 742f  stdir('./output/
-00000690: 7465 6d70 5f73 7461 7469 7374 6963 7327  temp_statistics'
-000006a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000006b0: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
-000006c0: 2827 2e2f 6f75 7470 7574 2f74 656d 705f  ('./output/temp_
-000006d0: 7374 6174 6973 7469 6373 2f27 202b 2072  statistics/' + r
-000006e0: 6573 756c 745f 6669 6c65 2c20 2772 2729  esult_file, 'r')
-000006f0: 2061 7320 7265 733a 0a20 2020 2020 2020   as res:.       
-00000700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000710: 206f 7574 7075 745f 6669 6c65 2e77 7269   output_file.wri
-00000720: 7465 2866 277b 7265 732e 7265 6164 2829  te(f'{res.read()
-00000730: 7d27 290a 2020 2020 2020 2020 2020 2020  }').            
-00000740: 2020 2020 2020 2020 6f73 2e72 656d 6f76          os.remov
-00000750: 6528 272e 2f6f 7574 7075 742f 7465 6d70  e('./output/temp
-00000760: 5f73 7461 7469 7374 6963 732f 2720 2b20  _statistics/' + 
-00000770: 7265 7375 6c74 5f66 696c 6529 0a20 2020  result_file).   
-00000780: 2020 2020 2020 2020 2020 2020 206f 7574               out
-00000790: 7075 745f 6669 6c65 2e77 7269 7465 2827  put_file.write('
-000007a0: 5c74 3c2f 7461 626c 653e 5c6e 2729 0a20  \t</table>\n'). 
-000007b0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-000007c0: 7574 7075 745f 6669 6c65 2e77 7269 7465  utput_file.write
-000007d0: 2827 3c2f 6469 763e 3c62 723e 3c62 723e  ('</div><br><br>
-000007e0: 5c6e 2729 0a20 2020 2020 2020 2020 2020  \n').           
-000007f0: 2069 6620 616e 7928 6f73 2e6c 6973 7464   if any(os.listd
-00000800: 6972 2827 2e2f 6f75 7470 7574 2f74 656d  ir('./output/tem
-00000810: 705f 6669 6775 7265 7327 2929 3a0a 2020  p_figures')):.  
-00000820: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-00000830: 675f 7479 7065 203d 206f 732e 6c69 7374  g_type = os.list
-00000840: 6469 7228 272e 2f6f 7574 7075 742f 7465  dir('./output/te
-00000850: 6d70 5f66 6967 7572 6573 2729 5b30 5d5b  mp_figures')[0][
-00000860: 3a35 5d0a 2020 2020 2020 2020 2020 2020  :5].            
-00000870: 2020 2020 666f 7220 6669 6775 7265 5f66      for figure_f
-00000880: 696c 6520 696e 206f 732e 6c69 7374 6469  ile in os.listdi
-00000890: 7228 272e 2f6f 7574 7075 742f 7465 6d70  r('./output/temp
-000008a0: 5f66 6967 7572 6573 2729 3a0a 2020 2020  _figures'):.    
-000008b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008c0: 7769 7468 206f 7065 6e28 272e 2f6f 7574  with open('./out
-000008d0: 7075 742f 7465 6d70 5f66 6967 7572 6573  put/temp_figures
-000008e0: 2f27 202b 2066 6967 7572 655f 6669 6c65  /' + figure_file
-000008f0: 2c20 2772 6227 2920 6173 2073 7667 3a0a  , 'rb') as svg:.
-00000900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000910: 2020 2020 2020 2020 6966 2066 6967 7572          if figur
-00000920: 655f 6669 6c65 5b3a 355d 2021 3d20 6669  e_file[:5] != fi
-00000930: 675f 7479 7065 3a0a 2020 2020 2020 2020  g_type:.        
-00000940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000950: 2020 2020 6f75 7470 7574 5f66 696c 652e      output_file.
-00000960: 7772 6974 6528 273c 6272 3e5c 6e27 290a  write('<br>\n').
-00000970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000980: 2020 2020 2020 2020 2020 2020 6669 675f              fig_
-00000990: 7479 7065 203d 2066 6967 7572 655f 6669  type = figure_fi
-000009a0: 6c65 5b3a 355d 0a20 2020 2020 2020 2020  le[:5].         
-000009b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000009c0: 7667 5f62 6173 6536 3420 3d20 7374 7228  vg_base64 = str(
-000009d0: 6261 7365 3634 2e62 3634 656e 636f 6465  base64.b64encode
-000009e0: 2873 7667 2e72 6561 6428 2929 2c27 7574  (svg.read()),'ut
-000009f0: 662d 3827 290a 2020 2020 2020 2020 2020  f-8').          
-00000a00: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
-00000a10: 7470 7574 5f66 696c 652e 7772 6974 6528  tput_file.write(
-00000a20: 6627 3c69 6d67 2073 7479 6c65 3d22 626f  f'<img style="bo
-00000a30: 7264 6572 2d73 7479 6c65 3a73 6f6c 6964  rder-style:solid
-00000a40: 3b20 626f 7264 6572 2d77 6964 7468 3a33  ; border-width:3
-00000a50: 7078 3b20 626f 7264 6572 2d63 6f6c 6f72  px; border-color
-00000a60: 3a23 4141 4141 4141 3b22 2073 7263 3d22  :#AAAAAA;" src="
-00000a70: 6461 7461 3a69 6d61 6765 2f73 7667 2b78  data:image/svg+x
-00000a80: 6d6c 3b62 6173 6536 342c 7b73 7667 5f62  ml;base64,{svg_b
-00000a90: 6173 6536 347d 2220 2f3e 5c6e 2729 0a20  ase64}" />\n'). 
-00000aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ab0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00000ac0: 2020 2020 2020 2020 2020 2020 6f73 2e72              os.r
-00000ad0: 656d 6f76 6528 272e 2f6f 7574 7075 742f  emove('./output/
-00000ae0: 7465 6d70 5f66 6967 7572 6573 2f27 202b  temp_figures/' +
-00000af0: 2066 6967 7572 655f 6669 6c65 290a 2020   figure_file).  
-00000b00: 2020 2020 2020 2020 2020 6f73 2e72 6d64            os.rmd
-00000b10: 6972 2827 2e2f 6f75 7470 7574 2f74 656d  ir('./output/tem
-00000b20: 705f 7265 7375 6c74 7327 290a 2020 2020  p_results').    
-00000b30: 2020 2020 2020 2020 6f73 2e72 6d64 6972          os.rmdir
-00000b40: 2827 2e2f 6f75 7470 7574 2f74 656d 705f  ('./output/temp_
-00000b50: 7374 6174 6973 7469 6373 2729 0a20 2020  statistics').   
-00000b60: 2020 2020 2020 2020 206f 732e 726d 6469           os.rmdi
-00000b70: 7228 272e 2f6f 7574 7075 742f 7465 6d70  r('./output/temp
-00000b80: 5f66 6967 7572 6573 2729 0a20 2020 200a  _figures').    .
-00000b90: 2020 2020 2020 2020 7072 696e 7428 275b          print('[
-00000ba0: 4c4f 475d 2048 544d 4c20 7265 706f 7274  LOG] HTML report
-00000bb0: 2063 7265 6174 6564 2729 0a20 2020 2065   created').    e
-00000bc0: 7863 6570 743a 0a20 2020 2020 2020 2070  xcept:.        p
-00000bd0: 7269 6e74 2827 5b45 5252 4f52 5d20 4661  rint('[ERROR] Fa
-00000be0: 696c 6564 2074 6f20 6372 6561 7465 2048  iled to create H
-00000bf0: 544d 4c20 7265 706f 7274 2729            TML report')
+00000000: 696d 706f 7274 206f 730d 0a69 6d70 6f72  import os..impor
+00000010: 7420 6261 7365 3634 0d0a 0d0a 6465 6620  t base64....def 
+00000020: 6578 706f 7274 5f72 6570 6f72 7428 4f55  export_report(OU
+00000030: 5450 5554 293a 0d0a 2020 2020 7072 696e  TPUT):..    prin
+00000040: 7428 275b 4c4f 475d 2045 7870 6f72 7469  t('[LOG] Exporti
+00000050: 6e67 2048 544d 4c20 7265 706f 7274 2729  ng HTML report')
+00000060: 0d0a 2020 2020 7472 793a 0d0a 2020 2020  ..    try:..    
+00000070: 2020 2020 7769 7468 206f 7065 6e28 4f55      with open(OU
+00000080: 5450 5554 2c20 2777 272c 2065 6e63 6f64  TPUT, 'w', encod
+00000090: 696e 673d 2275 7466 2d38 2229 2061 7320  ing="utf-8") as 
+000000a0: 6f75 7470 7574 5f66 696c 653a 0d0a 2020  output_file:..  
+000000b0: 2020 2020 2020 2020 2020 6966 2061 6e79            if any
+000000c0: 286f 732e 6c69 7374 6469 7228 272e 2f6f  (os.listdir('./o
+000000d0: 7574 7075 742f 7465 6d70 5f72 6573 756c  utput/temp_resul
+000000e0: 7473 2729 293a 0d0a 2020 2020 2020 2020  ts')):..        
+000000f0: 2020 2020 2020 2020 6f75 7470 7574 5f66          output_f
+00000100: 696c 652e 7772 6974 6528 273c 6469 7620  ile.write('<div 
+00000110: 7374 796c 653d 2264 6973 706c 6179 3a20  style="display: 
+00000120: 666c 6578 3b20 6a75 7374 6966 792d 636f  flex; justify-co
+00000130: 6e74 656e 743a 2063 656e 7465 723b 223e  ntent: center;">
+00000140: 3c68 333e 5265 7375 6c74 733c 2f68 333e  <h3>Results</h3>
+00000150: 3c2f 6469 763e 2729 0d0a 2020 2020 2020  </div>')..      
+00000160: 2020 2020 2020 2020 2020 6f75 7470 7574            output
+00000170: 5f66 696c 652e 7772 6974 6528 273c 6469  _file.write('<di
+00000180: 7620 7374 796c 653d 2264 6973 706c 6179  v style="display
+00000190: 3a20 666c 6578 3b20 6a75 7374 6966 792d  : flex; justify-
+000001a0: 636f 6e74 656e 743a 2063 656e 7465 723b  content: center;
+000001b0: 223e 5c6e 2729 0d0a 2020 2020 2020 2020  ">\n')..        
+000001c0: 2020 2020 2020 2020 6f75 7470 7574 5f66          output_f
+000001d0: 696c 652e 7772 6974 6528 275c 743c 7461  ile.write('\t<ta
+000001e0: 626c 6520 7374 796c 653d 2262 6f72 6465  ble style="borde
+000001f0: 723a 6e6f 6e65 3b20 7769 6474 683a 3330  r:none; width:30
+00000200: 253b 223e 5c6e 2729 0d0a 2020 2020 2020  %;">\n')..      
+00000210: 2020 2020 2020 2020 2020 666f 7220 7265            for re
+00000220: 7375 6c74 5f66 696c 6520 696e 206f 732e  sult_file in os.
+00000230: 6c69 7374 6469 7228 272e 2f6f 7574 7075  listdir('./outpu
+00000240: 742f 7465 6d70 5f72 6573 756c 7473 2729  t/temp_results')
+00000250: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00000260: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
+00000270: 2827 2e2f 6f75 7470 7574 2f74 656d 705f  ('./output/temp_
+00000280: 7265 7375 6c74 732f 2720 2b20 7265 7375  results/' + resu
+00000290: 6c74 5f66 696c 652c 2027 7227 2920 6173  lt_file, 'r') as
+000002a0: 2072 6573 3a0d 0a20 2020 2020 2020 2020   res:..         
+000002b0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+000002c0: 7574 7075 745f 6669 6c65 2e77 7269 7465  utput_file.write
+000002d0: 2866 277b 7265 732e 7265 6164 2829 7d27  (f'{res.read()}'
+000002e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000002f0: 2020 2020 2020 206f 732e 7265 6d6f 7665         os.remove
+00000300: 2827 2e2f 6f75 7470 7574 2f74 656d 705f  ('./output/temp_
+00000310: 7265 7375 6c74 732f 2720 2b20 7265 7375  results/' + resu
+00000320: 6c74 5f66 696c 6529 0d0a 2020 2020 2020  lt_file)..      
+00000330: 2020 2020 2020 2020 2020 6f75 7470 7574            output
+00000340: 5f66 696c 652e 7772 6974 6528 275c 743c  _file.write('\t<
+00000350: 2f74 6162 6c65 3e5c 6e27 290d 0a20 2020  /table>\n')..   
+00000360: 2020 2020 2020 2020 2020 2020 206f 7574               out
+00000370: 7075 745f 6669 6c65 2e77 7269 7465 2827  put_file.write('
+00000380: 3c2f 6469 763e 3c62 723e 3c62 723e 5c6e  </div><br><br>\n
+00000390: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
+000003a0: 6966 2061 6e79 286f 732e 6c69 7374 6469  if any(os.listdi
+000003b0: 7228 272e 2f6f 7574 7075 742f 7465 6d70  r('./output/temp
+000003c0: 5f73 7461 7469 7374 6963 7327 2929 3a0d  _statistics')):.
+000003d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000003e0: 206f 7574 7075 745f 6669 6c65 2e77 7269   output_file.wri
+000003f0: 7465 2827 3c64 6976 2073 7479 6c65 3d22  te('<div style="
+00000400: 6469 7370 6c61 793a 2066 6c65 783b 206a  display: flex; j
+00000410: 7573 7469 6679 2d63 6f6e 7465 6e74 3a20  ustify-content: 
+00000420: 6365 6e74 6572 3b22 3e3c 6833 3e53 7461  center;"><h3>Sta
+00000430: 7469 7374 6963 733c 2f68 333e 3c2f 6469  tistics</h3></di
+00000440: 763e 2729 0d0a 2020 2020 2020 2020 2020  v>')..          
+00000450: 2020 2020 2020 6f75 7470 7574 5f66 696c        output_fil
+00000460: 652e 7772 6974 6528 273c 6469 7620 7374  e.write('<div st
+00000470: 796c 653d 2264 6973 706c 6179 3a20 666c  yle="display: fl
+00000480: 6578 3b20 6a75 7374 6966 792d 636f 6e74  ex; justify-cont
+00000490: 656e 743a 2063 656e 7465 723b 223e 5c6e  ent: center;">\n
+000004a0: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
+000004b0: 2020 2020 6f75 7470 7574 5f66 696c 652e      output_file.
+000004c0: 7772 6974 6528 275c 743c 7461 626c 6520  write('\t<table 
+000004d0: 7374 796c 653d 2262 6f72 6465 723a 6e6f  style="border:no
+000004e0: 6e65 3b20 7769 6474 683a 3735 253b 223e  ne; width:75%;">
+000004f0: 5c6e 2729 0d0a 2020 2020 2020 2020 2020  \n')..          
+00000500: 2020 2020 2020 6f75 7470 7574 5f66 696c        output_fil
+00000510: 652e 7772 6974 6528 275c 745c 743c 7472  e.write('\t\t<tr
+00000520: 3e5c 6e27 290d 0a20 2020 2020 2020 2020  >\n')..         
+00000530: 2020 2020 2020 206f 7574 7075 745f 6669         output_fi
+00000540: 6c65 2e77 7269 7465 2827 5c74 5c74 5c74  le.write('\t\t\t
+00000550: 3c74 6820 7374 796c 653d 2274 6578 742d  <th style="text-
+00000560: 616c 6967 6e3a 6c65 6674 3b22 3e53 7461  align:left;">Sta
+00000570: 7469 7374 6963 3c2f 7468 3e5c 6e27 290d  tistic</th>\n').
+00000580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000590: 206f 7574 7075 745f 6669 6c65 2e77 7269   output_file.wri
+000005a0: 7465 2827 5c74 5c74 5c74 3c74 6820 7374  te('\t\t\t<th st
+000005b0: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
+000005c0: 6c65 6674 3b22 3e52 6561 6c20 6461 7461  left;">Real data
+000005d0: 7365 743c 2f74 683e 5c6e 2729 0d0a 2020  set</th>\n')..  
+000005e0: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
+000005f0: 7470 7574 5f66 696c 652e 7772 6974 6528  tput_file.write(
+00000600: 275c 745c 745c 743c 7468 2073 7479 6c65  '\t\t\t<th style
+00000610: 3d22 7465 7874 2d61 6c69 676e 3a6c 6566  ="text-align:lef
+00000620: 743b 223e 5369 6d75 6c61 7465 6420 6461  t;">Simulated da
+00000630: 7461 7365 743c 2f74 683e 5c6e 2729 0d0a  taset</th>\n')..
+00000640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000650: 6f75 7470 7574 5f66 696c 652e 7772 6974  output_file.writ
+00000660: 6528 275c 745c 743c 2f74 723e 5c6e 2729  e('\t\t</tr>\n')
+00000670: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000680: 2020 666f 7220 7265 7375 6c74 5f66 696c    for result_fil
+00000690: 6520 696e 206f 732e 6c69 7374 6469 7228  e in os.listdir(
+000006a0: 272e 2f6f 7574 7075 742f 7465 6d70 5f73  './output/temp_s
+000006b0: 7461 7469 7374 6963 7327 293a 0d0a 2020  tatistics'):..  
+000006c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006d0: 2020 7769 7468 206f 7065 6e28 272e 2f6f    with open('./o
+000006e0: 7574 7075 742f 7465 6d70 5f73 7461 7469  utput/temp_stati
+000006f0: 7374 6963 732f 2720 2b20 7265 7375 6c74  stics/' + result
+00000700: 5f66 696c 652c 2027 7227 2920 6173 2072  _file, 'r') as r
+00000710: 6573 3a0d 0a20 2020 2020 2020 2020 2020  es:..           
+00000720: 2020 2020 2020 2020 2020 2020 206f 7574               out
+00000730: 7075 745f 6669 6c65 2e77 7269 7465 2866  put_file.write(f
+00000740: 277b 7265 732e 7265 6164 2829 7d27 290d  '{res.read()}').
+00000750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000760: 2020 2020 206f 732e 7265 6d6f 7665 2827       os.remove('
+00000770: 2e2f 6f75 7470 7574 2f74 656d 705f 7374  ./output/temp_st
+00000780: 6174 6973 7469 6373 2f27 202b 2072 6573  atistics/' + res
+00000790: 756c 745f 6669 6c65 290d 0a20 2020 2020  ult_file)..     
+000007a0: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
+000007b0: 745f 6669 6c65 2e77 7269 7465 2827 5c74  t_file.write('\t
+000007c0: 3c2f 7461 626c 653e 5c6e 2729 0d0a 2020  </table>\n')..  
+000007d0: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
+000007e0: 7470 7574 5f66 696c 652e 7772 6974 6528  tput_file.write(
+000007f0: 273c 2f64 6976 3e3c 6272 3e3c 6272 3e5c  '</div><br><br>\
+00000800: 6e27 290d 0a20 2020 2020 2020 2020 2020  n')..           
+00000810: 2069 6620 616e 7928 6f73 2e6c 6973 7464   if any(os.listd
+00000820: 6972 2827 2e2f 6f75 7470 7574 2f74 656d  ir('./output/tem
+00000830: 705f 6669 6775 7265 7327 2929 3a0d 0a20  p_figures')):.. 
+00000840: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00000850: 6967 5f74 7970 6520 3d20 6f73 2e6c 6973  ig_type = os.lis
+00000860: 7464 6972 2827 2e2f 6f75 7470 7574 2f74  tdir('./output/t
+00000870: 656d 705f 6669 6775 7265 7327 295b 305d  emp_figures')[0]
+00000880: 5b3a 355d 0d0a 2020 2020 2020 2020 2020  [:5]..          
+00000890: 2020 2020 2020 666f 7220 6669 6775 7265        for figure
+000008a0: 5f66 696c 6520 696e 206f 732e 6c69 7374  _file in os.list
+000008b0: 6469 7228 272e 2f6f 7574 7075 742f 7465  dir('./output/te
+000008c0: 6d70 5f66 6967 7572 6573 2729 3a0d 0a20  mp_figures'):.. 
+000008d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008e0: 2020 2077 6974 6820 6f70 656e 2827 2e2f     with open('./
+000008f0: 6f75 7470 7574 2f74 656d 705f 6669 6775  output/temp_figu
+00000900: 7265 732f 2720 2b20 6669 6775 7265 5f66  res/' + figure_f
+00000910: 696c 652c 2027 7262 2729 2061 7320 7376  ile, 'rb') as sv
+00000920: 673a 0d0a 2020 2020 2020 2020 2020 2020  g:..            
+00000930: 2020 2020 2020 2020 2020 2020 6966 2066              if f
+00000940: 6967 7572 655f 6669 6c65 5b3a 355d 2021  igure_file[:5] !
+00000950: 3d20 6669 675f 7479 7065 3a0d 0a20 2020  = fig_type:..   
+00000960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000970: 2020 2020 2020 2020 206f 7574 7075 745f           output_
+00000980: 6669 6c65 2e77 7269 7465 2827 3c62 723e  file.write('<br>
+00000990: 5c6e 2729 0d0a 2020 2020 2020 2020 2020  \n')..          
+000009a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009b0: 2020 6669 675f 7479 7065 203d 2066 6967    fig_type = fig
+000009c0: 7572 655f 6669 6c65 5b3a 355d 0d0a 2020  ure_file[:5]..  
+000009d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009e0: 2020 2020 2020 7376 675f 6261 7365 3634        svg_base64
+000009f0: 203d 2073 7472 2862 6173 6536 342e 6236   = str(base64.b6
+00000a00: 3465 6e63 6f64 6528 7376 672e 7265 6164  4encode(svg.read
+00000a10: 2829 292c 2775 7466 2d38 2729 0d0a 2020  ()),'utf-8')..  
+00000a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a30: 2020 2020 2020 6f75 7470 7574 5f66 696c        output_fil
+00000a40: 652e 7772 6974 6528 6627 3c69 6d67 2073  e.write(f'<img s
+00000a50: 7479 6c65 3d22 626f 7264 6572 2d73 7479  tyle="border-sty
+00000a60: 6c65 3a73 6f6c 6964 3b20 626f 7264 6572  le:solid; border
+00000a70: 2d77 6964 7468 3a33 7078 3b20 626f 7264  -width:3px; bord
+00000a80: 6572 2d63 6f6c 6f72 3a23 4141 4141 4141  er-color:#AAAAAA
+00000a90: 3b22 2073 7263 3d22 6461 7461 3a69 6d61  ;" src="data:ima
+00000aa0: 6765 2f73 7667 2b78 6d6c 3b62 6173 6536  ge/svg+xml;base6
+00000ab0: 342c 7b73 7667 5f62 6173 6536 347d 2220  4,{svg_base64}" 
+00000ac0: 2f3e 5c6e 2729 0d0a 2020 2020 2020 2020  />\n')..        
+00000ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ae0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000af0: 2020 2020 2020 6f73 2e72 656d 6f76 6528        os.remove(
+00000b00: 272e 2f6f 7574 7075 742f 7465 6d70 5f66  './output/temp_f
+00000b10: 6967 7572 6573 2f27 202b 2066 6967 7572  igures/' + figur
+00000b20: 655f 6669 6c65 290d 0a20 2020 2020 2020  e_file)..       
+00000b30: 2020 2020 206f 732e 726d 6469 7228 272e       os.rmdir('.
+00000b40: 2f6f 7574 7075 742f 7465 6d70 5f72 6573  /output/temp_res
+00000b50: 756c 7473 2729 0d0a 2020 2020 2020 2020  ults')..        
+00000b60: 2020 2020 6f73 2e72 6d64 6972 2827 2e2f      os.rmdir('./
+00000b70: 6f75 7470 7574 2f74 656d 705f 7374 6174  output/temp_stat
+00000b80: 6973 7469 6373 2729 0d0a 2020 2020 2020  istics')..      
+00000b90: 2020 2020 2020 6f73 2e72 6d64 6972 2827        os.rmdir('
+00000ba0: 2e2f 6f75 7470 7574 2f74 656d 705f 6669  ./output/temp_fi
+00000bb0: 6775 7265 7327 290d 0a20 2020 200d 0a20  gures')..    .. 
+00000bc0: 2020 2020 2020 2070 7269 6e74 2827 5b4c         print('[L
+00000bd0: 4f47 5d20 4854 4d4c 2072 6570 6f72 7420  OG] HTML report 
+00000be0: 6372 6561 7465 6427 290d 0a20 2020 2065  created')..    e
+00000bf0: 7863 6570 743a 0d0a 2020 2020 2020 2020  xcept:..        
+00000c00: 7072 696e 7428 275b 4552 524f 525d 2046  print('[ERROR] F
+00000c10: 6169 6c65 6420 746f 2063 7265 6174 6520  ailed to create 
+00000c20: 4854 4d4c 2072 6570 6f72 7427 29         HTML report')
```

### Comparing `evalAIRR-0.0.8/evalAIRR/util/univar.py` & `evalAIRR-0.0.9/evalAIRR/util/univar.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,387 +1,387 @@
-import matplotlib.pyplot as plt
-import seaborn as sns
-import numpy as np
-import scipy.stats
-
-def cdf(data):
-    data_sorted = np.sort(data)
-    p = 1. * np.arange(len(data)) / (len(data) - 1)
-    return data_sorted, np.array(p)
-
-def get_feature_data(feature, data, features):
-    idx = np.where(features == feature)[0][0]
-    if not idx:
-        print(f'[ERROR] Feature {feature} not found!')
-        return np.array([])
-    return data[:, idx].flatten()
-
-def get_observation_data(observation_index, data):
-    if observation_index < 0 or observation_index >= len(data):
-        print(f'[ERROR] Observation with index {observation_index} does not exist!')
-        return np.array([])
-    return data[observation_index, :].flatten()
-
-def export_ks_test(feature, data_R, data_S, features_R, features_S):
-    data_R_f = get_feature_data(feature, data_R, features_R)
-    data_S_f = get_feature_data(feature, data_S, features_S)
-    if not any(data_R_f) or not any(data_S_f):
-        return
-
-    cdf_1_x, cdf_1_y = cdf(data_R_f)
-    cdf_2_x, cdf_2_y = cdf(data_S_f)
-    res = scipy.stats.ks_2samp(data_R_f, data_S_f)
-    
-    f, ax = plt.subplots(1, 1)
-    f.set_size_inches(5, 5)
-    f.suptitle(f'CDF comparison of feature {feature}\nin real and simulated datasets')
-    ax.plot(cdf_1_x, cdf_1_y, c='#1b24a8', label='Real dataset')
-    ax.plot(cdf_2_x, cdf_2_y, c='r', label='Simulated dataset')
-    ax.grid(visible=True)
-    ax.legend()
-    
-    print(f'[RESULT] Feature {feature} KS statistic =', res.statistic)
-    print(f'[RESULT] Feature {feature} P value =', res.pvalue)
-    with open(f'./output/temp_results/ks_test_{feature}.txt', 'w', encoding="utf-8") as file:
-        file.write('\t\t<tr colspan="2">\n')
-        file.write(f'\t\t\t<td>Feature {feature} KS statistic</td>\n')
-        file.write(f'\t\t\t<td>{res.statistic}</td>\n')
-        file.write('\t\t</tr>\n')
-
-        file.write('\t\t<tr colspan="2">\n')
-        file.write(f'\t\t\t<td>Feature {feature} P value</td>\n')
-        file.write(f'\t\t\t<td>{res.pvalue}</td>\n')
-        file.write('\t\t</tr>\n')
-
-    f.savefig(f'./output/temp_figures/ks_test_{feature}.svg')
-    del f
-    plt.close()
-
-def export_distr_histogram(feature, data_R, data_S, features_R, features_S, n_bins=30):
-    data_R_f = get_feature_data(feature, data_R, features_R)
-    data_S_f = get_feature_data(feature, data_S, features_S)
-    if not any(data_R_f) or not any(data_S_f):
-        return
-
-    bins = np.linspace(min(min(data_R_f), min(data_S_f)), max(max(data_R_f), max(data_S_f)), n_bins)
-
-    f, ax = plt.subplots(1, 1)
-    f.set_size_inches(9, 7)
-    f.suptitle(f'Distribution histograms of feature {feature}')
-    ax.hist([data_R_f, data_S_f], bins, label=['Real dataset', 'Simulated dataset'])
-    ax.legend(loc='upper right')
-    
-    f.savefig(f'./output/temp_figures/histogram_{feature}.svg')
-    del f
-    plt.close()
-
-def export_obs_distr_histogram(observation_index, data_R, data_S, n_bins=30):
-    if observation_index == 'all':
-        print('[ERROR] Observation distribution histogram report does not support the visualization of all observations')
-        return
-    data_R_o = get_observation_data(observation_index, data_R)
-    data_S_o = get_observation_data(observation_index, data_S)
-    if not any(data_R_o) or not any(data_S_o):
-        return
-
-    bins = np.linspace(min(min(data_R_o), min(data_S_o)), max(max(data_R_o), max(data_S_o)), n_bins)
-
-    f, ax = plt.subplots(1, 1)
-    f.set_size_inches(9, 7)
-    f.suptitle(f'Distribution histograms of observation with index {observation_index}')
-    ax.hist([data_R_o, data_S_o], bins, label=['Real dataset', 'Simulated dataset'])
-    ax.legend(loc='upper right')
-    
-    f.savefig(f'./output/temp_figures/histogram_obs_{observation_index}.svg')
-    del f
-    plt.close()
-
-def export_distr_boxplot(feature, data_R, data_S, features_R, features_S):
-    data_R_f = get_feature_data(feature, data_R, features_R)
-    data_S_f = get_feature_data(feature, data_S, features_S)
-    if not any(data_R_f) or not any(data_S_f):
-        return
-
-    f, ax = plt.subplots(1, 1)
-    f.set_size_inches(9, 7)
-    f.suptitle(f'Distribution boxplots of feature {feature}')
-    ax.boxplot([data_R_f, data_S_f], labels=['Real dataset', 'Simulated dataset'])
-    
-    f.savefig(f'./output/temp_figures/box_plot_{feature}.svg')
-    del f
-    plt.close()
-
-def export_obs_distr_boxplot(observation_index, data_R, data_S):
-    if observation_index == 'all':
-        print('[ERROR] Observation distribution box plot report does not support the visualization of all observations')
-        return
-    data_R_o = get_observation_data(observation_index, data_R)
-    data_S_o = get_observation_data(observation_index, data_S)
-    if not any(data_R_o) or not any(data_S_o):
-        return
-
-    f, ax = plt.subplots(1, 1)
-    f.set_size_inches(9, 7)
-    f.suptitle(f'Distribution boxplots of observation with index {observation_index}')
-    ax.boxplot([data_R_o, data_S_o], labels=['Real dataset', 'Simulated dataset'])
-    
-    f.savefig(f'./output/temp_figures/box_plot_obs_{observation_index}.svg')
-    del f
-    plt.close()
-
-def export_distr_violinplot(feature, data_R, data_S, features_R, features_S):
-    data_R_f = get_feature_data(feature, data_R, features_R)
-    data_S_f = get_feature_data(feature, data_S, features_S)
-    if not any(data_R_f) or not any(data_S_f):
-        return
-
-    f, [ax1, ax2] = plt.subplots(2, 1)
-    f.set_size_inches(9, 7)
-    f.suptitle(f'Distribution violin plots of feature {feature}')
-    ax1.violinplot(data_R_f, vert=False, widths=0.7,
-                     showmeans=True, showextrema=True, showmedians=True)
-    ax1.set_title('Real dataset')
-    ax1.set_yticklabels([])
-    ax1.set_yticks([])
-    ax1.set
-    ax2.violinplot(data_S_f, vert=False, widths=0.7,
-                     showmeans=True, showextrema=True, showmedians=True)
-    ax2.set_title('Simulated dataset')
-    ax2.set_yticklabels([])
-    ax2.set_yticks([])
-
-    xbound = (min(ax1.get_xbound()[0], ax2.get_xbound()[0]), max(ax1.get_xbound()[1], ax2.get_xbound()[1]))
-    ybound = (min(ax1.get_ybound()[0], ax2.get_ybound()[0]), max(ax1.get_ybound()[1], ax2.get_ybound()[1]))
-
-    ax1.set_xbound(xbound)
-    ax1.set_ybound(ybound)
-    ax2.set_xbound(xbound)
-    ax2.set_ybound(ybound)
-
-    f.savefig(f'./output/temp_figures/violin_plot_{feature}.svg')
-    del f
-    plt.close()
-
-def export_obs_distr_violinplot(observation_index, data_R, data_S):
-    if observation_index == 'all':
-        print('[ERROR] Observation distribution violin plot report does not support the visualization of all observations')
-        return
-    data_R_o = get_observation_data(observation_index, data_R)
-    data_S_o = get_observation_data(observation_index, data_S)
-    if not any(data_R_o) or not any(data_S_o):
-        return
-    
-    f, [ax1, ax2] = plt.subplots(2, 1)
-    f.set_size_inches(9, 7)
-    f.suptitle(f'Distribution violin plots of observation with index {observation_index}')
-    ax1.violinplot(data_R_o, vert=False, widths=0.7,
-                     showmeans=True, showextrema=True, showmedians=True)
-    ax1.set_title('Real dataset')
-    ax1.set_yticklabels([])
-    ax1.set_yticks([])
-    ax1.set
-    ax2.violinplot(data_S_o, vert=False, widths=0.7,
-                     showmeans=True, showextrema=True, showmedians=True)
-    ax2.set_title('Simulated dataset')
-    ax2.set_yticklabels([])
-    ax2.set_yticks([])
-
-    xbound = (min(ax1.get_xbound()[0], ax2.get_xbound()[0]), max(ax1.get_xbound()[1], ax2.get_xbound()[1]))
-    ybound = (min(ax1.get_ybound()[0], ax2.get_ybound()[0]), max(ax1.get_ybound()[1], ax2.get_ybound()[1]))
-
-    ax1.set_xbound(xbound)
-    ax1.set_ybound(ybound)
-    ax2.set_xbound(xbound)
-    ax2.set_ybound(ybound)
-
-    f.savefig(f'./output/temp_figures/violin_plot_obs_{observation_index}.svg')
-    del f
-    plt.close()
-
-def export_distr_densityplot(feature, data_R, data_S, features_R, features_S):
-    data_R_f = get_feature_data(feature, data_R, features_R)
-    data_S_f = get_feature_data(feature, data_S, features_S)
-    if not any(data_R_f) or not any(data_S_f):
-        return
-
-    f, ax = plt.subplots(1, 1)
-    f.set_size_inches(9, 7)
-    f.suptitle(f'Distribution density plot of feature {feature}')
-    sns.kdeplot(data_R_f, ax=ax, label='Real dataset', fill=True, common_norm=False, color='#5480d1', alpha=0.5, linewidth=0)
-    sns.kdeplot(data_S_f, ax=ax, label='Simulated dataset', fill=True, common_norm=False, color='#d65161', alpha=0.5, linewidth=0)
-    ax.legend()
-
-    f.savefig(f'./output/temp_figures/density_plot_{feature}.svg')
-    del f
-    plt.close()
-
-def export_obs_distr_densityplot(observation_index, data_R, data_S):
-    if observation_index != 'all':
-        data_R_o = get_observation_data(observation_index, data_R)
-        data_S_o = get_observation_data(observation_index, data_S)
-        if not any(data_R_o) or not any(data_S_o):
-            return
-
-    f, ax = plt.subplots(1, 1)
-    f.set_size_inches(9, 7)
-    
-    if observation_index == 'all':
-        f.suptitle(f'Distribution density plot of all observations')
-        for index in range(len(data_R)):
-            data_R_o = get_observation_data(index, data_R)
-            data_S_o = get_observation_data(index, data_S)
-            label = 'Real dataset' if index == 0 else None
-            sns.kdeplot(data_R_o, ax=ax, label=label, fill=True, common_norm=False, color='#5480d1', alpha=0.2, linewidth=0)
-            label = 'Simulated dataset' if index == 0 else None
-            sns.kdeplot(data_S_o, ax=ax, label=label, fill=True, common_norm=False, color='#d65161', alpha=0.2, linewidth=0)
-    else:
-        f.suptitle(f'Distribution density plot of observation with index {observation_index}')
-        sns.kdeplot(data_R_o, ax=ax, label='Real dataset', fill=True, common_norm=False, color='#5480d1', alpha=0.5, linewidth=0)
-        sns.kdeplot(data_S_o, ax=ax, label='Simulated dataset', fill=True, common_norm=False, color='#d65161', alpha=0.5, linewidth=0)
-
-    ax.legend()
-    f.savefig(f'./output/temp_figures/density_plot_obs_{observation_index}.svg')
-    del f
-    plt.close()
-
-def export_avg_var_scatter_plot(data_R, data_S, axis=0):
-    data_R_x = np.average(data_R, axis=axis)
-    data_R_y = np.var(data_R, axis=axis)
-    data_S_x = np.average(data_S, axis=axis)
-    data_S_y = np.var(data_S, axis=axis)
-
-    f, ax = plt.subplots(1, 1)
-    f.set_size_inches(9, 7)
-    f.suptitle('Feature average value vs variance' if axis == 0 else 'Observation average value vs variance')
-    ax.scatter(data_R_x, data_R_y, c='#5480d1', linewidths=None, alpha=0.5, label='Real')
-    ax.scatter(data_S_x, data_S_y, c='#d65161', linewidths=None, alpha=0.5, label='Simulated')
-    ax.set_xlabel('Average value')
-    ax.set_ylabel('Variance value')
-    ax.legend()
-    
-    f.savefig(f'./output/temp_figures/avg_var_{"feat" if axis == 0 else "obs"}_scatter_plot.svg')
-    del f
-    plt.close()
-
-def export_distance(feature, data_R, data_S, features_R, features_S):
-    data_R_f = get_feature_data(feature, data_R, features_R)
-    data_S_f = get_feature_data(feature, data_S, features_S)
-    if not any(data_R_f) or not any(data_S_f):
-        return
-
-    dist = np.linalg.norm(data_R_f - data_S_f)
-    print(f'[RESULT] Euclidean distance of feature {feature} : {dist}')
-
-    with open(f'./output/temp_results/distance_{feature}.txt', 'w', encoding="utf-8") as file:
-        file.write('\t\t<tr colspan="2">\n')
-        file.write(f'\t\t\t<td>Euclidean distance of feature {feature}</td>\n')
-        file.write(f'\t\t\t<td>{dist}</td>\n')
-        file.write('\t\t</tr>\n')
-
-def export_obs_distance(observation_index, data_R, data_S):
-    if observation_index == 'all':
-        print('[ERROR] Observation Euclidean distance report does not support reporting on all observations')
-        return
-    data_R_o = get_observation_data(observation_index, data_R)
-    data_S_o = get_observation_data(observation_index, data_S)
-    if not any(data_R_o) or not any(data_S_o):
-        return
-
-    dist = []
-    if data_S_o.shape[0] < data_R_o.shape[0]:
-        data_S_o_padded = np.zeros(data_R_o.shape)
-        data_S_o_padded[:data_S_o.shape[0]] = data_S_o
-        dist = np.linalg.norm(data_R_o - data_S_o_padded)
-    elif data_R_o.shape[0] < data_S_o.shape[0]:
-        data_R_o_padded = np.zeros(data_S_o.shape)
-        data_R_o_padded[:data_R_o.shape[0]] = data_R_o
-        dist = np.linalg.norm(data_S_o - data_R_o_padded)
-    else:
-        dist = np.linalg.norm(data_R_o - data_S_o)
-
-    print(f'[RESULT] Euclidean distance of observation with index {observation_index} : {dist}')
-
-    with open(f'./output/temp_results/distance_obs_{observation_index}.txt', 'w', encoding="utf-8") as file:
-        file.write('\t\t<tr colspan="2">\n')
-        file.write(f'\t\t\t<td>Euclidean distance of observation with index {observation_index}</td>\n')
-        file.write(f'\t\t\t<td>{dist}</td>\n')
-        file.write('\t\t</tr>\n')
-    
-def export_statistics(feature, data_R, data_S, features_R, features_S):
-    data_R_f = get_feature_data(feature, data_R, features_R)
-    data_S_f = get_feature_data(feature, data_S, features_S)
-    if not any(data_R_f) or not any(data_S_f):
-        return
-
-    avg = { 'real': np.average(data_R_f), 'sim': np.average(data_S_f)}
-    median = { 'real': np.median(data_R_f), 'sim': np.median(data_S_f)}
-    std = { 'real': np.std(data_R_f), 'sim': np.std(data_S_f)}
-    var = { 'real': np.var(data_R_f), 'sim': np.var(data_S_f)}
-
-    print('[RESULT] Average of feature {0:>16} : REAL = {1:>25}, SIMULATED = {2:>25}'.format(feature, avg['real'], avg['sim']))
-    print('[RESULT] Median of feature {0:>17} : REAL = {1:>25}, SIMULATED = {2:>25}'.format(feature, median['real'], median['sim']))
-    print('[RESULT] Standard deviation of feature {0:>5} : REAL = {1:>25}, SIMULATED = {2:>25}'.format(feature, std['real'], std['sim']))
-    print('[RESULT] Variance of feature {0:>15} : REAL = {1:>25}, SIMULATED = {2:>25}'.format(feature, var['real'], var['sim']))
-
-    with open(f'./output/temp_statistics/{feature}.txt', 'w', encoding="utf-8") as file:
-        file.write('\t\t<tr>\n')
-        file.write(f'\t\t\t<td>Average of feature {feature}</td>\n')
-        file.write(f'\t\t\t<td>{avg["real"]}</td>\n')
-        file.write(f'\t\t\t<td>{avg["sim"]}</td>\n')
-        file.write('\t\t</tr>\n')
-        file.write('\t\t<tr>\n')
-        file.write(f'\t\t\t<td>Median of feature {feature}</td>\n')
-        file.write(f'\t\t\t<td>{median["real"]}</td>\n')
-        file.write(f'\t\t\t<td>{median["sim"]}</td>\n')
-        file.write('\t\t</tr>\n')
-        file.write('\t\t<tr>\n')
-        file.write(f'\t\t\t<td>Standard deviation of feature {feature}</td>\n')
-        file.write(f'\t\t\t<td>{std["real"]}</td>\n')
-        file.write(f'\t\t\t<td>{std["sim"]}</td>\n')
-        file.write('\t\t</tr>\n')
-        file.write('\t\t<tr>\n')
-        file.write(f'\t\t\t<td>Variance of feature {feature}</td>\n')
-        file.write(f'\t\t\t<td>{var["real"]}</td>\n')
-        file.write(f'\t\t\t<td>{var["sim"]}</td>\n')
-        file.write('\t\t</tr>\n')
-
-def export_obs_statistics(observation_index, data_R, data_S):
-    if observation_index == 'all':
-        print('[ERROR] Observation statistics report does not support reporting on all observations')
-        return
-    data_R_o = get_observation_data(observation_index, data_R)
-    data_S_o = get_observation_data(observation_index, data_S)
-    if not any(data_R_o) or not any(data_S_o):
-        return
-
-    avg = { 'real': np.average(data_R_o), 'sim': np.average(data_S_o)}
-    median = { 'real': np.median(data_R_o), 'sim': np.median(data_S_o)}
-    std = { 'real': np.std(data_R_o), 'sim': np.std(data_S_o)}
-    var = { 'real': np.var(data_R_o), 'sim': np.var(data_S_o)}
-
-    print('[RESULT] Average of observation with index {0:>16} : REAL = {1:>25}, SIMULATED = {2:>25}'.format(observation_index, avg['real'], avg['sim']))
-    print('[RESULT] Median of observation with index {0:>17} : REAL = {1:>25}, SIMULATED = {2:>25}'.format(observation_index, median['real'], median['sim']))
-    print('[RESULT] Standard deviation of observation with index {0:>5} : REAL = {1:>25}, SIMULATED = {2:>25}'.format(observation_index, std['real'], std['sim']))
-    print('[RESULT] Variance of observation with index {0:>15} : REAL = {1:>25}, SIMULATED = {2:>25}'.format(observation_index, var['real'], var['sim']))
-
-    with open(f'./output/temp_statistics/obs_{observation_index}.txt', 'w', encoding="utf-8") as file:
-        file.write('\t\t<tr>\n')
-        file.write(f'\t\t\t<td>Average of observation with index {observation_index}</td>\n')
-        file.write(f'\t\t\t<td>{avg["real"]}</td>\n')
-        file.write(f'\t\t\t<td>{avg["sim"]}</td>\n')
-        file.write('\t\t</tr>\n')
-        file.write('\t\t<tr>\n')
-        file.write(f'\t\t\t<td>Median of observation with index {observation_index}</td>\n')
-        file.write(f'\t\t\t<td>{median["real"]}</td>\n')
-        file.write(f'\t\t\t<td>{median["sim"]}</td>\n')
-        file.write('\t\t</tr>\n')
-        file.write('\t\t<tr>\n')
-        file.write(f'\t\t\t<td>Standard deviation of observation with index {observation_index}</td>\n')
-        file.write(f'\t\t\t<td>{std["real"]}</td>\n')
-        file.write(f'\t\t\t<td>{std["sim"]}</td>\n')
-        file.write('\t\t</tr>\n')
-        file.write('\t\t<tr>\n')
-        file.write(f'\t\t\t<td>Variance of observation with index {observation_index}</td>\n')
-        file.write(f'\t\t\t<td>{var["real"]}</td>\n')
-        file.write(f'\t\t\t<td>{var["sim"]}</td>\n')
-        file.write('\t\t</tr>\n')
+import matplotlib.pyplot as plt
+import seaborn as sns
+import numpy as np
+import scipy.stats
+
+def cdf(data):
+    data_sorted = np.sort(data)
+    p = 1. * np.arange(len(data)) / (len(data) - 1)
+    return data_sorted, np.array(p)
+
+def get_feature_data(feature, data, features):
+    idx = np.where(features == feature)[0][0]
+    if not idx:
+        print(f'[ERROR] Feature {feature} not found!')
+        return np.array([])
+    return data[:, idx].flatten()
+
+def get_observation_data(observation_index, data):
+    if observation_index < 0 or observation_index >= len(data):
+        print(f'[ERROR] Observation with index {observation_index} does not exist!')
+        return np.array([])
+    return data[observation_index, :].flatten()
+
+def export_ks_test(feature, data_R, data_S, features_R, features_S):
+    data_R_f = get_feature_data(feature, data_R, features_R)
+    data_S_f = get_feature_data(feature, data_S, features_S)
+    if not any(data_R_f) or not any(data_S_f):
+        return
+
+    cdf_1_x, cdf_1_y = cdf(data_R_f)
+    cdf_2_x, cdf_2_y = cdf(data_S_f)
+    res = scipy.stats.ks_2samp(data_R_f, data_S_f)
+    
+    f, ax = plt.subplots(1, 1)
+    f.set_size_inches(5, 5)
+    f.suptitle(f'CDF comparison of feature {feature}\nin real and simulated datasets')
+    ax.plot(cdf_1_x, cdf_1_y, c='#1b24a8', label='Real dataset')
+    ax.plot(cdf_2_x, cdf_2_y, c='r', label='Simulated dataset')
+    ax.grid(visible=True)
+    ax.legend()
+    
+    print(f'[RESULT] Feature {feature} KS statistic =', res.statistic)
+    print(f'[RESULT] Feature {feature} P value =', res.pvalue)
+    with open(f'./output/temp_results/ks_test_{feature}.txt', 'w', encoding="utf-8") as file:
+        file.write('\t\t<tr colspan="2">\n')
+        file.write(f'\t\t\t<td>Feature {feature} KS statistic</td>\n')
+        file.write(f'\t\t\t<td>{res.statistic}</td>\n')
+        file.write('\t\t</tr>\n')
+
+        file.write('\t\t<tr colspan="2">\n')
+        file.write(f'\t\t\t<td>Feature {feature} P value</td>\n')
+        file.write(f'\t\t\t<td>{res.pvalue}</td>\n')
+        file.write('\t\t</tr>\n')
+
+    f.savefig(f'./output/temp_figures/ks_test_{feature}.svg')
+    del f
+    plt.close()
+
+def export_distr_histogram(feature, data_R, data_S, features_R, features_S, n_bins=30):
+    data_R_f = get_feature_data(feature, data_R, features_R)
+    data_S_f = get_feature_data(feature, data_S, features_S)
+    if not any(data_R_f) or not any(data_S_f):
+        return
+
+    bins = np.linspace(min(min(data_R_f), min(data_S_f)), max(max(data_R_f), max(data_S_f)), n_bins)
+
+    f, ax = plt.subplots(1, 1)
+    f.set_size_inches(9, 7)
+    f.suptitle(f'Distribution histograms of feature {feature}')
+    ax.hist([data_R_f, data_S_f], bins, label=['Real dataset', 'Simulated dataset'])
+    ax.legend(loc='upper right')
+    
+    f.savefig(f'./output/temp_figures/histogram_{feature}.svg')
+    del f
+    plt.close()
+
+def export_obs_distr_histogram(observation_index, data_R, data_S, n_bins=30):
+    if observation_index == 'all':
+        print('[ERROR] Observation distribution histogram report does not support the visualization of all observations')
+        return
+    data_R_o = get_observation_data(observation_index, data_R)
+    data_S_o = get_observation_data(observation_index, data_S)
+    if not any(data_R_o) or not any(data_S_o):
+        return
+
+    bins = np.linspace(min(min(data_R_o), min(data_S_o)), max(max(data_R_o), max(data_S_o)), n_bins)
+
+    f, ax = plt.subplots(1, 1)
+    f.set_size_inches(9, 7)
+    f.suptitle(f'Distribution histograms of observation with index {observation_index}')
+    ax.hist([data_R_o, data_S_o], bins, label=['Real dataset', 'Simulated dataset'])
+    ax.legend(loc='upper right')
+    
+    f.savefig(f'./output/temp_figures/histogram_obs_{observation_index}.svg')
+    del f
+    plt.close()
+
+def export_distr_boxplot(feature, data_R, data_S, features_R, features_S):
+    data_R_f = get_feature_data(feature, data_R, features_R)
+    data_S_f = get_feature_data(feature, data_S, features_S)
+    if not any(data_R_f) or not any(data_S_f):
+        return
+
+    f, ax = plt.subplots(1, 1)
+    f.set_size_inches(9, 7)
+    f.suptitle(f'Distribution boxplots of feature {feature}')
+    ax.boxplot([data_R_f, data_S_f], labels=['Real dataset', 'Simulated dataset'])
+    
+    f.savefig(f'./output/temp_figures/box_plot_{feature}.svg')
+    del f
+    plt.close()
+
+def export_obs_distr_boxplot(observation_index, data_R, data_S):
+    if observation_index == 'all':
+        print('[ERROR] Observation distribution box plot report does not support the visualization of all observations')
+        return
+    data_R_o = get_observation_data(observation_index, data_R)
+    data_S_o = get_observation_data(observation_index, data_S)
+    if not any(data_R_o) or not any(data_S_o):
+        return
+
+    f, ax = plt.subplots(1, 1)
+    f.set_size_inches(9, 7)
+    f.suptitle(f'Distribution boxplots of observation with index {observation_index}')
+    ax.boxplot([data_R_o, data_S_o], labels=['Real dataset', 'Simulated dataset'])
+    
+    f.savefig(f'./output/temp_figures/box_plot_obs_{observation_index}.svg')
+    del f
+    plt.close()
+
+def export_distr_violinplot(feature, data_R, data_S, features_R, features_S):
+    data_R_f = get_feature_data(feature, data_R, features_R)
+    data_S_f = get_feature_data(feature, data_S, features_S)
+    if not any(data_R_f) or not any(data_S_f):
+        return
+
+    f, [ax1, ax2] = plt.subplots(2, 1)
+    f.set_size_inches(9, 7)
+    f.suptitle(f'Distribution violin plots of feature {feature}')
+    ax1.violinplot(data_R_f, vert=False, widths=0.7,
+                     showmeans=True, showextrema=True, showmedians=True)
+    ax1.set_title('Real dataset')
+    ax1.set_yticklabels([])
+    ax1.set_yticks([])
+    ax1.set
+    ax2.violinplot(data_S_f, vert=False, widths=0.7,
+                     showmeans=True, showextrema=True, showmedians=True)
+    ax2.set_title('Simulated dataset')
+    ax2.set_yticklabels([])
+    ax2.set_yticks([])
+
+    xbound = (min(ax1.get_xbound()[0], ax2.get_xbound()[0]), max(ax1.get_xbound()[1], ax2.get_xbound()[1]))
+    ybound = (min(ax1.get_ybound()[0], ax2.get_ybound()[0]), max(ax1.get_ybound()[1], ax2.get_ybound()[1]))
+
+    ax1.set_xbound(xbound)
+    ax1.set_ybound(ybound)
+    ax2.set_xbound(xbound)
+    ax2.set_ybound(ybound)
+
+    f.savefig(f'./output/temp_figures/violin_plot_{feature}.svg')
+    del f
+    plt.close()
+
+def export_obs_distr_violinplot(observation_index, data_R, data_S):
+    if observation_index == 'all':
+        print('[ERROR] Observation distribution violin plot report does not support the visualization of all observations')
+        return
+    data_R_o = get_observation_data(observation_index, data_R)
+    data_S_o = get_observation_data(observation_index, data_S)
+    if not any(data_R_o) or not any(data_S_o):
+        return
+    
+    f, [ax1, ax2] = plt.subplots(2, 1)
+    f.set_size_inches(9, 7)
+    f.suptitle(f'Distribution violin plots of observation with index {observation_index}')
+    ax1.violinplot(data_R_o, vert=False, widths=0.7,
+                     showmeans=True, showextrema=True, showmedians=True)
+    ax1.set_title('Real dataset')
+    ax1.set_yticklabels([])
+    ax1.set_yticks([])
+    ax1.set
+    ax2.violinplot(data_S_o, vert=False, widths=0.7,
+                     showmeans=True, showextrema=True, showmedians=True)
+    ax2.set_title('Simulated dataset')
+    ax2.set_yticklabels([])
+    ax2.set_yticks([])
+
+    xbound = (min(ax1.get_xbound()[0], ax2.get_xbound()[0]), max(ax1.get_xbound()[1], ax2.get_xbound()[1]))
+    ybound = (min(ax1.get_ybound()[0], ax2.get_ybound()[0]), max(ax1.get_ybound()[1], ax2.get_ybound()[1]))
+
+    ax1.set_xbound(xbound)
+    ax1.set_ybound(ybound)
+    ax2.set_xbound(xbound)
+    ax2.set_ybound(ybound)
+
+    f.savefig(f'./output/temp_figures/violin_plot_obs_{observation_index}.svg')
+    del f
+    plt.close()
+
+def export_distr_densityplot(feature, data_R, data_S, features_R, features_S):
+    data_R_f = get_feature_data(feature, data_R, features_R)
+    data_S_f = get_feature_data(feature, data_S, features_S)
+    if not any(data_R_f) or not any(data_S_f):
+        return
+
+    f, ax = plt.subplots(1, 1)
+    f.set_size_inches(9, 7)
+    f.suptitle(f'Distribution density plot of feature {feature}')
+    sns.kdeplot(data_R_f, ax=ax, label='Real dataset', fill=True, common_norm=False, color='#5480d1', alpha=0.5, linewidth=0)
+    sns.kdeplot(data_S_f, ax=ax, label='Simulated dataset', fill=True, common_norm=False, color='#d65161', alpha=0.5, linewidth=0)
+    ax.legend()
+
+    f.savefig(f'./output/temp_figures/density_plot_{feature}.svg')
+    del f
+    plt.close()
+
+def export_obs_distr_densityplot(observation_index, data_R, data_S):
+    if observation_index != 'all':
+        data_R_o = get_observation_data(observation_index, data_R)
+        data_S_o = get_observation_data(observation_index, data_S)
+        if not any(data_R_o) or not any(data_S_o):
+            return
+
+    f, ax = plt.subplots(1, 1)
+    f.set_size_inches(9, 7)
+    
+    if observation_index == 'all':
+        f.suptitle(f'Distribution density plot of all observations')
+        for index in range(len(data_R)):
+            data_R_o = get_observation_data(index, data_R)
+            data_S_o = get_observation_data(index, data_S)
+            label = 'Real dataset' if index == 0 else None
+            sns.kdeplot(data_R_o, ax=ax, label=label, fill=True, common_norm=False, color='#5480d1', alpha=0.2, linewidth=0)
+            label = 'Simulated dataset' if index == 0 else None
+            sns.kdeplot(data_S_o, ax=ax, label=label, fill=True, common_norm=False, color='#d65161', alpha=0.2, linewidth=0)
+    else:
+        f.suptitle(f'Distribution density plot of observation with index {observation_index}')
+        sns.kdeplot(data_R_o, ax=ax, label='Real dataset', fill=True, common_norm=False, color='#5480d1', alpha=0.5, linewidth=0)
+        sns.kdeplot(data_S_o, ax=ax, label='Simulated dataset', fill=True, common_norm=False, color='#d65161', alpha=0.5, linewidth=0)
+
+    ax.legend()
+    f.savefig(f'./output/temp_figures/density_plot_obs_{observation_index}.svg')
+    del f
+    plt.close()
+
+def export_avg_var_scatter_plot(data_R, data_S, axis=0):
+    data_R_x = np.average(data_R, axis=axis)
+    data_R_y = np.var(data_R, axis=axis)
+    data_S_x = np.average(data_S, axis=axis)
+    data_S_y = np.var(data_S, axis=axis)
+
+    f, ax = plt.subplots(1, 1)
+    f.set_size_inches(9, 7)
+    f.suptitle('Feature average value vs variance' if axis == 0 else 'Observation average value vs variance')
+    ax.scatter(data_R_x, data_R_y, c='#5480d1', linewidths=None, alpha=0.5, label='Real')
+    ax.scatter(data_S_x, data_S_y, c='#d65161', linewidths=None, alpha=0.5, label='Simulated')
+    ax.set_xlabel('Average value')
+    ax.set_ylabel('Variance value')
+    ax.legend()
+    
+    f.savefig(f'./output/temp_figures/avg_var_{"feat" if axis == 0 else "obs"}_scatter_plot.svg')
+    del f
+    plt.close()
+
+def export_distance(feature, data_R, data_S, features_R, features_S):
+    data_R_f = get_feature_data(feature, data_R, features_R)
+    data_S_f = get_feature_data(feature, data_S, features_S)
+    if not any(data_R_f) or not any(data_S_f):
+        return
+
+    dist = np.linalg.norm(data_R_f - data_S_f)
+    print(f'[RESULT] Euclidean distance of feature {feature} : {dist}')
+
+    with open(f'./output/temp_results/distance_{feature}.txt', 'w', encoding="utf-8") as file:
+        file.write('\t\t<tr colspan="2">\n')
+        file.write(f'\t\t\t<td>Euclidean distance of feature {feature}</td>\n')
+        file.write(f'\t\t\t<td>{dist}</td>\n')
+        file.write('\t\t</tr>\n')
+
+def export_obs_distance(observation_index, data_R, data_S):
+    if observation_index == 'all':
+        print('[ERROR] Observation Euclidean distance report does not support reporting on all observations')
+        return
+    data_R_o = get_observation_data(observation_index, data_R)
+    data_S_o = get_observation_data(observation_index, data_S)
+    if not any(data_R_o) or not any(data_S_o):
+        return
+
+    dist = []
+    if data_S_o.shape[0] < data_R_o.shape[0]:
+        data_S_o_padded = np.zeros(data_R_o.shape)
+        data_S_o_padded[:data_S_o.shape[0]] = data_S_o
+        dist = np.linalg.norm(data_R_o - data_S_o_padded)
+    elif data_R_o.shape[0] < data_S_o.shape[0]:
+        data_R_o_padded = np.zeros(data_S_o.shape)
+        data_R_o_padded[:data_R_o.shape[0]] = data_R_o
+        dist = np.linalg.norm(data_S_o - data_R_o_padded)
+    else:
+        dist = np.linalg.norm(data_R_o - data_S_o)
+
+    print(f'[RESULT] Euclidean distance of observation with index {observation_index} : {dist}')
+
+    with open(f'./output/temp_results/distance_obs_{observation_index}.txt', 'w', encoding="utf-8") as file:
+        file.write('\t\t<tr colspan="2">\n')
+        file.write(f'\t\t\t<td>Euclidean distance of observation with index {observation_index}</td>\n')
+        file.write(f'\t\t\t<td>{dist}</td>\n')
+        file.write('\t\t</tr>\n')
+    
+def export_statistics(feature, data_R, data_S, features_R, features_S):
+    data_R_f = get_feature_data(feature, data_R, features_R)
+    data_S_f = get_feature_data(feature, data_S, features_S)
+    if not any(data_R_f) or not any(data_S_f):
+        return
+
+    avg = { 'real': np.average(data_R_f), 'sim': np.average(data_S_f)}
+    median = { 'real': np.median(data_R_f), 'sim': np.median(data_S_f)}
+    std = { 'real': np.std(data_R_f), 'sim': np.std(data_S_f)}
+    var = { 'real': np.var(data_R_f), 'sim': np.var(data_S_f)}
+
+    print('[RESULT] Average of feature {0:>16} : REAL = {1:>25}, SIMULATED = {2:>25}'.format(feature, avg['real'], avg['sim']))
+    print('[RESULT] Median of feature {0:>17} : REAL = {1:>25}, SIMULATED = {2:>25}'.format(feature, median['real'], median['sim']))
+    print('[RESULT] Standard deviation of feature {0:>5} : REAL = {1:>25}, SIMULATED = {2:>25}'.format(feature, std['real'], std['sim']))
+    print('[RESULT] Variance of feature {0:>15} : REAL = {1:>25}, SIMULATED = {2:>25}'.format(feature, var['real'], var['sim']))
+
+    with open(f'./output/temp_statistics/{feature}.txt', 'w', encoding="utf-8") as file:
+        file.write('\t\t<tr>\n')
+        file.write(f'\t\t\t<td>Average of feature {feature}</td>\n')
+        file.write(f'\t\t\t<td>{avg["real"]}</td>\n')
+        file.write(f'\t\t\t<td>{avg["sim"]}</td>\n')
+        file.write('\t\t</tr>\n')
+        file.write('\t\t<tr>\n')
+        file.write(f'\t\t\t<td>Median of feature {feature}</td>\n')
+        file.write(f'\t\t\t<td>{median["real"]}</td>\n')
+        file.write(f'\t\t\t<td>{median["sim"]}</td>\n')
+        file.write('\t\t</tr>\n')
+        file.write('\t\t<tr>\n')
+        file.write(f'\t\t\t<td>Standard deviation of feature {feature}</td>\n')
+        file.write(f'\t\t\t<td>{std["real"]}</td>\n')
+        file.write(f'\t\t\t<td>{std["sim"]}</td>\n')
+        file.write('\t\t</tr>\n')
+        file.write('\t\t<tr>\n')
+        file.write(f'\t\t\t<td>Variance of feature {feature}</td>\n')
+        file.write(f'\t\t\t<td>{var["real"]}</td>\n')
+        file.write(f'\t\t\t<td>{var["sim"]}</td>\n')
+        file.write('\t\t</tr>\n')
+
+def export_obs_statistics(observation_index, data_R, data_S):
+    if observation_index == 'all':
+        print('[ERROR] Observation statistics report does not support reporting on all observations')
+        return
+    data_R_o = get_observation_data(observation_index, data_R)
+    data_S_o = get_observation_data(observation_index, data_S)
+    if not any(data_R_o) or not any(data_S_o):
+        return
+
+    avg = { 'real': np.average(data_R_o), 'sim': np.average(data_S_o)}
+    median = { 'real': np.median(data_R_o), 'sim': np.median(data_S_o)}
+    std = { 'real': np.std(data_R_o), 'sim': np.std(data_S_o)}
+    var = { 'real': np.var(data_R_o), 'sim': np.var(data_S_o)}
+
+    print('[RESULT] Average of observation with index {0:>16} : REAL = {1:>25}, SIMULATED = {2:>25}'.format(observation_index, avg['real'], avg['sim']))
+    print('[RESULT] Median of observation with index {0:>17} : REAL = {1:>25}, SIMULATED = {2:>25}'.format(observation_index, median['real'], median['sim']))
+    print('[RESULT] Standard deviation of observation with index {0:>5} : REAL = {1:>25}, SIMULATED = {2:>25}'.format(observation_index, std['real'], std['sim']))
+    print('[RESULT] Variance of observation with index {0:>15} : REAL = {1:>25}, SIMULATED = {2:>25}'.format(observation_index, var['real'], var['sim']))
+
+    with open(f'./output/temp_statistics/obs_{observation_index}.txt', 'w', encoding="utf-8") as file:
+        file.write('\t\t<tr>\n')
+        file.write(f'\t\t\t<td>Average of observation with index {observation_index}</td>\n')
+        file.write(f'\t\t\t<td>{avg["real"]}</td>\n')
+        file.write(f'\t\t\t<td>{avg["sim"]}</td>\n')
+        file.write('\t\t</tr>\n')
+        file.write('\t\t<tr>\n')
+        file.write(f'\t\t\t<td>Median of observation with index {observation_index}</td>\n')
+        file.write(f'\t\t\t<td>{median["real"]}</td>\n')
+        file.write(f'\t\t\t<td>{median["sim"]}</td>\n')
+        file.write('\t\t</tr>\n')
+        file.write('\t\t<tr>\n')
+        file.write(f'\t\t\t<td>Standard deviation of observation with index {observation_index}</td>\n')
+        file.write(f'\t\t\t<td>{std["real"]}</td>\n')
+        file.write(f'\t\t\t<td>{std["sim"]}</td>\n')
+        file.write('\t\t</tr>\n')
+        file.write('\t\t<tr>\n')
+        file.write(f'\t\t\t<td>Variance of observation with index {observation_index}</td>\n')
+        file.write(f'\t\t\t<td>{var["real"]}</td>\n')
+        file.write(f'\t\t\t<td>{var["sim"]}</td>\n')
+        file.write('\t\t</tr>\n')
```

### Comparing `evalAIRR-0.0.8/evalAIRR.egg-info/PKG-INFO` & `evalAIRR-0.0.9/evalAIRR.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,177 +1,181 @@
-Metadata-Version: 2.1
-Name: evalAIRR
-Version: 0.0.8
-Summary: Comparison of real and simulated AIRR datasets
-Author: Lukas Sparnauskas
-Author-email: <lukas.11sp@gmail.com>
-License: MIT
-Keywords: python,airr,simulated data,ml,machine learning
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Environment :: Console
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-
-
-# evalAIRR
-
-A tool that allows comparison of real and simulated datasets by providing different statistical indicators and dataset visualizations in one report.
-
-## Installation
-
-It is recommended to use a virtual python environment to run evalAIRR if another python environment is used. Here is a quick guide on how you can set up a virtual environment:
-
-`https://docs.python.org/3/tutorial/venv.html#creating-virtual-environments`
-
-### Install using pip
-
-Run this command to install the evalAIRR package:
-
-`pip install evalairr`
-
-## Quickstart
-
-evalAIRR uses a YAML file for configuration. If you are unfamiliar with how YAML files are structured, read this guide to the syntax:
-
-`https://docs.fileformat.com/programming/yaml/#syntax`
-
-This is the stucture of a sample report configuration file you can use to start off with (it is included in the repository location ./yaml_files/quickstart.yaml):
-
-```
-datasets:
-  real:
-    path: ./data/encoded_real_1000_200.csv
-  sim:
-    path: ./data/encoded_sim_1000_200.csv
-reports:
-  feature_based:
-    report1:
-      features:
-        - TGT
-        - ANV
-      report_types:
-        - ks
-        - distr_densityplot
-output:
-  path: './output/report.html'
-
-```
-
-This report will process the two provided datasets (real and simulated), and create an HTML report with feature-based report types - Kolmogorov–Smirnov test (indicated by `ks`) and a feature distribution density plot (indicated by `distr_densityplot`) for the features `TGT` and `ANV`. It will then export the report to the path `./output/report.html`. More details on what reports can be created can be found in the *YAML Configuration Guidelines* secion.
-
-You can run the program by running this command within the installation directory:
-
-`evalairr -i ./yaml_files/quickstart.yaml`
-
-The report will be generated in the specified output path in the configuration file or, if a specific path is not provided, in `<CURRENT_DIRECTORY>/output/report.html`. The report is exported in the HTML format.
-
-## YAML Configuration Guidelines
-
-The configuration YAML file consists of 3 main sections: `datasets`, `reports` and `output`.
-
-### Datasets
-
-In the `datasets` section, you have to provide paths to a real and a simulated datasets that you are comparing. This can be done by specifying the file path of each file in the `path` variable under the sections `real` and `sim` respectively. Here is an example of how a configured `datasets` section looks like:
-
-```
-datasets:
-  real:
-    path: ./data/encoded_real_1000_200.csv
-  sim:
-    path: ./data/encoded_sim_1000_200.csv
-```
-
-### Reports
-
-In the `reports` section, you can provide the list of report types you want to create and their parameters. There are three types of report groups depending on the different parameters: `feature_based`, `observation_based` and `generic`. Here is the list of reports you can create that compare the features of the real dataset with the simulated dataset:
-
-#### Feature-based reports
-- `ks` - Kolmogorov–Smirnov statistic. Parameters: list of features you are creating the report for.
-- `distr_histogram` - feature distribution histogram. Parameters: list of features you are creating the report for.
-- `distr_boxplot` - feature distribution boxplot. Parameters: list of features you are creating the report for.
-- `distr_violinplot` - feature distribution violin plot. Parameters: list of features you are creating the report for.
-- `distr_densityplot` - feature distribution density plot. Parameters: list of features you are creating the report for.
-- `distance` - Euclidean distance between the real and simulated feature. Parameters: list of features you are creating the report for.
-- `statistics` - statistical indicators (average, median, standard deviation and variance) of a feature in both real and simulated datasets. Parameters: list of features you are creating the report for.
-
-#### Observation-based reports
-- `observation_distr_histogram` - observation distribution histogram. Parameters: list of observations you are creating the report for.
-- `observation_distr_boxplot` - observation distribution boxplot. Parameters: list of observations you are creating the report for.
-- `observation_distr_violinplot` - observation distribution violin plot. Parameters: list of observations you are creating the report for.
-- `observation_distr_densityplot` - observation distribution density plot. Parameters: list of observations you are creating the report for. The observation index 'all' can be used to report on all observations in one plot.
-- `observation_distance` - Euclidean distance between the real and simulated observation. Parameters: list of observations you are creating the report for.
-- `observation_statistics` - statistical indicators (average, median, standard deviation and variance) of an observation in both real and simulated datasets. Parameters: list of observations you are creating the report for.
-
-#### General reports
-- `copula_2d` - a 2D scatter plot that displays two features in a Gausian Multivariate copula space. Parameters: a report section of any name, under which the compared features are specified.
-- `copula_3d` - a 3D scatter plot that displays three features in a Gausian Multivariate copula space. Parameters: a report section of any name, under which the compared features are specified.
-- `feature_average_vs_variance` - a scatter plot that displays the average value of every feature on one axis and the variance of every feature on the other axis.
-- `observation_average_vs_variance` - a scatter plot that displays the average value of every observation on one axis and the variance of every observation on the other axis.
-- `corr` - correlation matrix heatmaps of the real and simulated datasets. Parameters: `percent_features` - an optional parameter for dimensionality reduction using PCA. A float value corresponding with the ratio of feature reduction (e.g. `percent_features` equal to 0.5 would reduce the feature count by half). 
-- `pca_2d` - two scatter plots with both datasets reduced to two dimensions using PCA.
-
-Here is a sample `reports` section of a configuration file containing all of the reports:
-
-```
-reports:
-  feature_based:
-    report1:
-      features:
-        - TGT
-        - ANV
-      report_types:
-        - ks
-        - distr_histogram
-        - distr_boxplot
-        - distr_violinplot
-        - distr_densityplot
-        - distance
-        - statistics
-  observation_based:
-    report1:
-      observations:
-        - 0
-      report_types:
-        - observation_distr_histogram
-        - observation_distr_boxplot
-        - observation_distr_violinplot
-        - observation_distr_densityplot
-        - observation_distance
-        - observation_statistics
-    report2:
-      observations:
-        - all
-      report_types:
-        - observation_distr_densityplot
-  general:
-    copula_2d:
-      report1:
-        - TGT
-        - ANV
-    copula_3d:
-      report1:
-        - TGT
-        - ANV
-        - CAS
-    feature_average_vs_variance:
-    observation_average_vs_variance:
-    corr:
-      percent_features: 0.6
-    pca_2d:
-```
-
-### Output
-
-An optional section where you can specify the file path of the generated report. The default path of the generated report is `<INSTALL_DIRECTORY>/output/report.html`. The report is exported in the HTML format.
-
-An example output section:
-
-```
-output:
-  path: './output/report.html'
-```
+Metadata-Version: 2.1
+Name: evalAIRR
+Version: 0.0.9
+Summary: Comparison of real and simulated AIRR datasets
+Home-page: UNKNOWN
+Author: Lukas Sparnauskas
+Author-email: <lukas.11sp@gmail.com>
+License: MIT
+Keywords: python,airr,simulated data,ml,machine learning
+Platform: UNKNOWN
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Environment :: Console
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+
+
+# evalAIRR
+
+A tool that allows comparison of real and simulated datasets by providing different statistical indicators and dataset visualizations in one report.
+
+## Installation
+
+It is recommended to use a virtual python environment to run evalAIRR if another python environment is used. Here is a quick guide on how you can set up a virtual environment:
+
+`https://docs.python.org/3/tutorial/venv.html#creating-virtual-environments`
+
+### Install using pip
+
+Run this command to install the evalAIRR package:
+
+`pip install evalairr`
+
+## Quickstart
+
+evalAIRR uses a YAML file for configuration. If you are unfamiliar with how YAML files are structured, read this guide to the syntax:
+
+`https://docs.fileformat.com/programming/yaml/#syntax`
+
+This is the stucture of a sample report configuration file you can use to start off with (it is included in the repository location ./yaml_files/quickstart.yaml):
+
+```
+datasets:
+  real:
+    path: ./data/encoded_real_1000_200.csv
+  sim:
+    path: ./data/encoded_sim_1000_200.csv
+reports:
+  feature_based:
+    report1:
+      features:
+        - TGT
+        - ANV
+      report_types:
+        - ks
+        - distr_densityplot
+output:
+  path: './output/report.html'
+
+```
+
+This report will process the two provided datasets (real and simulated), and create an HTML report with feature-based report types - Kolmogorov–Smirnov test (indicated by `ks`) and a feature distribution density plot (indicated by `distr_densityplot`) for the features `TGT` and `ANV`. It will then export the report to the path `./output/report.html`. More details on what reports can be created can be found in the *YAML Configuration Guidelines* secion.
+
+You can run the program by running this command within the installation directory:
+
+`evalairr -i ./yaml_files/quickstart.yaml`
+
+The report will be generated in the specified output path in the configuration file or, if a specific path is not provided, in `<CURRENT_DIRECTORY>/output/report.html`. The report is exported in the HTML format.
+
+## YAML Configuration Guidelines
+
+The configuration YAML file consists of 3 main sections: `datasets`, `reports` and `output`.
+
+### Datasets
+
+In the `datasets` section, you have to provide paths to a real and a simulated datasets that you are comparing. This can be done by specifying the file path of each file in the `path` variable under the sections `real` and `sim` respectively. Here is an example of how a configured `datasets` section looks like:
+
+```
+datasets:
+  real:
+    path: ./data/encoded_real_1000_200.csv
+  sim:
+    path: ./data/encoded_sim_1000_200.csv
+```
+
+### Reports
+
+In the `reports` section, you can provide the list of report types you want to create and their parameters. There are three types of report groups depending on the different parameters: `feature_based`, `observation_based` and `generic`. Here is the list of reports you can create that compare the features of the real dataset with the simulated dataset:
+
+#### Feature-based reports
+- `ks` - Kolmogorov–Smirnov statistic. Parameters: list of features you are creating the report for.
+- `distr_histogram` - feature distribution histogram. Parameters: list of features you are creating the report for.
+- `distr_boxplot` - feature distribution boxplot. Parameters: list of features you are creating the report for.
+- `distr_violinplot` - feature distribution violin plot. Parameters: list of features you are creating the report for.
+- `distr_densityplot` - feature distribution density plot. Parameters: list of features you are creating the report for.
+- `distance` - Euclidean distance between the real and simulated feature. Parameters: list of features you are creating the report for.
+- `statistics` - statistical indicators (average, median, standard deviation and variance) of a feature in both real and simulated datasets. Parameters: list of features you are creating the report for.
+
+#### Observation-based reports
+- `observation_distr_histogram` - observation distribution histogram. Parameters: list of observations you are creating the report for.
+- `observation_distr_boxplot` - observation distribution boxplot. Parameters: list of observations you are creating the report for.
+- `observation_distr_violinplot` - observation distribution violin plot. Parameters: list of observations you are creating the report for.
+- `observation_distr_densityplot` - observation distribution density plot. Parameters: list of observations you are creating the report for. The observation index 'all' can be used to report on all observations in one plot.
+- `observation_distance` - Euclidean distance between the real and simulated observation. Parameters: list of observations you are creating the report for.
+- `observation_statistics` - statistical indicators (average, median, standard deviation and variance) of an observation in both real and simulated datasets. Parameters: list of observations you are creating the report for.
+
+#### General reports
+- `copula_2d` - a 2D scatter plot that displays two features in a Gausian Multivariate copula space. Parameters: a report section of any name, under which the compared features are specified.
+- `copula_3d` - a 3D scatter plot that displays three features in a Gausian Multivariate copula space. Parameters: a report section of any name, under which the compared features are specified.
+- `feature_average_vs_variance` - a scatter plot that displays the average value of every feature on one axis and the variance of every feature on the other axis.
+- `observation_average_vs_variance` - a scatter plot that displays the average value of every observation on one axis and the variance of every observation on the other axis.
+- `corr` - correlation matrix heatmaps of the real and simulated datasets. Parameters: `percent_features` - an optional parameter for dimensionality reduction using PCA. A float value corresponding with the ratio of feature reduction (e.g. `percent_features` equal to 0.5 would reduce the feature count by half). 
+- `pca_2d` - two scatter plots with both datasets reduced to two dimensions using PCA.
+
+Here is a sample `reports` section of a configuration file containing all of the reports:
+
+```
+reports:
+  feature_based:
+    report1:
+      features:
+        - TGT
+        - ANV
+      report_types:
+        - ks
+        - distr_histogram
+        - distr_boxplot
+        - distr_violinplot
+        - distr_densityplot
+        - distance
+        - statistics
+  observation_based:
+    report1:
+      observations:
+        - 0
+      report_types:
+        - observation_distr_histogram
+        - observation_distr_boxplot
+        - observation_distr_violinplot
+        - observation_distr_densityplot
+        - observation_distance
+        - observation_statistics
+    report2:
+      observations:
+        - all
+      report_types:
+        - observation_distr_densityplot
+  general:
+    copula_2d:
+      report1:
+        - TGT
+        - ANV
+    copula_3d:
+      report1:
+        - TGT
+        - ANV
+        - CAS
+    feature_average_vs_variance:
+    observation_average_vs_variance:
+    corr:
+      percent_features: 0.6
+    pca_2d:
+```
+
+### Output
+
+An optional section where you can specify the file path of the generated report. The default path of the generated report is `<INSTALL_DIRECTORY>/output/report.html`. The report is exported in the HTML format.
+
+An example output section:
+
+```
+output:
+  path: './output/report.html'
+```
+
+
```

### Comparing `evalAIRR-0.0.8/setup.py` & `evalAIRR-0.0.9/setup.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from setuptools import setup, find_packages
-from evalAIRR.version import __version__
-import codecs
-import os
-
-here = os.path.abspath(os.path.dirname(__file__))
-
-with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
-    long_description = "\n" + fh.read()
-
-DESCRIPTION = 'Comparison of real and simulated AIRR datasets'
-
-setup(
-    name="evalAIRR",
-    version=__version__,
-    author="Lukas Sparnauskas",
-    author_email="<lukas.11sp@gmail.com>",
-    description=DESCRIPTION,
-    long_description_content_type="text/markdown",
-    long_description=long_description,
-    include_package_data=True,
-    license='MIT',
-    packages=find_packages(),
-    keywords=['python', 'airr', 'simulated data', 'ml', 'machine learning'],
-    entry_points={'console_scripts': ['evalairr=evalAIRR.main:run']},
-    classifiers=[
-        "Development Status :: 2 - Pre-Alpha",
-        "Intended Audience :: Science/Research",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.10",
-        "Environment :: Console",
-        "Operating System :: Unix",
-        "Operating System :: MacOS :: MacOS X",
-        "Operating System :: Microsoft :: Windows",
-    ]
+from setuptools import setup, find_packages
+from evalAIRR.version import __version__
+import codecs
+import os
+
+here = os.path.abspath(os.path.dirname(__file__))
+
+with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
+    long_description = "\n" + fh.read()
+
+DESCRIPTION = 'Comparison of real and simulated AIRR datasets'
+
+setup(
+    name="evalAIRR",
+    version=__version__,
+    author="Lukas Sparnauskas",
+    author_email="<lukas.11sp@gmail.com>",
+    description=DESCRIPTION,
+    long_description_content_type="text/markdown",
+    long_description=long_description,
+    include_package_data=True,
+    license='MIT',
+    packages=find_packages(),
+    keywords=['python', 'airr', 'simulated data', 'ml', 'machine learning'],
+    entry_points={'console_scripts': ['evalairr=evalAIRR.main:run']},
+    classifiers=[
+        "Development Status :: 2 - Pre-Alpha",
+        "Intended Audience :: Science/Research",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.10",
+        "Environment :: Console",
+        "Operating System :: Unix",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: Microsoft :: Windows",
+    ]
 )
```

