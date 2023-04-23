# Comparing `tmp/networkx_robustness-0.0.6.tar.gz` & `tmp/networkx_robustness-0.0.7.tar.gz`

## Comparing `networkx_robustness-0.0.6.tar` & `networkx_robustness-0.0.7.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 networkx_robustness-0.0.6/src/networkx_robustness/__init__.py
--rw-r--r--   0        0        0    11392 2020-02-02 00:00:00.000000 networkx_robustness-0.0.6/src/networkx_robustness/networkx_robustness.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 networkx_robustness-0.0.6/LICENSE
--rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 networkx_robustness-0.0.6/README.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 networkx_robustness-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     4877 2020-02-02 00:00:00.000000 networkx_robustness-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 networkx_robustness-0.0.7/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 networkx_robustness-0.0.7/src/networkx_robustness/__init__.py
+-rw-r--r--   0        0        0    12417 2020-02-02 00:00:00.000000 networkx_robustness-0.0.7/src/networkx_robustness/networkx_robustness.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 networkx_robustness-0.0.7/LICENSE
+-rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 networkx_robustness-0.0.7/README.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 networkx_robustness-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 networkx_robustness-0.0.7/PKG-INFO
```

### Comparing `networkx_robustness-0.0.6/src/networkx_robustness/networkx_robustness.py` & `networkx_robustness-0.0.7/src/networkx_robustness/networkx_robustness.py`

 * *Files 5% similar despite different names*

```diff
@@ -230,7 +230,37 @@
         Gc_nodes = Gc.number_of_nodes()
         # get the fraction of nodes in the largest connected component
         frac.append(Gc_nodes / G_nodes)
         # get the average path length of the largest connected component
         apl.append(nx.average_shortest_path_length(Gc, weight=weight))
 
     return initial, frac, apl
+
+def molloy_reed(G=None):
+    """
+    Compute the Molloy-Reed criterion for a network
+    :param G: networkx graph
+    :return: Molloy-Reed criterion
+    """
+    # get the average squared degree
+    avg_sq_degree = sum([d ** 2 for n, d in G.degree()]) / G.number_of_nodes()
+    # get the average degree
+    avg_degree = sum([d for n, d in G.degree()]) / G.number_of_nodes()
+    # compute the Molloy-Reed criterion
+    molloy_reed = avg_sq_degree/avg_degree
+
+    return molloy_reed
+
+def critical_threshold(G=None):
+    """
+    Compute the critical threshold for a network
+    :param G: networkx graph
+    :return: critical threshold
+    """
+    # get the average squared degree
+    avg_sq_degree = sum([d ** 2 for n, d in G.degree()]) / G.number_of_nodes()
+    # get the average degree
+    avg_degree = sum([d for n, d in G.degree()]) / G.number_of_nodes()
+    # compute the Molloy-Reed criterion
+    molloy_reed = avg_sq_degree/avg_degree
+    # compute the critical threshold
+    critical_threshold = 1 - (1/(molloy_reed-1))
```

### Comparing `networkx_robustness-0.0.6/LICENSE` & `networkx_robustness-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `networkx_robustness-0.0.6/README.md` & `networkx_robustness-0.0.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,38 @@
+Metadata-Version: 2.1
+Name: networkx_robustness
+Version: 0.0.7
+Summary: A package for simulating network attacks on NetworkX graphs
+Project-URL: Homepage, https://github.com/tsantanam/networkx-robustness
+Project-URL: Bug Tracker, https://github.com/tsantanam/networkx-robustness/issues
+Author-email: Tejas Santanam <santanam.tejas@gmail.com>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 # networkx-robustness
 
+[![DOI](https://zenodo.org/badge/631239682.svg)](https://zenodo.org/badge/latestdoi/631239682) [![PyPI Version](https://img.shields.io/pypi/v/networkx-robustness.svg)](https://pypi.python.org/pypi/networkx-robustness)
+
 A package for simulating network attacks on NetworkX graphs. The current supported attacks include random attacks and targeted attacks on nodes with the highest degree centrality, betweenness centrality, closeness centrality, and eigenvector centrality. Attack functions return the initial fraction of nodes in the giant component, a list of the fraction of nodes in the giant component after each node removal, and a list of the average path length in the giant component after each node removal.
 
+The package also contains functions for calculating the Molloy-Reed criterion and the critical threshold for a network.
+
 ## Citation
 
 If you use this package, please cite the package as:
 
-Tejas Santanam. (2023). tsantanam/networkx-robustness: v0.0.6 (v0.0.6). Zenodo. https://doi.org/10.5281/zenodo.7855211
+Tejas Santanam. (2023). tsantanam/networkx-robustness: v0.0.7 (v0.0.7). Zenodo. https://doi.org/10.5281/zenodo.7855211
 
 ## Installation
 
-The package can be installed using the pip package manager and requires Python 3.7 or greater.
+The package can be installed using the pip package manager and requires Python 3.7 or greater. There is a package dependency with NetworkX.
 
 ```bash
 pip install networkx-robustness
 ```
 
 ## Example
 
@@ -27,41 +45,43 @@
 #Random NetworkX graph with 100 nodes
 G = nx.gnp_random_graph(100, 0.5)
 
 #Simulate a random attack on 20 nodes
 initial, frac, apl = networkx_robustness.simulate_random_attack(G, attack_fraction=0.2)
 ```
 
-## Simulating random attacks
+## Documentation
+
+### Simulating random attacks
 
 ```python
 initial, frac, apl = simulate_random_attack(G=None, attack_fraction=0.1, weight=None)
     """
     Simulate random attack on a network
     :param G: networkx graph
     :param attack_fraction: fraction of nodes to be attacked (default: 0.1)
     :param weight: weight of edges (default: None)
     :return: initial (float), frac (list), apl (list)
     """
 ```
 
-## Simulating degree centrality targeted attacks
+### Simulating degree centrality targeted attacks
 
 ```python
 initial, frac, apl = simulate_degree_attack(G=None, attack_fraction=0.1, weight=None)
     """
     Simulate degree attack on a network
     :param G: networkx graph
     :param attack_fraction: fraction of nodes to be attacked (default: 0.1)
     :param weight: weight of edges (default: None)
     :return: initial (float), frac (list), apl (list)
     """
 ```
 
-## Simulating betweenness centrality targeted attacks
+### Simulating betweenness centrality targeted attacks
 
 ```python
 initial, frac, apl = simulate_betweenness_attack(G=None, attack_fraction=0.1, weight=None, normalized=True, k=None, seed=None, endpoints=False)
     """
     Simulate betweenness attack on a network
     :param G: networkx graph
     :param attack_fraction: fraction of nodes to be attacked (default: 0.1)
@@ -70,37 +90,59 @@
     :param k: use k node samples to estimate betweenness (default: None)
     :param seed: seed for random number generator (default: None)
     :param endpoints: If True include the endpoints in the shortest path counts (default: False)
     :return: initial (float), frac (list), apl (list)
     """
 ```
 
-## Simulating closeness centrality targeted attacks
+### Simulating closeness centrality targeted attacks
 
 ```python
 initial, frac, apl = simulate_closeness_attack(G=None, attack_fraction=0.1, weight=None, u=None, wf_improved=True)
     """
     Simulate closeness attack on a network
     :param G: networkx graph
     :param attack_fraction: fraction of nodes to be attacked (default: 0.1)
     :param weight: weight of edges (default: None)
     :param u: node for which closeness is to be computed (default: None)
     :param wf_improved: use of the improved algorithm to scale by the fraction of nodes reachable (default: True)
     :return: initial (float), frac (list), apl (list)
     """
 ```
 
-## Simulating eigenvector centrality targeted attacks
+### Simulating eigenvector centrality targeted attacks
 
 ```python
 initial, frac, apl = simulate_eigenvector_attack(G=None, attack_fraction=0.1, weight=None, tol=1e-06, max_iter=100, nstart=None)
     """
     Simulate eigenvector attack on a network
     :param G: networkx graph
     :param attack_fraction: fraction of nodes to be attacked (default: 0.1)
     :param weight: weight of edges (default: None)
     :param tol: tolerance for the power iteration method (default: 1e-06)
     :param max_iter: maximum number of iterations for the power iteration method (default: 100)
     :param nstart: initial vector for the power iteration method (default: None)
     :return: initial (float), frac (list), apl (list)
     """
 ```
+
+### Calculating the Molloy-Reed Criterion
+
+```python
+molloy_reed = molloy_reed(G=None)
+    """
+    Compute the Molloy-Reed criterion for a network
+    :param G: networkx graph
+    :return: Molloy-Reed criterion
+    """
+```
+
+### Calculating the critical threshold
+
+```python
+critical_threshold = critical_threshold(G=None)
+    """
+    Compute the critical threshold for a network
+    :param G: networkx graph
+    :return: critical threshold
+    """
+```
```

### Comparing `networkx_robustness-0.0.6/pyproject.toml` & `networkx_robustness-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "networkx_robustness"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Tejas Santanam", email="santanam.tejas@gmail.com" },
 ]
 description = "A package for simulating network attacks on NetworkX graphs"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `networkx_robustness-0.0.6/PKG-INFO` & `networkx_robustness-0.0.7/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,24 @@
-Metadata-Version: 2.1
-Name: networkx_robustness
-Version: 0.0.6
-Summary: A package for simulating network attacks on NetworkX graphs
-Project-URL: Homepage, https://github.com/tsantanam/networkx-robustness
-Project-URL: Bug Tracker, https://github.com/tsantanam/networkx-robustness/issues
-Author-email: Tejas Santanam <santanam.tejas@gmail.com>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 # networkx-robustness
 
+[![DOI](https://zenodo.org/badge/631239682.svg)](https://zenodo.org/badge/latestdoi/631239682) [![PyPI Version](https://img.shields.io/pypi/v/networkx-robustness.svg)](https://pypi.python.org/pypi/networkx-robustness)
+
 A package for simulating network attacks on NetworkX graphs. The current supported attacks include random attacks and targeted attacks on nodes with the highest degree centrality, betweenness centrality, closeness centrality, and eigenvector centrality. Attack functions return the initial fraction of nodes in the giant component, a list of the fraction of nodes in the giant component after each node removal, and a list of the average path length in the giant component after each node removal.
 
+The package also contains functions for calculating the Molloy-Reed criterion and the critical threshold for a network.
+
 ## Citation
 
 If you use this package, please cite the package as:
 
-Tejas Santanam. (2023). tsantanam/networkx-robustness: v0.0.6 (v0.0.6). Zenodo. https://doi.org/10.5281/zenodo.7855211
+Tejas Santanam. (2023). tsantanam/networkx-robustness: v0.0.7 (v0.0.7). Zenodo. https://doi.org/10.5281/zenodo.7855211
 
 ## Installation
 
-The package can be installed using the pip package manager and requires Python 3.7 or greater.
+The package can be installed using the pip package manager and requires Python 3.7 or greater. There is a package dependency with NetworkX.
 
 ```bash
 pip install networkx-robustness
 ```
 
 ## Example
 
@@ -41,41 +31,43 @@
 #Random NetworkX graph with 100 nodes
 G = nx.gnp_random_graph(100, 0.5)
 
 #Simulate a random attack on 20 nodes
 initial, frac, apl = networkx_robustness.simulate_random_attack(G, attack_fraction=0.2)
 ```
 
-## Simulating random attacks
+## Documentation
+
+### Simulating random attacks
 
 ```python
 initial, frac, apl = simulate_random_attack(G=None, attack_fraction=0.1, weight=None)
     """
     Simulate random attack on a network
     :param G: networkx graph
     :param attack_fraction: fraction of nodes to be attacked (default: 0.1)
     :param weight: weight of edges (default: None)
     :return: initial (float), frac (list), apl (list)
     """
 ```
 
-## Simulating degree centrality targeted attacks
+### Simulating degree centrality targeted attacks
 
 ```python
 initial, frac, apl = simulate_degree_attack(G=None, attack_fraction=0.1, weight=None)
     """
     Simulate degree attack on a network
     :param G: networkx graph
     :param attack_fraction: fraction of nodes to be attacked (default: 0.1)
     :param weight: weight of edges (default: None)
     :return: initial (float), frac (list), apl (list)
     """
 ```
 
-## Simulating betweenness centrality targeted attacks
+### Simulating betweenness centrality targeted attacks
 
 ```python
 initial, frac, apl = simulate_betweenness_attack(G=None, attack_fraction=0.1, weight=None, normalized=True, k=None, seed=None, endpoints=False)
     """
     Simulate betweenness attack on a network
     :param G: networkx graph
     :param attack_fraction: fraction of nodes to be attacked (default: 0.1)
@@ -84,37 +76,59 @@
     :param k: use k node samples to estimate betweenness (default: None)
     :param seed: seed for random number generator (default: None)
     :param endpoints: If True include the endpoints in the shortest path counts (default: False)
     :return: initial (float), frac (list), apl (list)
     """
 ```
 
-## Simulating closeness centrality targeted attacks
+### Simulating closeness centrality targeted attacks
 
 ```python
 initial, frac, apl = simulate_closeness_attack(G=None, attack_fraction=0.1, weight=None, u=None, wf_improved=True)
     """
     Simulate closeness attack on a network
     :param G: networkx graph
     :param attack_fraction: fraction of nodes to be attacked (default: 0.1)
     :param weight: weight of edges (default: None)
     :param u: node for which closeness is to be computed (default: None)
     :param wf_improved: use of the improved algorithm to scale by the fraction of nodes reachable (default: True)
     :return: initial (float), frac (list), apl (list)
     """
 ```
 
-## Simulating eigenvector centrality targeted attacks
+### Simulating eigenvector centrality targeted attacks
 
 ```python
 initial, frac, apl = simulate_eigenvector_attack(G=None, attack_fraction=0.1, weight=None, tol=1e-06, max_iter=100, nstart=None)
     """
     Simulate eigenvector attack on a network
     :param G: networkx graph
     :param attack_fraction: fraction of nodes to be attacked (default: 0.1)
     :param weight: weight of edges (default: None)
     :param tol: tolerance for the power iteration method (default: 1e-06)
     :param max_iter: maximum number of iterations for the power iteration method (default: 100)
     :param nstart: initial vector for the power iteration method (default: None)
     :return: initial (float), frac (list), apl (list)
     """
 ```
+
+### Calculating the Molloy-Reed Criterion
+
+```python
+molloy_reed = molloy_reed(G=None)
+    """
+    Compute the Molloy-Reed criterion for a network
+    :param G: networkx graph
+    :return: Molloy-Reed criterion
+    """
+```
+
+### Calculating the critical threshold
+
+```python
+critical_threshold = critical_threshold(G=None)
+    """
+    Compute the critical threshold for a network
+    :param G: networkx graph
+    :return: critical threshold
+    """
+```
```

