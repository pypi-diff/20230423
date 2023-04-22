# Comparing `tmp/networkx_robustness-0.0.4.tar.gz` & `tmp/networkx_robustness-0.0.5.tar.gz`

## Comparing `networkx_robustness-0.0.4.tar` & `networkx_robustness-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 networkx_robustness-0.0.4/src/networkx_robustness/__init__.py
--rw-r--r--   0        0        0    11392 2020-02-02 00:00:00.000000 networkx_robustness-0.0.4/src/networkx_robustness/networkx_robustness.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 networkx_robustness-0.0.4/LICENSE
--rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 networkx_robustness-0.0.4/README.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 networkx_robustness-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 networkx_robustness-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 networkx_robustness-0.0.5/src/networkx_robustness/__init__.py
+-rw-r--r--   0        0        0    11392 2020-02-02 00:00:00.000000 networkx_robustness-0.0.5/src/networkx_robustness/networkx_robustness.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 networkx_robustness-0.0.5/LICENSE
+-rw-r--r--   0        0        0     4264 2020-02-02 00:00:00.000000 networkx_robustness-0.0.5/README.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 networkx_robustness-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4838 2020-02-02 00:00:00.000000 networkx_robustness-0.0.5/PKG-INFO
```

### Comparing `networkx_robustness-0.0.4/src/networkx_robustness/networkx_robustness.py` & `networkx_robustness-0.0.5/src/networkx_robustness/networkx_robustness.py`

 * *Files identical despite different names*

### Comparing `networkx_robustness-0.0.4/LICENSE` & `networkx_robustness-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `networkx_robustness-0.0.4/README.md` & `networkx_robustness-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # networkx-robustness
 
 A package for simulating network attacks on NetworkX graphs. The current supported attacks include random attacks and targeted attacks on nodes with the highest degree centrality, betweenness centrality, closeness centrality, and eigenvector centrality. Attack functions return the initial fraction of nodes in the giant component, a list of the fraction of nodes in the giant component after each node removal, and a list of the average path length in the giant component after each node removal.
 
+## Citation
+
+If you use this package, please cite the package as:
+
+Tejas Santanam. (2023). tsantanam/networkx-robustness: v0.0.5 (v0.0.5). Zenodo.
+
 ## Installation
 
 The package can be installed using the pip package manager and requires Python 3.7 or greater.
 
 ```bash
 pip install networkx-robustness
 ```
```

### Comparing `networkx_robustness-0.0.4/pyproject.toml` & `networkx_robustness-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "networkx_robustness"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Tejas Santanam", email="santanam.tejas@gmail.com" },
 ]
 description = "A package for simulating network attacks on NetworkX graphs"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `networkx_robustness-0.0.4/PKG-INFO` & `networkx_robustness-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: networkx_robustness
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package for simulating network attacks on NetworkX graphs
 Project-URL: Homepage, https://github.com/tsantanam/networkx-robustness
 Project-URL: Bug Tracker, https://github.com/tsantanam/networkx-robustness/issues
 Author-email: Tejas Santanam <santanam.tejas@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,20 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # networkx-robustness
 
 A package for simulating network attacks on NetworkX graphs. The current supported attacks include random attacks and targeted attacks on nodes with the highest degree centrality, betweenness centrality, closeness centrality, and eigenvector centrality. Attack functions return the initial fraction of nodes in the giant component, a list of the fraction of nodes in the giant component after each node removal, and a list of the average path length in the giant component after each node removal.
 
+## Citation
+
+If you use this package, please cite the package as:
+
+Tejas Santanam. (2023). tsantanam/networkx-robustness: v0.0.5 (v0.0.5). Zenodo.
+
 ## Installation
 
 The package can be installed using the pip package manager and requires Python 3.7 or greater.
 
 ```bash
 pip install networkx-robustness
 ```
```

