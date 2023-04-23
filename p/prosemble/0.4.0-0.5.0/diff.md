# Comparing `tmp/prosemble-0.4.0.tar.gz` & `tmp/prosemble-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosemble-0.4.0.tar", last modified: Mon Apr  3 20:26:47 2023, max compression
+gzip compressed data, was "prosemble-0.5.0.tar", last modified: Sun Apr 23 19:58:20 2023, max compression
```

## Comparing `prosemble-0.4.0.tar` & `prosemble-0.5.0.tar`

### file list

```diff
@@ -1,35 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 20:26:47.489287 prosemble-0.4.0/
--rw-rw-rw-   0        0        0     1095 2022-05-22 15:35:18.000000 prosemble-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     1896 2023-04-03 20:26:47.489287 prosemble-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      924 2023-03-05 13:07:08.000000 prosemble-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-03 20:26:47.445993 prosemble-0.4.0/prosemble/
--rw-rw-rw-   0        0        0      128 2023-03-05 17:20:24.000000 prosemble-0.4.0/prosemble/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:26:47.464995 prosemble-0.4.0/prosemble/core/
--rw-rw-rw-   0        0        0      138 2023-04-02 22:26:45.000000 prosemble-0.4.0/prosemble/core/__init__.py
--rw-rw-rw-   0        0        0      420 2023-03-05 12:42:58.000000 prosemble-0.4.0/prosemble/core/distance.py
--rw-rw-rw-   0        0        0     6312 2023-04-03 20:22:45.000000 prosemble-0.4.0/prosemble/core/graphdata.py
--rw-rw-rw-   0        0        0        2 2023-03-03 22:57:08.000000 prosemble-0.4.0/prosemble/core/initializers.py
--rw-rw-rw-   0        0        0    38834 2022-09-17 20:19:36.000000 prosemble-0.4.0/prosemble/core/labelsecurity.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:26:47.487285 prosemble-0.4.0/prosemble/models/
--rw-rw-rw-   0        0        0      333 2023-04-03 14:41:47.000000 prosemble-0.4.0/prosemble/models/__init__.py
--rw-rw-rw-   0        0        0    11783 2023-04-02 23:14:14.000000 prosemble-0.4.0/prosemble/models/bgpc.py
--rw-rw-rw-   0        0        0    11062 2023-04-02 22:26:45.000000 prosemble-0.4.0/prosemble/models/fcm.py
--rw-rw-rw-   0        0        0    11838 2023-04-02 22:26:45.000000 prosemble-0.4.0/prosemble/models/fpcm.py
--rw-rw-rw-   0        0        0     8954 2023-04-02 22:26:45.000000 prosemble-0.4.0/prosemble/models/hcm.py
--rw-rw-rw-   0        0        0    18646 2023-04-02 22:26:45.000000 prosemble-0.4.0/prosemble/models/ipcm.py
--rw-rw-rw-   0        0        0    18455 2023-04-02 22:26:45.000000 prosemble-0.4.0/prosemble/models/ipcm_2.py
--rw-rw-rw-   0        0        0     5683 2023-04-02 22:26:45.000000 prosemble-0.4.0/prosemble/models/kmeans.py
--rw-rw-rw-   0        0        0     2070 2023-04-02 22:26:45.000000 prosemble-0.4.0/prosemble/models/knn.py
--rw-rw-rw-   0        0        0     2687 2023-04-02 22:26:45.000000 prosemble-0.4.0/prosemble/models/npc.py
--rw-rw-rw-   0        0        0    14305 2023-04-02 22:26:45.000000 prosemble-0.4.0/prosemble/models/pcm.py
--rw-rw-rw-   0        0        0    13648 2023-04-02 22:26:45.000000 prosemble-0.4.0/prosemble/models/pfcm.py
--rw-rw-rw-   0        0        0     3799 2023-03-05 12:48:40.000000 prosemble-0.4.0/prosemble/models/som.py
--rw-rw-rw-   0        0        0     8223 2023-04-03 14:20:26.000000 prosemble-0.4.0/prosemble/models/spectralclustering.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:26:47.454993 prosemble-0.4.0/prosemble.egg-info/
--rw-rw-rw-   0        0        0     1896 2023-04-03 20:26:47.000000 prosemble-0.4.0/prosemble.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      723 2023-04-03 20:26:47.000000 prosemble-0.4.0/prosemble.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 20:26:47.000000 prosemble-0.4.0/prosemble.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-04-03 20:26:47.000000 prosemble-0.4.0/prosemble.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-03 20:26:47.000000 prosemble-0.4.0/prosemble.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-03 20:26:47.489287 prosemble-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1327 2023-04-03 20:24:37.000000 prosemble-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 19:58:20.940987 prosemble-0.5.0/
+-rw-rw-rw-   0        0        0     1095 2022-05-22 15:35:18.000000 prosemble-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0     1896 2023-04-23 19:58:20.940987 prosemble-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0      924 2023-03-05 13:07:08.000000 prosemble-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 19:58:20.888859 prosemble-0.5.0/prosemble/
+-rw-rw-rw-   0        0        0      128 2023-04-23 19:39:20.000000 prosemble-0.5.0/prosemble/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 19:58:20.905826 prosemble-0.5.0/prosemble/core/
+-rw-rw-rw-   0        0        0      138 2023-04-02 22:26:45.000000 prosemble-0.5.0/prosemble/core/__init__.py
+-rw-rw-rw-   0        0        0      420 2023-03-05 12:42:58.000000 prosemble-0.5.0/prosemble/core/distance.py
+-rw-rw-rw-   0        0        0     6312 2023-04-03 20:22:45.000000 prosemble-0.5.0/prosemble/core/graphdata.py
+-rw-rw-rw-   0        0        0        2 2023-03-03 22:57:08.000000 prosemble-0.5.0/prosemble/core/initializers.py
+-rw-rw-rw-   0        0        0    38834 2022-09-17 20:19:36.000000 prosemble-0.5.0/prosemble/core/labelsecurity.py
+drwxrwxrwx   0        0        0        0 2023-04-23 19:58:20.938824 prosemble-0.5.0/prosemble/models/
+-rw-rw-rw-   0        0        0      446 2023-04-23 19:39:20.000000 prosemble-0.5.0/prosemble/models/__init__.py
+-rw-rw-rw-   0        0        0    14031 2023-04-23 16:47:52.000000 prosemble-0.5.0/prosemble/models/afcm.py
+-rw-rw-rw-   0        0        0    11784 2023-04-23 19:14:00.000000 prosemble-0.5.0/prosemble/models/bgpc.py
+-rw-rw-rw-   0        0        0    11062 2023-04-23 19:14:00.000000 prosemble-0.5.0/prosemble/models/fcm.py
+-rw-rw-rw-   0        0        0    11838 2023-04-23 19:14:01.000000 prosemble-0.5.0/prosemble/models/fpcm.py
+-rw-rw-rw-   0        0        0     8952 2023-04-23 19:14:01.000000 prosemble-0.5.0/prosemble/models/hcm.py
+-rw-rw-rw-   0        0        0    18646 2023-04-23 19:14:01.000000 prosemble-0.5.0/prosemble/models/ipcm.py
+-rw-rw-rw-   0        0        0    18455 2023-04-23 19:14:01.000000 prosemble-0.5.0/prosemble/models/ipcm_2.py
+-rw-rw-rw-   0        0        0    15410 2023-04-23 16:47:52.000000 prosemble-0.5.0/prosemble/models/kafcm.py
+-rw-rw-rw-   0        0        0    11772 2023-04-23 16:47:52.000000 prosemble-0.5.0/prosemble/models/kfcm.py
+-rw-rw-rw-   0        0        0    13516 2023-04-23 16:51:46.000000 prosemble-0.5.0/prosemble/models/kfpcm.py
+-rw-rw-rw-   0        0        0     5682 2023-04-23 19:14:01.000000 prosemble-0.5.0/prosemble/models/kmeans.py
+-rw-rw-rw-   0        0        0     2070 2023-04-02 22:26:45.000000 prosemble-0.5.0/prosemble/models/knn.py
+-rw-rw-rw-   0        0        0    15313 2023-04-23 16:27:34.000000 prosemble-0.5.0/prosemble/models/kpcm.py
+-rw-rw-rw-   0        0        0    16045 2023-04-23 16:27:34.000000 prosemble-0.5.0/prosemble/models/kpfcm.py
+-rw-rw-rw-   0        0        0     2687 2023-04-02 22:26:45.000000 prosemble-0.5.0/prosemble/models/npc.py
+-rw-rw-rw-   0        0        0    14305 2023-04-23 19:14:01.000000 prosemble-0.5.0/prosemble/models/pcm.py
+-rw-rw-rw-   0        0        0    13648 2023-04-23 19:14:01.000000 prosemble-0.5.0/prosemble/models/pfcm.py
+-rw-rw-rw-   0        0        0     3801 2023-04-23 19:14:01.000000 prosemble-0.5.0/prosemble/models/som.py
+-rw-rw-rw-   0        0        0     8223 2023-04-03 14:20:26.000000 prosemble-0.5.0/prosemble/models/spectralclustering.py
+drwxrwxrwx   0        0        0        0 2023-04-23 19:58:20.897825 prosemble-0.5.0/prosemble.egg-info/
+-rw-rw-rw-   0        0        0     1896 2023-04-23 19:58:20.000000 prosemble-0.5.0/prosemble.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      876 2023-04-23 19:58:20.000000 prosemble-0.5.0/prosemble.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 19:58:20.000000 prosemble-0.5.0/prosemble.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-04-23 19:58:20.000000 prosemble-0.5.0/prosemble.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-23 19:58:20.000000 prosemble-0.5.0/prosemble.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 19:58:20.941986 prosemble-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1327 2023-04-23 19:39:20.000000 prosemble-0.5.0/setup.py
```

### Comparing `prosemble-0.4.0/LICENSE` & `prosemble-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prosemble-0.4.0/PKG-INFO` & `prosemble-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosemble
-Version: 0.4.0
+Version: 0.5.0
 Summary: Prototype and non prototype-based machine learning package
 Home-page: https://github.com/naotoo1/prosemble
 Author: Nana Abeka Otoo
 Author-email: abekaotoo@gmail.com
 License: UNKNOWN
 Keywords: ensemble,Prototype models
 Platform: UNKNOWN
```

### Comparing `prosemble-0.4.0/README.md` & `prosemble-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `prosemble-0.4.0/prosemble/core/graphdata.py` & `prosemble-0.5.0/prosemble/core/graphdata.py`

 * *Files identical despite different names*

### Comparing `prosemble-0.4.0/prosemble/core/labelsecurity.py` & `prosemble-0.5.0/prosemble/core/labelsecurity.py`

 * *Files identical despite different names*

### Comparing `prosemble-0.4.0/prosemble/models/bgpc.py` & `prosemble-0.5.0/prosemble/models/bgpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,24 +109,24 @@
     def compute_centroids(self, u_matrix):
 
         fuzzified_assignments = [
             [u_ik[i] for _, u_ik in enumerate(u_matrix)]
             for i in range(self.num_clusters)
         ]
 
-        sum_fuzzified_assigments = [np.sum(i) for i in fuzzified_assignments]
+        sum_fuzzified_assignments = [np.sum(i) for i in fuzzified_assignments]
 
         centroid_numerator = [
             [np.multiply(fuzzified_assignments[cluster_index][index], sample)
              for index, sample in enumerate(self.data)]
             for cluster_index in range(self.num_clusters)
         ]
 
         centroids = np.array(
-            [np.sum(v, axis=0) / sum_fuzzified_assigments[i]
+            [np.sum(v, axis=0) / sum_fuzzified_assignments[i]
              for i, v in enumerate(centroid_numerator)]
         )
 
         return centroids
 
     def compute_beta_decay(self, iter):
         return 0.1 * np.power((self.b_f / 0.1), (iter / self.num_iter))
@@ -257,15 +257,15 @@
         """
         return self._get_cluster_results(self.fit_clus[0])
 
     def predict_new(self, x):
         """
 
         :param x: array-like: input vector
-        :return: cluster label of intput vector
+        :return: cluster label of input vector
         """
         return [
             self._nearest_centroids(sample, self.fit_cent[0])
             for index, sample in enumerate(x)
         ]
 
     def get_clusters_index_cent(self):
```

### Comparing `prosemble-0.4.0/prosemble/models/fcm.py` & `prosemble-0.5.0/prosemble/models/fcm.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     ord:  {non-zero int, inf, -inf, ‘fro’, ‘nuc’}
           order of the norm
 
     set_U_matrix: array-like:
         initial U matrix to  begin with. default is None
 
     plot_steps: bool:
-        True for visulisation of training and False otherwise
+        True for visualisation of training and False otherwise
 
     """
 
     def __init__(self, data, c, m, num_iter, epsilon, ord, set_U_matrix=None, plot_steps=False):
         self.data = data
         self.num_clusters = c
         self.fuzzifier = m
@@ -237,25 +237,25 @@
         """
         return self._get_cluster_results(self.fit_clus[0])
 
     def predict_new(self, x):
         """
 
         :param x:array-like: input vector
-        :return: cluster label of intput vector
+        :return: cluster label of input vector
         """
         return [self._nearest_centroids(sample, self.fit_cent[0]) for index, sample in enumerate(x)]
 
     def get_clusters_index_cent(self):
         return self.fit_clus, self.fit_cent
 
     def fit(self):
         """
 
-        :return: fits the model to the imput data set
+        :return: fits the model to the input data set
         """
         if self.num_iter is None:
             return self.get_centroids_()
         return self.get_centroids()
 
     def get_distance_space(self, x):
         """
```

### Comparing `prosemble-0.4.0/prosemble/models/fpcm.py` & `prosemble-0.5.0/prosemble/models/fpcm.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,15 +298,15 @@
                                    2 / (self.fuzzifier - 1)) / denomenator
                 final_matrix[i][j] = uik_new
         return final_matrix
 
     def get_prototypes(self, labels):
         """
 
-        :param labels: array-like: labels of the imput data set
+        :param labels: array-like: labels of the input data set
         :return: prototypes for the GNPC classifier design
         """
         self.fit()
         clusters_indices, centroids = self.fit_clus[0], self.fit_cent[0]
         clusters = [labels[cluster_with_indices] for cluster_with_indices in clusters_indices]
         max_occurrence = [dict(Counter(cluster)) for _, cluster in enumerate(clusters)]
         reposition_centroids = np.argsort([max(count, key=count.get) for count in max_occurrence])
```

### Comparing `prosemble-0.4.0/prosemble/models/hcm.py` & `prosemble-0.5.0/prosemble/models/hcm.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     ord:  {non-zero int, inf, -inf, ‘fro’, ‘nuc’}
           order of the norm
 
     set_prototypes: array-like:
         initial prototypes to  begin with. default is None
 
     plot_steps: bool:
-        True for visulisation of training and False otherwise
+        True for visualisation of training and False otherwise
 
     """
 
     def __init__(self, data, c, num_inter, epsilon, ord, set_prototypes=None, plot_steps=False):
         self.data = data
         self.num_clusters = c
         self.num_iter = num_inter
@@ -237,15 +237,15 @@
             init_proba[index][results] = 1
         return init_proba
 
     def get_prototypes(self, labels):
         """
 
         :param labels: array-like
-        :return: prototypes used as component initiatializer  for GNPC classifier design
+        :return: prototypes used as component initializer  for GNPC classifier design
         """
         self.fit()
         clusters_indices, centroids = self.fit_clus[0], self.fit_cent[0]
         clusters = [labels[cluster_with_indices] for cluster_with_indices in clusters_indices]
         max_occurrence = [dict(Counter(cluster)) for _, cluster in enumerate(clusters)]
         reposition_centroids = np.argsort([max(count, key=count.get) for count in max_occurrence])
         prototypes = centroids[reposition_centroids]
```

### Comparing `prosemble-0.4.0/prosemble/models/ipcm.py` & `prosemble-0.5.0/prosemble/models/ipcm.py`

 * *Files 0% similar despite different names*

```diff
@@ -466,15 +466,15 @@
                 tik_new = 1 / (1 + denomenator)
                 initial_t_matrix[i][j] = tik_new
         return initial_t_matrix
 
     def get_prototypes(self, labels):
         """
 
-        :param labels: array-like: labels of the imput data set
+        :param labels: array-like: labels of the input data set
         :return: prototypes for the GNPC classifier design
         """
         self.fit()
         clusters_indices, centroids = self.fit_clus[0], self.fit_cent[0]
         clusters = [labels[cluster_with_indices] for cluster_with_indices in clusters_indices]
         max_occurrence = [dict(Counter(cluster)) for _, cluster in enumerate(clusters)]
         reposition_centroids = np.argsort([max(count, key=count.get) for count in max_occurrence])
```

### Comparing `prosemble-0.4.0/prosemble/models/ipcm_2.py` & `prosemble-0.5.0/prosemble/models/ipcm_2.py`

 * *Files 0% similar despite different names*

```diff
@@ -461,15 +461,15 @@
                 initial_t_matrix[i][j] = tik_new
         return initial_t_matrix
 
     # Classification aspect
     def get_prototypes(self, labels):
         """
 
-        :param labels: array-like: labels of the imput data set
+        :param labels: array-like: labels of the input data set
         :return: prototypes for the GNPC classifier design
         """
         self.fit()
         clusters_indices, centroids = self.fit_clus[0], self.fit_cent[0]
         clusters = [labels[cluster_with_indices] for cluster_with_indices in clusters_indices]
         max_occurrence = [dict(Counter(cluster)) for _, cluster in enumerate(clusters)]
         reposition_centroids = np.argsort([max(count, key=count.get) for count in max_occurrence])
```

### Comparing `prosemble-0.4.0/prosemble/models/kmeans.py` & `prosemble-0.5.0/prosemble/models/kmeans.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         return self.model.get_distance_space(x)
 
     # classification aspect
     def get_prototypes_class(self, labels):
         """
 
         :param labels: array-like: labels of the input data set
-        :return: component initiatlizer for GNPC classifier designs
+        :return: component initializer for GNPC classifier designs
         """
         return self.model.get_prototypes(labels)
 
     def predict_proba(self, x):
         """
 
         :param x: input vector
```

### Comparing `prosemble-0.4.0/prosemble/models/knn.py` & `prosemble-0.5.0/prosemble/models/knn.py`

 * *Files identical despite different names*

### Comparing `prosemble-0.4.0/prosemble/models/npc.py` & `prosemble-0.5.0/prosemble/models/npc.py`

 * *Files identical despite different names*

### Comparing `prosemble-0.4.0/prosemble/models/pcm.py` & `prosemble-0.5.0/prosemble/models/pcm.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,15 +296,15 @@
         """
 
         return self.objective_function
 
     def predict(self):
         """
 
-        :return: array-like: cluster lables of input data
+        :return: array-like: cluster labels of input data
         """
         return self._get_cluster_results(self.fit_clus[0])
 
     def predict_new(self, x):
         """
 
         :param x: array-like: input vector
```

### Comparing `prosemble-0.4.0/prosemble/models/pfcm.py` & `prosemble-0.5.0/prosemble/models/pfcm.py`

 * *Files 0% similar despite different names*

```diff
@@ -361,15 +361,15 @@
                                    2 / (self.fuzzifier - 1)) / denomenator
                 final_matrix[i][j] = uik_new
         return final_matrix
 
     def get_prototypes(self, labels):
         """
 
-        :param labels: array-like: labels of the imput data set
+        :param labels: array-like: labels of the input data set
         :return: prototypes for the GNPC classifier design
         """
         self.fit()
         clusters_indices, centroids = self.fit_clus[0], self.fit_cent[0]
         clusters = [labels[cluster_with_indices] for cluster_with_indices in clusters_indices]
         max_occurrence = [dict(Counter(cluster)) for _, cluster in enumerate(clusters)]
         reposition_centroids = np.argsort([max(count, key=count.get) for count in max_occurrence])
```

### Comparing `prosemble-0.4.0/prosemble/models/som.py` & `prosemble-0.5.0/prosemble/models/som.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
                     shortest_distance = distance
                     winner = [row, col]
         return winner
 
     def fit(self):
         for step in range(self.num_iter):
             learning_rate, neighbourhood_range = self.lr_decay(num_iter=step, distance_n=4)
-            rand_sample_index = np.random.randint(0, high=self.data.shape[0])  # random index of traing data
+            rand_sample_index = np.random.randint(0, high=self.data.shape[0])  # random index of training data
             winner = self.winning_neuron(data=self.data, t=rand_sample_index)
             for row in range(self.grid):
                 for col in range(self.grid):
                     if manhattan_distance([row, col], winner) <= neighbourhood_range:
                         self.som[row][col] += learning_rate * (
                                 self.data[rand_sample_index] - self.som[row][col])  # update neighbour's weight
         return self.som
```

### Comparing `prosemble-0.4.0/prosemble/models/spectralclustering.py` & `prosemble-0.5.0/prosemble/models/spectralclustering.py`

 * *Files identical despite different names*

### Comparing `prosemble-0.4.0/prosemble.egg-info/PKG-INFO` & `prosemble-0.5.0/prosemble.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosemble
-Version: 0.4.0
+Version: 0.5.0
 Summary: Prototype and non prototype-based machine learning package
 Home-page: https://github.com/naotoo1/prosemble
 Author: Nana Abeka Otoo
 Author-email: abekaotoo@gmail.com
 License: UNKNOWN
 Keywords: ensemble,Prototype models
 Platform: UNKNOWN
```

### Comparing `prosemble-0.4.0/prosemble.egg-info/SOURCES.txt` & `prosemble-0.5.0/prosemble.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -9,20 +9,26 @@
 prosemble.egg-info/top_level.txt
 prosemble/core/__init__.py
 prosemble/core/distance.py
 prosemble/core/graphdata.py
 prosemble/core/initializers.py
 prosemble/core/labelsecurity.py
 prosemble/models/__init__.py
+prosemble/models/afcm.py
 prosemble/models/bgpc.py
 prosemble/models/fcm.py
 prosemble/models/fpcm.py
 prosemble/models/hcm.py
 prosemble/models/ipcm.py
 prosemble/models/ipcm_2.py
+prosemble/models/kafcm.py
+prosemble/models/kfcm.py
+prosemble/models/kfpcm.py
 prosemble/models/kmeans.py
 prosemble/models/knn.py
+prosemble/models/kpcm.py
+prosemble/models/kpfcm.py
 prosemble/models/npc.py
 prosemble/models/pcm.py
 prosemble/models/pfcm.py
 prosemble/models/som.py
 prosemble/models/spectralclustering.py
```

### Comparing `prosemble-0.4.0/setup.py` & `prosemble-0.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="prosemble",
-    version="0.4.0",
+    version="0.5.0",
     author="Nana Abeka Otoo",
     author_email="abekaotoo@gmail.com",
     description="Prototype and non prototype-based machine learning package",
     url="https://github.com/naotoo1/prosemble",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
```

