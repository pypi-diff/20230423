# Comparing `tmp/teg_CCC-0.0.1.tar.gz` & `tmp/teg_CCC-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teg_CCC-0.0.1.tar", last modified: Sun Apr 23 16:09:14 2023, max compression
+gzip compressed data, was "teg_CCC-0.0.2.tar", last modified: Sun Apr 23 16:17:12 2023, max compression
```

## Comparing `teg_CCC-0.0.1.tar` & `teg_CCC-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 16:09:14.084492 teg_CCC-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-03-26 19:15:12.000000 teg_CCC-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1957 2023-04-23 16:09:14.083496 teg_CCC-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1370 2023-04-23 16:06:34.000000 teg_CCC-0.0.1/README.md
--rw-rw-rw-   0        0        0      719 2023-04-23 16:08:10.000000 teg_CCC-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-23 16:09:14.084492 teg_CCC-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-23 16:09:14.083496 teg_CCC-0.0.1/teg_CCC.egg-info/
--rw-rw-rw-   0        0        0     1957 2023-04-23 16:09:13.000000 teg_CCC-0.0.1/teg_CCC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-04-23 16:09:14.000000 teg_CCC-0.0.1/teg_CCC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 16:09:13.000000 teg_CCC-0.0.1/teg_CCC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-04-23 16:09:13.000000 teg_CCC-0.0.1/teg_CCC.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-23 16:09:13.000000 teg_CCC-0.0.1/teg_CCC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2340 2023-04-23 15:43:02.000000 teg_CCC-0.0.1/teg_CCC.py
+drwxrwxrwx   0        0        0        0 2023-04-23 16:17:12.068331 teg_CCC-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-03-26 19:15:12.000000 teg_CCC-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1972 2023-04-23 16:17:12.068331 teg_CCC-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1385 2023-04-23 16:15:44.000000 teg_CCC-0.0.2/README.md
+-rw-rw-rw-   0        0        0      719 2023-04-23 16:16:02.000000 teg_CCC-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-23 16:17:12.068331 teg_CCC-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-23 16:17:12.067172 teg_CCC-0.0.2/teg_CCC.egg-info/
+-rw-rw-rw-   0        0        0     1972 2023-04-23 16:17:12.000000 teg_CCC-0.0.2/teg_CCC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-04-23 16:17:12.000000 teg_CCC-0.0.2/teg_CCC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 16:17:12.000000 teg_CCC-0.0.2/teg_CCC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-04-23 16:17:12.000000 teg_CCC-0.0.2/teg_CCC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-23 16:17:12.000000 teg_CCC-0.0.2/teg_CCC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2340 2023-04-23 15:43:02.000000 teg_CCC-0.0.2/teg_CCC.py
```

### Comparing `teg_CCC-0.0.1/LICENSE` & `teg_CCC-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `teg_CCC-0.0.1/PKG-INFO` & `teg_CCC-0.0.2/teg_CCC.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: teg_CCC
-Version: 0.0.1
+Name: teg-CCC
+Version: 0.0.2
 Summary: Estimate the true number of clusters for k-means clustering using the Cluster Consistency Criterion (CCC).
 Author-email: "Thomas E. Gladwin" <thomasgladwin@hotmail.com>
 Project-URL: Homepage, https://tegladwin.com
 Project-URL: Bug Tracker, https://github.com/thomasgladwin/teg_CCC
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,14 +14,14 @@
 
 Estimate the true number of clusters for k-means clustering using the Cluster Consistency Criterion (CCC).
 
 This algorithm follows the rationale that true cluster centres should be similar in random split-halves of the data. If too maby clusters are specified, the cluster centres will become driven by random sampling error.
 
 The CCC implements this as follows. For each number of clusters, the data are split into random halves for a given number of splits (e.g., 20). For each sp0lit, a k-means cluster analysis is run on each half separately. The distances between most-similar cluster centres are summed. The similarity score is e^(-distance_sum). The mean similarity score over random splits is the score for the given number of clusters.
 
-The best estimate of the true number of clusters is determined by where the score drops off, which occurs when the number of clusters becomes higher than the true number of clusters.
+The best estimate of the true number of clusters is determined by where the improvement in score drops off, which occurs when the number of clusters becomes higher than the true number of clusters.
 
 The file test.py gives an example and simulation script. Usage is:
 
 O = teg_CCC.get_best_k_CCC(X)
 
 where X is a 2D array of shape N_Observations x N_Variables. There is an optional argument for max_n_clusters, set to 10 by default. The output is a dictionary with the estimate of true cluster centres (best_n) as well as the similarity score per number of clusters (scores_per_n) and the associated number of clusters (n_vec).
```

### Comparing `teg_CCC-0.0.1/README.md` & `teg_CCC-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Estimate the true number of clusters for k-means clustering using the Cluster Consistency Criterion (CCC).
 
 This algorithm follows the rationale that true cluster centres should be similar in random split-halves of the data. If too maby clusters are specified, the cluster centres will become driven by random sampling error.
 
 The CCC implements this as follows. For each number of clusters, the data are split into random halves for a given number of splits (e.g., 20). For each sp0lit, a k-means cluster analysis is run on each half separately. The distances between most-similar cluster centres are summed. The similarity score is e^(-distance_sum). The mean similarity score over random splits is the score for the given number of clusters.
 
-The best estimate of the true number of clusters is determined by where the score drops off, which occurs when the number of clusters becomes higher than the true number of clusters.
+The best estimate of the true number of clusters is determined by where the improvement in score drops off, which occurs when the number of clusters becomes higher than the true number of clusters.
 
 The file test.py gives an example and simulation script. Usage is:
 
 O = teg_CCC.get_best_k_CCC(X)
 
 where X is a 2D array of shape N_Observations x N_Variables. There is an optional argument for max_n_clusters, set to 10 by default. The output is a dictionary with the estimate of true cluster centres (best_n) as well as the similarity score per number of clusters (scores_per_n) and the associated number of clusters (n_vec).
```

### Comparing `teg_CCC-0.0.1/pyproject.toml` & `teg_CCC-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "teg_CCC"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Thomas E. Gladwin", email="thomasgladwin@hotmail.com" },
 ]
 description = "Estimate the true number of clusters for k-means clustering using the Cluster Consistency Criterion (CCC)."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `teg_CCC-0.0.1/teg_CCC.egg-info/PKG-INFO` & `teg_CCC-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: teg-CCC
-Version: 0.0.1
+Name: teg_CCC
+Version: 0.0.2
 Summary: Estimate the true number of clusters for k-means clustering using the Cluster Consistency Criterion (CCC).
 Author-email: "Thomas E. Gladwin" <thomasgladwin@hotmail.com>
 Project-URL: Homepage, https://tegladwin.com
 Project-URL: Bug Tracker, https://github.com/thomasgladwin/teg_CCC
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,14 +14,14 @@
 
 Estimate the true number of clusters for k-means clustering using the Cluster Consistency Criterion (CCC).
 
 This algorithm follows the rationale that true cluster centres should be similar in random split-halves of the data. If too maby clusters are specified, the cluster centres will become driven by random sampling error.
 
 The CCC implements this as follows. For each number of clusters, the data are split into random halves for a given number of splits (e.g., 20). For each sp0lit, a k-means cluster analysis is run on each half separately. The distances between most-similar cluster centres are summed. The similarity score is e^(-distance_sum). The mean similarity score over random splits is the score for the given number of clusters.
 
-The best estimate of the true number of clusters is determined by where the score drops off, which occurs when the number of clusters becomes higher than the true number of clusters.
+The best estimate of the true number of clusters is determined by where the improvement in score drops off, which occurs when the number of clusters becomes higher than the true number of clusters.
 
 The file test.py gives an example and simulation script. Usage is:
 
 O = teg_CCC.get_best_k_CCC(X)
 
 where X is a 2D array of shape N_Observations x N_Variables. There is an optional argument for max_n_clusters, set to 10 by default. The output is a dictionary with the estimate of true cluster centres (best_n) as well as the similarity score per number of clusters (scores_per_n) and the associated number of clusters (n_vec).
```

### Comparing `teg_CCC-0.0.1/teg_CCC.py` & `teg_CCC-0.0.2/teg_CCC.py`

 * *Files identical despite different names*

