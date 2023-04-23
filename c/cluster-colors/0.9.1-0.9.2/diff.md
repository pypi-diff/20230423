# Comparing `tmp/cluster_colors-0.9.1.tar.gz` & `tmp/cluster_colors-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cluster_colors-0.9.1.tar", max compression
+gzip compressed data, was "cluster_colors-0.9.2.tar", max compression
```

## Comparing `cluster_colors-0.9.1.tar` & `cluster_colors-0.9.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1457 2023-04-12 19:39:24.312366 cluster_colors-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     3533 2023-04-10 15:14:34.401917 cluster_colors-0.9.1/README.md
--rw-r--r--   0        0        0      383 2023-03-14 23:49:36.976311 cluster_colors-0.9.1/src/cluster_colors/__init__.py
--rw-r--r--   0        0        0    29220 2023-04-12 19:31:39.512110 cluster_colors-0.9.1/src/cluster_colors/clusters.py
--rw-r--r--   0        0        0      290 2023-03-14 18:50:46.788014 cluster_colors-0.9.1/src/cluster_colors/config.py
--rw-r--r--   0        0        0     3009 2023-03-14 02:27:27.128539 cluster_colors-0.9.1/src/cluster_colors/cut_colors.py
--rw-r--r--   0        0        0     3004 2023-04-10 15:14:34.433735 cluster_colors-0.9.1/src/cluster_colors/distance_matrix.py
--rw-r--r--   0        0        0     5239 2023-04-10 15:14:34.433735 cluster_colors-0.9.1/src/cluster_colors/image_colors.py
--rw-r--r--   0        0        0     1290 2023-04-10 15:14:34.433735 cluster_colors-0.9.1/src/cluster_colors/kmedians.py
--rw-r--r--   0        0        0      295 2023-03-13 11:40:04.953104 cluster_colors-0.9.1/src/cluster_colors/paths.py
--rw-r--r--   0        0        0     5159 2023-03-19 19:41:53.291090 cluster_colors-0.9.1/src/cluster_colors/pool_colors.py
--rw-r--r--   0        0        0        0 2023-03-09 22:18:11.789791 cluster_colors-0.9.1/src/cluster_colors/py.typed
--rw-r--r--   0        0        0      908 2023-04-10 21:13:40.908497 cluster_colors-0.9.1/src/cluster_colors/type_hints.py
--rw-r--r--   0        0        0     3245 2023-04-10 21:13:40.908497 cluster_colors-0.9.1/src/cluster_colors/vector_stacker.py
--rw-r--r--   0        0        0     4325 1970-01-01 00:00:00.000000 cluster_colors-0.9.1/setup.py
--rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 cluster_colors-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1457 2023-04-13 17:58:24.252444 cluster_colors-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     3533 2023-04-10 15:14:34.401917 cluster_colors-0.9.2/README.md
+-rw-r--r--   0        0        0      383 2023-03-14 23:49:36.976311 cluster_colors-0.9.2/src/cluster_colors/__init__.py
+-rw-r--r--   0        0        0    29449 2023-04-13 17:57:00.662409 cluster_colors-0.9.2/src/cluster_colors/clusters.py
+-rw-r--r--   0        0        0      290 2023-03-14 18:50:46.788014 cluster_colors-0.9.2/src/cluster_colors/config.py
+-rw-r--r--   0        0        0     3009 2023-03-14 02:27:27.128539 cluster_colors-0.9.2/src/cluster_colors/cut_colors.py
+-rw-r--r--   0        0        0     3004 2023-04-10 15:14:34.433735 cluster_colors-0.9.2/src/cluster_colors/distance_matrix.py
+-rw-r--r--   0        0        0     5239 2023-04-10 15:14:34.433735 cluster_colors-0.9.2/src/cluster_colors/image_colors.py
+-rw-r--r--   0        0        0     1290 2023-04-10 15:14:34.433735 cluster_colors-0.9.2/src/cluster_colors/kmedians.py
+-rw-r--r--   0        0        0      295 2023-03-13 11:40:04.953104 cluster_colors-0.9.2/src/cluster_colors/paths.py
+-rw-r--r--   0        0        0     5159 2023-03-19 19:41:53.291090 cluster_colors-0.9.2/src/cluster_colors/pool_colors.py
+-rw-r--r--   0        0        0        0 2023-03-09 22:18:11.789791 cluster_colors-0.9.2/src/cluster_colors/py.typed
+-rw-r--r--   0        0        0      908 2023-04-10 21:13:40.908497 cluster_colors-0.9.2/src/cluster_colors/type_hints.py
+-rw-r--r--   0        0        0     3245 2023-04-10 21:13:40.908497 cluster_colors-0.9.2/src/cluster_colors/vector_stacker.py
+-rw-r--r--   0        0        0     4325 1970-01-01 00:00:00.000000 cluster_colors-0.9.2/setup.py
+-rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 cluster_colors-0.9.2/PKG-INFO
```

### Comparing `cluster_colors-0.9.1/pyproject.toml` & `cluster_colors-0.9.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cluster-colors"
-version = "0.9.1"
+version = "0.9.2"
 description = "Cluster color vectors with kmedians"
 authors = ["Shay Hill <shay_public@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "cluster_colors", from = "src"}]
 
 [tool.poetry.dependencies]
@@ -21,15 +21,15 @@
 matplotlib = "^3.6.3"
 pre-commit = "^2.21.0"
 black = "^23.1.0"
 tox = "^4.4.7"
 
 [tool.commitizen]
 name = "cz_conventionalish"
-version = "0.9.1"
+version = "0.9.2"
 tag_format = "$version"
 version_files = [
     "pyproject.toml:^version"
 ]
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `cluster_colors-0.9.1/README.md` & `cluster_colors-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `cluster_colors-0.9.1/src/cluster_colors/clusters.py` & `cluster_colors-0.9.2/src/cluster_colors/clusters.py`

 * *Files 1% similar despite different names*

```diff
@@ -451,25 +451,30 @@
         :param max_count: The maximum number of clusters to allow.
         :param min_span: The minimum span to allow. If this is low and no max_count
             is given, expect to split all the way down to singletons, which could
             take several seconds.
         :return: The number of clusters in the state that was found.
         :raises StopIteration: if all states satisfy condition. In this case, we
             won't know if we are at the rightmost state.
+
+        When max count is one, prev will only ever have the value None. It is not
+        possible to fail other tests in this state, so the `prev or state` return
+        values will never be returned when prev is still None. This is because a
+        single cluster has a minimum span of infinity.
         """
         max_count = max_count or self._hard_max
         max_count = min(max_count, self._hard_max)
         min_span = 0 if min_span is None else min_span
         enumerated = self._enumerate()
-        prev = next(enumerated)  # will always be 1
+        prev = None
         for state in enumerated:
             if state.min_span < min_span:  # this is the first one that is too small
-                return prev
+                return prev or state
             if state.index_ > max_count:  # overshot because tied clusters were split
-                return prev
+                return prev or state
             if state.index_ == max_count:  # reached maximum count
                 return state
             prev = state
         raise StopIteration
 
 
 class Clusters:
@@ -768,8 +773,7 @@
 
         :return: a cluster that contains all members of all clusters
 
         This is a pathway to a Clusters instance sum weight, sum exemplar, etc.
         """
         members_list = [x.members for x in self.clusters]
         return Cluster(members_list[0].union(*members_list[1:]))
-        # return next(iter(self._states.seek_ge(1).clusters))
```

### Comparing `cluster_colors-0.9.1/src/cluster_colors/cut_colors.py` & `cluster_colors-0.9.2/src/cluster_colors/cut_colors.py`

 * *Files identical despite different names*

### Comparing `cluster_colors-0.9.1/src/cluster_colors/distance_matrix.py` & `cluster_colors-0.9.2/src/cluster_colors/distance_matrix.py`

 * *Files identical despite different names*

### Comparing `cluster_colors-0.9.1/src/cluster_colors/image_colors.py` & `cluster_colors-0.9.2/src/cluster_colors/image_colors.py`

 * *Files identical despite different names*

### Comparing `cluster_colors-0.9.1/src/cluster_colors/kmedians.py` & `cluster_colors-0.9.2/src/cluster_colors/kmedians.py`

 * *Files identical despite different names*

### Comparing `cluster_colors-0.9.1/src/cluster_colors/pool_colors.py` & `cluster_colors-0.9.2/src/cluster_colors/pool_colors.py`

 * *Files identical despite different names*

### Comparing `cluster_colors-0.9.1/src/cluster_colors/type_hints.py` & `cluster_colors-0.9.2/src/cluster_colors/type_hints.py`

 * *Files identical despite different names*

### Comparing `cluster_colors-0.9.1/src/cluster_colors/vector_stacker.py` & `cluster_colors-0.9.2/src/cluster_colors/vector_stacker.py`

 * *Files identical despite different names*

### Comparing `cluster_colors-0.9.1/setup.py` & `cluster_colors-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['colormath>=3.0.0,<4.0.0',
  'numpy>=1.24.1,<2.0.0',
  'paragraphs>=0.2.0,<0.3.0',
  'stacked-quantile>=0.3.0,<0.4.0']
 
 setup_kwargs = {
     'name': 'cluster-colors',
-    'version': '0.9.1',
+    'version': '0.9.2',
     'description': 'Cluster color vectors with kmedians',
     'long_description': 'Divisive (but not hierarchical) clustering.\n\nSlow, but clustering exactly how I want it. Iteratively split cluster with highest SSE. Splits are used to find new exemplars, which are thrown into k-medians with existing exemplars. Takes pretty extreme measures to avoid not only non-determinism but also non-arbitrary-ism:\n\n* a Clusters instance, when asked to split, will split the cluster with the highest SSE. If there is a tie, the Clusters instance will not arbitrarily decide between the tied clusters, but will instead split all clusters tied for max SSE. This means there is a small chance you will not be able to split a group of colors into exactly n clusters.\n* delta-e is non-commutative, so delta-e is computed *twice* for each distance (a -> b and b -> a). The maximum of these two is used. This doubles the time of an already slow calculation, but delta-e is only used for distances between clusters, and this module is designed to work with small numbers of clusters (Agglomerative clustering may be a better bet if you want to use small clusters.)\n\nAdvantages:\n* finds big clusters\n* deterministic and non-arbitrary\n* robust to outliers\n* fast for what it is, can easily split a few thousand members into a small number of clusters\n* decisions made early on do not effect the result as much as they would in true hierarchical clustering\n* has strategies to avoid ties or arbitrary (even if deterministic) decisions with small member sets. This is important when dealing with questions like "which of these five colors is most unlike the others?"\n\nDisadvantages:\n* child clusters will not necessarily contain (or only contain) the members of the parent, so this is not hierarchical, though you can "merge" split clusters by regressing to previous states.\n* sloooows down as the number of clusters grows, not the best way to de-cluster all the way back to constituent members.\n* uses Euclidean distance (sum squared error) for many steps. Delta e is used for final splitting criteria.\n\nThis clustering is designed for questions like "what are the five dominant colors in this image (respecting transparency)?"\n\n## Three large steps in the background\n\n### Average colors by n-bit representation\n\n`pool_colors`: reduce 8-bit image colors (potentially 16_777_216 colors) to a maximum of 262_144 by averaging. The ouput of `pool_colors` will also contain a weight axis for each color, representing the combined opacity of all pixels of that color.\n\n### Median cut along longest axis\n\n`cut_colors`: reduce colors to around 512 by recursively splitting along longest axis (longest actual axis. Not constrained to x, y, or, z axes).\n\n### k-medians clustering\n\n`KMediansClusters`: split and merge (undo split) clusters.\n\n* start with one cluster with 100 members\n* split this cluster recursively into five clusters (30, 30, 20, 10, 10)\n* ask for the largest cluster, and there\'s a tie\n* KMediansClusters will recursively unsplit clusters until all ties are broken. This will *rarely* be needed.\n\n\n## Installation\n\n    pip install cluster_colors\n\n## Basic usage\n\n~~~python\nfrom cluster_colors import get_image_clusters\n\nclusters = get_image_clusters(image_filename) # one cluster at this point\nclusters.split_to_delta_e(16)\nsplit_clusters = clusters.get_rsorted_clusters()\n\ncolors: list[tuple[float, float, float]] = [c.exemplar for c in split_clusters]\n\n# to save the cluster exemplars as an image file\n\nshow_clusters(split_clusters, "open_file_to_see_clusters")\n~~~\n',
     'author': 'Shay Hill',
     'author_email': 'shay_public@hotmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `cluster_colors-0.9.1/PKG-INFO` & `cluster_colors-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cluster-colors
-Version: 0.9.1
+Version: 0.9.2
 Summary: Cluster color vectors with kmedians
 License: MIT
 Author: Shay Hill
 Author-email: shay_public@hotmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

