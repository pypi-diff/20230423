# Comparing `tmp/scace-0.1.0.tar.gz` & `tmp/scace-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scace-0.1.0.tar", last modified: Tue Feb 21 14:12:03 2023, max compression
+gzip compressed data, was "scace-0.1.1.tar", last modified: Sun Apr 23 12:07:35 2023, max compression
```

## Comparing `scace-0.1.0.tar` & `scace-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-02-21 14:12:03.733773 scace-0.1.0/
--rw-rw-rw-   0        0        0     3376 2023-02-21 14:12:03.732776 scace-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2330 2023-02-21 13:47:37.000000 scace-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-02-21 14:12:03.700978 scace-0.1.0/scace/
--rw-rw-rw-   0        0        0      381 2023-02-21 14:11:58.000000 scace-0.1.0/scace/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-21 14:12:03.710608 scace-0.1.0/scace/model/
--rw-rw-rw-   0        0        0      100 2023-02-21 06:30:13.000000 scace-0.1.0/scace/model/__init__.py
--rw-rw-rw-   0        0        0    10712 2023-02-21 07:01:43.000000 scace-0.1.0/scace/model/merge_split.py
--rw-rw-rw-   0        0        0     5079 2023-02-16 15:26:20.000000 scace-0.1.0/scace/model/scace_net.py
--rw-rw-rw-   0        0        0    11672 2023-02-21 13:16:45.000000 scace-0.1.0/scace/scace_train.py
-drwxrwxrwx   0        0        0        0 2023-02-21 14:12:03.718418 scace-0.1.0/scace/util/
--rw-rw-rw-   0        0        0      106 2023-02-16 17:04:36.000000 scace-0.1.0/scace/util/__init__.py
--rw-rw-rw-   0        0        0      641 2023-02-21 13:52:48.000000 scace-0.1.0/scace/util/data_utils.py
--rw-rw-rw-   0        0        0     1620 2023-02-16 16:24:04.000000 scace-0.1.0/scace/util/losses.py
--rw-rw-rw-   0        0        0     2478 2023-02-17 09:07:42.000000 scace-0.1.0/scace/util/tools.py
-drwxrwxrwx   0        0        0        0 2023-02-21 14:12:03.707166 scace-0.1.0/scace.egg-info/
--rw-rw-rw-   0        0        0     3376 2023-02-21 14:12:03.000000 scace-0.1.0/scace.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      606 2023-02-21 14:12:03.000000 scace-0.1.0/scace.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-21 14:12:03.000000 scace-0.1.0/scace.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-02-21 14:12:03.000000 scace-0.1.0/scace.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-02-21 14:12:03.000000 scace-0.1.0/scace.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-21 14:12:03.721426 scace-0.1.0/scace_new/
--rw-rw-rw-   0        0        0      381 2023-02-17 07:27:20.000000 scace-0.1.0/scace_new/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-21 14:12:03.725503 scace-0.1.0/scace_new/model/
--rw-rw-rw-   0        0        0      119 2023-02-21 06:54:56.000000 scace-0.1.0/scace_new/model/__init__.py
--rw-rw-rw-   0        0        0    10696 2023-02-21 06:54:56.000000 scace-0.1.0/scace_new/model/merge_split.py
--rw-rw-rw-   0        0        0     5079 2023-02-16 15:26:20.000000 scace-0.1.0/scace_new/model/scace_net.py
--rw-rw-rw-   0        0        0    11784 2023-02-21 12:21:32.000000 scace-0.1.0/scace_new/scace_train.py
-drwxrwxrwx   0        0        0        0 2023-02-21 14:12:03.730778 scace-0.1.0/scace_new/util/
--rw-rw-rw-   0        0        0      106 2023-02-16 17:04:36.000000 scace-0.1.0/scace_new/util/__init__.py
--rw-rw-rw-   0        0        0      539 2023-02-17 01:40:30.000000 scace-0.1.0/scace_new/util/data_utils.py
--rw-rw-rw-   0        0        0     1620 2023-02-16 16:24:04.000000 scace-0.1.0/scace_new/util/losses.py
--rw-rw-rw-   0        0        0     2478 2023-02-17 09:07:42.000000 scace-0.1.0/scace_new/util/tools.py
--rw-rw-rw-   0        0        0       42 2023-02-21 14:12:03.734772 scace-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1177 2023-02-21 14:11:17.000000 scace-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 12:07:35.092735 scace-0.1.1/
+-rw-rw-rw-   0        0        0     3276 2023-04-23 12:07:35.092735 scace-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2325 2023-02-24 03:35:01.000000 scace-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 12:07:35.073057 scace-0.1.1/scace/
+-rw-rw-rw-   0        0        0      381 2023-04-23 11:52:35.000000 scace-0.1.1/scace/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 12:07:35.084440 scace-0.1.1/scace/model/
+-rw-rw-rw-   0        0        0      119 2023-04-23 11:52:35.000000 scace-0.1.1/scace/model/__init__.py
+-rw-rw-rw-   0        0        0    10356 2023-04-23 11:52:35.000000 scace-0.1.1/scace/model/merge_split.py
+-rw-rw-rw-   0        0        0     5079 2023-02-16 15:26:20.000000 scace-0.1.1/scace/model/scace_net.py
+-rw-rw-rw-   0        0        0    12303 2023-04-23 11:55:52.000000 scace-0.1.1/scace/scace_train.py
+drwxrwxrwx   0        0        0        0 2023-04-23 12:07:35.090530 scace-0.1.1/scace/util/
+-rw-rw-rw-   0        0        0      106 2023-02-16 17:04:36.000000 scace-0.1.1/scace/util/__init__.py
+-rw-rw-rw-   0        0        0      641 2023-02-21 13:52:48.000000 scace-0.1.1/scace/util/data_utils.py
+-rw-rw-rw-   0        0        0     1548 2023-04-23 11:52:35.000000 scace-0.1.1/scace/util/losses.py
+-rw-rw-rw-   0        0        0     3538 2023-04-23 11:52:35.000000 scace-0.1.1/scace/util/tools.py
+drwxrwxrwx   0        0        0        0 2023-04-23 12:07:35.081618 scace-0.1.1/scace.egg-info/
+-rw-rw-rw-   0        0        0     3276 2023-04-23 12:07:34.000000 scace-0.1.1/scace.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-04-23 12:07:35.000000 scace-0.1.1/scace.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 12:07:35.000000 scace-0.1.1/scace.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-04-23 12:07:35.000000 scace-0.1.1/scace.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-23 12:07:35.000000 scace-0.1.1/scace.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 12:07:35.092735 scace-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1177 2023-04-23 12:07:13.000000 scace-0.1.1/setup.py
```

### Comparing `scace-0.1.0/PKG-INFO` & `scace-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: scace
-Version: 0.1.0
+Version: 0.1.1
 Summary: scAce: an adaptive embedding and clustering method for single-cell gene expression data
 Home-page: https://github.com/sldyns/scAce
 Author: Kun Qian, Xinwei He
 Author-email: kun_qian@foxmail.com
 Maintainer: Kun Qian
 Maintainer-email: kun_qian@foxmail.com
 License: MIT Licence
-Description: # scAce: an adaptive embedding and clustering method
+Description: # scAce: an adaptive embedding and clustering method for scRNA-seq data
         
         ## Overview
         
         scAce is consisted of three major steps, a pre-training step based on a variational autoencoder, a cluster initialization step to obtain initial cluster labels, and an adaptive cluster merging step to iteratively
         update cluster labels and cell embeddings. In the pre-training step, scAce takes the single-cell gene expression matrix as its input to train a VAE network. For each gene, the VAE learns and outputs three parameters of a ZINB distribution (mean, dispersion, and proportion of zero). In the cluster initialization step, scAce offeres two manners. With *de novo* initialization, Leiden is used to obtain initial cluster labels; with clustering enhancement, initial cluster labels are obtained by applying a cluster splitting approach to a set of existing clustering results. In the adaptive cluster merging step,  given the pre-trained VAE network and the initial cluster labels, the network parameters, cell embeddings, cluster labels and centroids are iteratively updated by alternately performing network update and cluster merging steps. The final results of cell embeddings and cluster labels are output by scAce after the iteration process stops.
         
         ## Installation
         
-        You can install `scAce` from pypi with:
+        Please install `scAce` from pypi with:
         
         ```
         pip install scace
         ```
-        Or clone this repository and using
+        Or clone this repository and use
         
         ```
         pip install -e .
         ```
         in the root of this repository.
-        ## Usage
+        ## Quick start
         
         Load the data to be analyzed:
         
         ```
         import scanpy as sc
         
         adata = sc.AnnData(data)
@@ -51,27 +51,23 @@
         sc.pp.normalize_per_cell(adata)
         adata.obs['scale_factor'] = adata.obs.n_counts / adata.obs.n_counts.median()
         
         sc.pp.log1p(adata)
         sc.pp.scale(adata)
         ```
         
-        Run scAce algorithm:
+        Run the scAce method:
         
         ```
         from scace import run_scace
         adata = run_scace(adata)
         ```
         
-        The output adata contains cluster labels in `adata.obs['scace_cluster']` and the resulting embedding in `adata.obsm['scace_emb']`, this embedding can be used as input of other downstream task.
+        The output adata contains cluster labels in `adata.obs['scace_cluster']` and the cell embeddings in `adata.obsm['scace_emb']`. The embeddings can be used as input of other downstream analyses.
         
-        To see an example, please refer to `tutorial.ipynb`.
+        <ins>Please refer to `tutorial.ipynb` for a detailed description of scAce's usage.<ins>
         
-        ## Reproduce results
         
-        See folder `reproducibility`.
-        
-        Follow `README.md` in `data` and `pkgs` to prepare data and packages.
         
 Keywords: single-cell RNA-sequencing,clustering,cluster merging
 Platform: any
 Description-Content-Type: text/markdown
```

### Comparing `scace-0.1.0/README.md` & `scace-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,59 @@
-# scAce: an adaptive embedding and clustering method
-
-## Overview
-
-scAce is consisted of three major steps, a pre-training step based on a variational autoencoder, a cluster initialization step to obtain initial cluster labels, and an adaptive cluster merging step to iteratively
-update cluster labels and cell embeddings. In the pre-training step, scAce takes the single-cell gene expression matrix as its input to train a VAE network. For each gene, the VAE learns and outputs three parameters of a ZINB distribution (mean, dispersion, and proportion of zero). In the cluster initialization step, scAce offeres two manners. With *de novo* initialization, Leiden is used to obtain initial cluster labels; with clustering enhancement, initial cluster labels are obtained by applying a cluster splitting approach to a set of existing clustering results. In the adaptive cluster merging step,  given the pre-trained VAE network and the initial cluster labels, the network parameters, cell embeddings, cluster labels and centroids are iteratively updated by alternately performing network update and cluster merging steps. The final results of cell embeddings and cluster labels are output by scAce after the iteration process stops.
-
-## Installation
-
-You can install `scAce` from pypi with:
-
-```
-pip install scace
-```
-Or clone this repository and using
-
-```
-pip install -e .
-```
-in the root of this repository.
-## Usage
-
-Load the data to be analyzed:
-
-```
-import scanpy as sc
-
-adata = sc.AnnData(data)
-```
-
-Perform data pre-processing:
-
-```
-# Basic filtering
-sc.pp.filter_genes(adata, min_cells=3)
-sc.pp.filter_cells(adata, min_genes=200)
-
-adata.raw = adata.copy()
-
-# Total-count normlize, logarithmize and scale the data  
-sc.pp.normalize_per_cell(adata)
-adata.obs['scale_factor'] = adata.obs.n_counts / adata.obs.n_counts.median()
-
-sc.pp.log1p(adata)
-sc.pp.scale(adata)
-```
-
-Run scAce algorithm:
-
-```
-from scace import run_scace
-adata = run_scace(adata)
-```
-
-The output adata contains cluster labels in `adata.obs['scace_cluster']` and the resulting embedding in `adata.obsm['scace_emb']`, this embedding can be used as input of other downstream task.
-
-To see an example, please refer to `tutorial.ipynb`.
-
-## Reproduce results
-
-See folder `reproducibility`.
-
-Follow `README.md` in `data` and `pkgs` to prepare data and packages.
+# scAce: an adaptive embedding and clustering method for scRNA-seq data
+
+## Overview
+
+scAce is consisted of three major steps, a pre-training step based on a variational autoencoder, a cluster initialization step to obtain initial cluster labels, and an adaptive cluster merging step to iteratively
+update cluster labels and cell embeddings. In the pre-training step, scAce takes the single-cell gene expression matrix as its input to train a VAE network. For each gene, the VAE learns and outputs three parameters of a ZINB distribution (mean, dispersion, and proportion of zero). In the cluster initialization step, scAce offeres two manners. With *de novo* initialization, Leiden is used to obtain initial cluster labels; with clustering enhancement, initial cluster labels are obtained by applying a cluster splitting approach to a set of existing clustering results. In the adaptive cluster merging step,  given the pre-trained VAE network and the initial cluster labels, the network parameters, cell embeddings, cluster labels and centroids are iteratively updated by alternately performing network update and cluster merging steps. The final results of cell embeddings and cluster labels are output by scAce after the iteration process stops.
+
+## Installation
+
+Please install `scAce` from pypi with:
+
+```
+pip install scace
+```
+Or clone this repository and use
+
+```
+pip install -e .
+```
+in the root of this repository.
+## Quick start
+
+Load the data to be analyzed:
+
+```
+import scanpy as sc
+
+adata = sc.AnnData(data)
+```
+
+Perform data pre-processing:
+
+```
+# Basic filtering
+sc.pp.filter_genes(adata, min_cells=3)
+sc.pp.filter_cells(adata, min_genes=200)
+
+adata.raw = adata.copy()
+
+# Total-count normlize, logarithmize and scale the data  
+sc.pp.normalize_per_cell(adata)
+adata.obs['scale_factor'] = adata.obs.n_counts / adata.obs.n_counts.median()
+
+sc.pp.log1p(adata)
+sc.pp.scale(adata)
+```
+
+Run the scAce method:
+
+```
+from scace import run_scace
+adata = run_scace(adata)
+```
+
+The output adata contains cluster labels in `adata.obs['scace_cluster']` and the cell embeddings in `adata.obsm['scace_emb']`. The embeddings can be used as input of other downstream analyses.
+
+<ins>Please refer to `tutorial.ipynb` for a detailed description of scAce's usage.<ins>
+
+
```

### Comparing `scace-0.1.0/scace/model/merge_split.py` & `scace-0.1.1/scace/model/merge_split.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,26 +9,24 @@
         intra_dis.append(np.sum(cluster_dis) / data_cluster.shape[0])
 
     return intra_dis
 
 
 def merge_compute(y_pred, mu, scace_emb):
 
-    n_clusters = len(np.unique(y_pred))
-
     # Check if len(mu_prepare) == len(np.unique(y_pred))
     idx_cent = []
     for i in range(len(mu)):
         if (y_pred == i).any() == False:
             idx_cent.append(i)
     if len(idx_cent) == 0:
         mu = mu
     else:
         mu = np.delete(mu, idx_cent, 0)
-        n_clusters = len(mu)
+    n_clusters = len(mu)
 
     # Change label to 0 ~ len(np.unique(label))
     for i in range(len(np.unique(y_pred))):
         if np.unique(y_pred)[i] != i:
             y_pred[y_pred == np.unique(y_pred)[i]] = i
 
 
@@ -42,32 +40,27 @@
     for i in range(0, n_clusters):
         for j in range(i + 1, n_clusters):
             weight = d_ave / ((intra_dis[i] + intra_dis[j]) / 2)
             sum_1 += weight * np.linalg.norm(Centroid[i] - Centroid[j])
 
     d_bar = sum_1 / (n_clusters * (n_clusters - 1))
 
-    return y_pred, Centroid, d_bar, intra_dis, d_ave, n_clusters
+    return y_pred, Centroid, d_bar, intra_dis, d_ave
 
 
 
 def centroid_merge(X, cent_to_merge, label, min_dis, intra_dis, d_ave):
-    # d_bar_f = []
-    # d_inter_f = []
+
     pred_f = []
 
     for t in range(200):
 
-        # d_bar_f.append(min_dis)
         if t == 0:
             pred_f.append(label)
 
-        # intra_dis = cluster_intra_dis(X, cent_to_merge, label)
-        # d_ave = np.mean(intra_dis)
-
         Cent_dis = []
         Cent_i = []
         Cent_e = []
         Final_Centroid_merge = cent_to_merge
 
         n_Clusters = len(Final_Centroid_merge)
 
@@ -75,16 +68,14 @@
             for e in range(i + 1, n_Clusters):
                 weight = d_ave / ((intra_dis[i] + intra_dis[e]) / 2)
                 dis = np.linalg.norm(Final_Centroid_merge[i] - Final_Centroid_merge[e])
                 Cent_dis.append(weight * dis)
                 Cent_i.append(i)
                 Cent_e.append(e)
 
-        # d_inter_f.append(np.round(np.asarray(Cent_dis), 2))
-
         for i in range(len(Cent_dis)):
             if Cent_dis[i] < min_dis and Cent_dis[i] == min(Cent_dis):
 
                 Cent_merge = (Final_Centroid_merge[Cent_i[i]] + Final_Centroid_merge[Cent_e[i]]) / 2
 
                 Final_Centroid_merge = np.delete(Final_Centroid_merge, (Cent_i[i], Cent_e[i]), 0)
                 Final_Centroid_merge = np.insert(Final_Centroid_merge, Cent_i[i], Cent_merge, 0)
@@ -105,26 +96,21 @@
 
             else:
                 pass
 
         n_clusters_t = len(np.unique(label))
         pred_f.append(label)
 
-        # adata.obs['pred'] = np.array(label).squeeze()
-        # adata.obs['pred'] = adata.obs['pred'].astype(str).astype('category')
-        # sc.pl.tsne(adata, color=['pred'])
-
         intra_dis = cluster_intra_dis(X, cent_to_merge, label)
         d_ave = np.mean(intra_dis)
 
         sum_1 = 0
         for i in range(n_clusters_t):
             for j in range(i + 1, n_clusters_t):
                 weight = d_ave / ((intra_dis[i] + intra_dis[j]) / 2)
-                # weight = 1
 
                 sum_1 += weight * (np.linalg.norm(Final_Centroid_merge[i] - Final_Centroid_merge[j]))
 
         d_bar = sum_1 / (n_clusters_t * (n_clusters_t - 1))
 
         min_dis = d_bar
 
@@ -152,20 +138,24 @@
             continue
 
     return Final_Centroid_merge, label, n_clusters_t, pred_f
 
 
 
 def centroid_split(X, X_1, Centroid_split, label):
-    '''
-    X: 计数矩阵
-    X_1：计数矩阵 + 标签(标签放最后一列)
-    '''
+    """
+        Parameters
+        ----------
+        X
+            Embedding after pre-training. Rows are cells and columns are genes.
+        X_1
+            Embedding + Column vectors of cell types (Label splicing in the last column).
+    """
 
-    ### 算权重
+    ### Compute weights
     intra_dis = cluster_intra_dis(X, Centroid_split, label)
     d_ave = np.mean(intra_dis)
 
     sum_1 = 0
     n_clusters = len(np.unique(label))
     for i in range(0, n_clusters):
         for j in range(i + 1, n_clusters):
@@ -265,15 +255,15 @@
                     continue
             label = label.tolist()
 
         n_clusters = Centroid_split.shape[0]
         X_1 = np.concatenate([np.array(X), np.array(label).reshape(len(label), 1)], axis=1)
         X_copy = 1 * X_1
 
-        ### Calculate weights
+        ### Compute weights
         intra_dis = cluster_intra_dis(X, Centroid_split, np.array(label))
         d_ave = np.mean(intra_dis)
 
         sum_1 = 0
         for i in range(0, n_clusters):
             for j in range(i + 1, n_clusters):
                 weight = d_ave / ((intra_dis[i] + intra_dis[j]) / 2)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `scace-0.1.0/scace/model/scace_net.py` & `scace-0.1.1/scace/model/scace_net.py`

 * *Files identical despite different names*

### Comparing `scace-0.1.0/scace/scace_train.py` & `scace-0.1.1/scace/scace_train.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 import torch.optim as optim
 from torch.nn import Parameter
 from torch.utils.data import DataLoader
 from tqdm import tqdm
 
 from .model import scAce, centroid_merge, merge_compute
 from .util import scDataset, ZINBLoss, ClusterLoss, ELOBkldLoss, clustering, calculate_metric, compute_mu
-
+import time
 
 def run_scace(adata: sc.AnnData,
-              n_epochs_pre: int = 300,
+              n_epochs_pre: int = 200,
               n_epochs: int = 500,
               batch_size: int = 256,
               lr: float = 1e-4,
               resolution: float = 2,
               init_cluster=None,
+              init_method='leiden',
               cl_type=None,
               save_pretrain: bool = False,
               saved_ckpt: str = None,
               pretrained_ckpt: str = None,
               return_all: bool = False):
     """
         Train scAce.
@@ -33,17 +34,19 @@
         n_epochs
             Number of total epochs in training.
         batch_size
             Number of cells for training in one epoch.
         lr
             Learning rate for AdamOptimizer.
         resolution
-            The resolution parameter of sc.tl.leiden for the initial clustering.
+            The resolution parameter of sc.tl.leiden or sc.tl.louvain for the initial clustering.
         init_cluster
             Initial cluster results. If provided, perform cluster splitting after pre-training.
+        init_method
+            Method used for cluster initialization. Default is 'leiden', optionally input 'leiden', 'louvain' or 'kmeans'.
         save_pretrain
             If True, save the pre-trained model.
         saved_ckpt
             File name of pre-trained model to be saved, only used when save_pretrain is True.
         pretrained_ckpt
             File name of saved pre-trained model. If provided, load the saved pre-trained model without performing
             pre-training step.
@@ -63,14 +66,16 @@
             Final ARI. Will be returned if 'return_all' is True and cell type information is provided.
         K
             Final number of clusters. Will be returned if 'return_all' is True.
         pred_all
             All temporary clustering results. Will be returned if 'return_all' is True.
         emb_all
             All temporary embedding. Will be returned if 'return_all' is True.
+        run_time
+            Time spent in training.
     """
 
     ####################   Assert several input variables  ########################
     # To print and store all temporary results
     if return_all:
         pred_all, emb_all = [], []
 
@@ -90,34 +95,37 @@
     # Create dataset
     train_dataset = scDataset(raw_mat, exp_mat, scale_factor)
     train_loader = DataLoader(train_dataset, batch_size=batch_size, shuffle=True, num_workers=0)
     n_iters = len(train_loader)
 
     ####################   Set some parameters   #################
     # hyper-parameter
-    kld_w = 0.001
+    kld_w2 = 0.01
+    kld_w1 = 0.001
     z_dim = 32
     encode_layers = [512]
     decode_layers = [512]
     activation = 'relu'
 
     # parameter for training
-    tol, clu_w, m_numbers = 0.05, 1., 0
+    tol, clu_w, m_numbers = 0.05, 1, 0
     merge_flag = True
 
     #######################   Prepare models & optimzers & loss  #######################
     input_dim = adata.X.shape[1]
 
     scace_model = scAce(input_dim=input_dim, device=device, z_dim=z_dim, encode_layers=encode_layers,
                         decode_layers=decode_layers, activation=activation).to(device)
 
     optimizer = optim.Adam(params=scace_model.parameters(), lr=lr)
 
     ZINB_Loss, KLD_Loss, Cluster_Loss = ZINBLoss(ridge_lambda=0), ELOBkldLoss(), ClusterLoss()
 
+    start = time.time()
+
     ###########################   Pre-training   #########################
     if pretrained_ckpt:
         print('Pre-trained model provided, load checkpoint from file "{}".'.format(pretrained_ckpt))
 
         scace_model.load_state_dict(torch.load(pretrained_ckpt))
 
     else:
@@ -133,15 +141,15 @@
                 raw, exp, sf = raw.to(device), exp.to(device), sf.to(device)
                 z_mu, z_logvar, mu, disp, pi = scace_model(exp)
 
                 # VAE Loss
                 zinb_loss = ZINB_Loss(x=raw, mean=mu, disp=disp, pi=pi, scale_factor=sf)
                 kld_loss = KLD_Loss(z_mu, z_logvar)
 
-                loss = zinb_loss + kld_w * kld_loss
+                loss = zinb_loss + kld_w1 * kld_loss
                 optimizer.zero_grad()
                 loss.backward()
                 optimizer.step()
 
                 # Record losses
                 if return_all:
                     avg_zinb += zinb_loss.item() / n_iters
@@ -164,16 +172,19 @@
 
     # Initial clustering
     if init_cluster is not None:
         print('Perform initial clustering through cluster split with provided cluster labels')
         y_pred_last, mu, scace_emb = clustering(scace_model, exp_mat, init_cluster=init_cluster)
 
     else:
-        print('Perform initial clustering through Leiden with resolution = {}'.format(resolution))
-        y_pred_last, mu, scace_emb = clustering(scace_model, exp_mat, resolution=resolution)
+        if init_method == 'kmeans':
+            print('Perform initial clustering through K-means')
+        else:
+            print('Perform initial clustering through {} with resolution = {}'.format(init_method, resolution))
+        y_pred_last, mu, scace_emb = clustering(scace_model, exp_mat, init_method, resolution=resolution)
 
     # Number of initial clusters
     n_clusters = len(np.unique(y_pred_last))
     print('Finish initial clustering! Number of initial clusters is {}'.format(n_clusters))
 
     # Initial parameter mu
     scace_model.mu = Parameter(torch.Tensor(n_clusters, scace_model.z_dim).to(device))
@@ -203,30 +214,31 @@
         # Check stop & cluster merging criterion
         delta_label = np.sum(y_pred != y_pred_last).astype(np.float32) / len(y_pred)
         y_pred_last = y_pred
 
         if epoch > 0 and delta_label < tol:
             if not merge_flag: print("Reach tolerance threshold. Stopping training."); break
 
+        if epoch > 0 and (delta_label < tol or epoch % 20 == 0):
+
             print('Reach tolerance threshold. Perform cluster merging.')
 
             mu_prepare = scace_model.mu.cpu().detach().numpy()
-            y_pred, Centroid, d_bar, intra_dis, d_ave, n_clusters = merge_compute(y_pred, mu_prepare, scace_emb)
+            y_pred, Centroid, d_bar, intra_dis, d_ave = merge_compute(y_pred, mu_prepare, scace_emb)
 
             Final_Centroid_merge, Label_merge, n_clusters_t, pred_t = centroid_merge(scace_emb, Centroid, y_pred, d_bar, intra_dis, d_ave)
             m_numbers += 1
 
-            # If n_clusters not change, stop merging clusters
+            # n_clusters not change, stop merging clusters
             if m_numbers > 1 and n_clusters_t == n_clusters:
                 merge_flag, tol = False, tol / 10.
                 print('Stop merging clusters! Continue updating several rounds.')
 
             else:
                 n_clusters = n_clusters_t
-
                 y_pred = Label_merge
 
                 mu = compute_mu(scace_emb, y_pred)
 
                 scace_model.mu = Parameter(torch.Tensor(n_clusters, scace_model.z_dim).to(device))
                 optimizer = optim.Adam(params=scace_model.parameters(), lr=lr)
                 scace_model.mu.data.copy_(torch.Tensor(mu))
@@ -251,15 +263,15 @@
             zinb_loss = ZINB_Loss(x=raw, mean=mu, disp=disp, pi=pi, scale_factor=sf)
             kld_loss = KLD_Loss(z_mu, z_logvar)
 
             # DEC Loss
             clu_loss = Cluster_Loss(p[idx].detach(), q)
 
             # All losses
-            loss = zinb_loss + kld_w * kld_loss + clu_w * clu_loss
+            loss = zinb_loss + kld_w2 * kld_loss + clu_w * clu_loss
 
             # Optimize VAE + DEC
             optimizer.zero_grad()
             loss.backward()
             optimizer.step()
 
             # Record losses
@@ -270,27 +282,32 @@
                 avg_loss += loss.item() / n_iters
 
         if return_all:
             print(
                 'Train epoch [{}/{}]. ZINB loss:{:.4f}, kld loss:{:.4f}, cluster loss:{:.4f}, total loss:{:.4f}'.format(
                     epoch + 1, n_epochs, avg_zinb, avg_kld, avg_clu, avg_loss))
 
+
         # Update the targe distribution p
         y_pred, scace_emb, q, p = clustering(scace_model, exp_mat)
 
         if cl_type is not None:
             nmi, ari = calculate_metric(y_pred, cell_type)
             print('Clustering   %d: NMI= %.4f, ARI= %.4f, Delta=%.4f' % (
                 epoch + 1, nmi, ari, delta_label))
 
+    end = time.time()
+    run_time = end - start
+    print(f'Total time: {end - start} seconds')
+
     ############################   Return results   #########################
     adata.obsm['scace_emb'] = scace_emb
     adata.obs['scace_cluster'] = y_pred
 
     K = len(np.unique(y_pred))
 
     if return_all:
         if cl_type is not None:
-            return adata, nmi, ari, K, pred_all, emb_all
-        return adata, K, pred_all, emb_all
+            return adata, nmi, ari, K, pred_all, emb_all, run_time
+        return adata, K, pred_all, emb_all, run_time
 
     return adata
```

### Comparing `scace-0.1.0/scace/util/data_utils.py` & `scace-0.1.1/scace/util/data_utils.py`

 * *Files identical despite different names*

### Comparing `scace-0.1.0/scace/util/losses.py` & `scace-0.1.1/scace/util/losses.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 class ClusterLoss(nn.Module):
 
     def __init__(self):
         super(ClusterLoss, self).__init__()
 
     def forward(self, target, pred):
         return torch.mean(torch.sum(target * torch.log(target / (pred + 1e-6)), dim=-1))
-        # return torch.sum(target * torch.log(target / (pred + 1e-6)))
 
 
 class ELOBkldLoss(nn.Module):
     def __init__(self):
         super(ELOBkldLoss, self).__init__()
 
     def forward(self, mu, logvar):
```

### Comparing `scace-0.1.0/scace/util/tools.py` & `scace-0.1.1/scace/util/tools.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import numpy as np
 import pandas as pd
 import scanpy as sc
 import torch
 from scipy.optimize import linear_sum_assignment
 from sklearn import metrics
+from sklearn.cluster import KMeans
 
 from ..model import centroid_split
 
-
 def compute_mu(scace_emb, pred):
     mu = []
     for idx in np.unique(pred):
         mu.append(scace_emb[idx == pred, :].mean(axis=0))
 
     return np.array(mu)
 
@@ -36,36 +36,68 @@
     for i in range(y_pred.size):
         w[y_pred[i], y_true[i]] += 1
 
     row_ind, col_ind = linear_sum_assignment(w.max() - w)
     return w[row_ind, col_ind].sum() * 1.0 / y_pred.size
 
 
-def clustering(model, exp_mat, init_cluster=None, resolution=None):
+def clustering(model, exp_mat, init_cluster=None, init_method=None, resolution=None):
     model.eval()
     scace_emb = model.EncodeAll(exp_mat)
     model.train()
 
-    if resolution:
+
+    if init_method == 'kmeans':
+        scace_emb = scace_emb.cpu().numpy()
+        max_score = -1
+        k_init = 0
+        for k in range(15, 31):
+
+            kmeans = KMeans(k, n_init=50)
+            y_pred = kmeans.fit_predict(scace_emb)
+            s_score = metrics.silhouette_score(scace_emb, y_pred)
+            if s_score > max_score:
+                max_score = s_score
+                k_init = k
+
+        kmeans = KMeans(k_init, n_init=50)
+        y_pred = kmeans.fit_predict(scace_emb)
+        mu = kmeans.cluster_centers_
+        return y_pred, mu, scace_emb
+
+
+    elif init_method == 'leiden':
         adata_l = sc.AnnData(scace_emb.cpu().numpy())
         sc.pp.neighbors(adata_l, n_neighbors=10)
         sc.tl.leiden(adata_l, resolution=resolution, random_state=0)
         y_pred = np.asarray(adata_l.obs['leiden'], dtype=int)
         mu = compute_mu(scace_emb.cpu().numpy(), y_pred)
 
         return y_pred, mu, scace_emb.cpu().numpy()
 
+
+    elif init_method == 'louvain':
+        adata_l = sc.AnnData(scace_emb.cpu().numpy())
+        sc.pp.neighbors(adata_l, n_neighbors=10)
+        sc.tl.louvain(adata_l, resolution=resolution, random_state=0)
+        y_pred = np.asarray(adata_l.obs['louvain'], dtype=int)
+        mu = compute_mu(scace_emb.cpu().numpy(), y_pred)
+
+        return y_pred, mu, scace_emb.cpu().numpy()
+
+
     if init_cluster is not None:
         cluster_centers = compute_mu(scace_emb.cpu().numpy(), init_cluster)
 
         data_1 = np.concatenate([scace_emb.cpu().numpy(), np.array(init_cluster).reshape(-1, 1)], axis=1)
         mu, y_pred = centroid_split(scace_emb.cpu().numpy(), data_1, cluster_centers, np.array(init_cluster))
 
         return y_pred, mu, scace_emb.cpu().numpy()
 
+
     # Deep Embedded Clustering
     q = model.soft_assign(scace_emb)
     p = model.target_distribution(q)
 
     y_pred = torch.argmax(q, dim=1).cpu().numpy()
 
     return y_pred, scace_emb.cpu().numpy(), q, p
```

### Comparing `scace-0.1.0/scace.egg-info/PKG-INFO` & `scace-0.1.1/scace.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: scace
-Version: 0.1.0
+Version: 0.1.1
 Summary: scAce: an adaptive embedding and clustering method for single-cell gene expression data
 Home-page: https://github.com/sldyns/scAce
 Author: Kun Qian, Xinwei He
 Author-email: kun_qian@foxmail.com
 Maintainer: Kun Qian
 Maintainer-email: kun_qian@foxmail.com
 License: MIT Licence
-Description: # scAce: an adaptive embedding and clustering method
+Description: # scAce: an adaptive embedding and clustering method for scRNA-seq data
         
         ## Overview
         
         scAce is consisted of three major steps, a pre-training step based on a variational autoencoder, a cluster initialization step to obtain initial cluster labels, and an adaptive cluster merging step to iteratively
         update cluster labels and cell embeddings. In the pre-training step, scAce takes the single-cell gene expression matrix as its input to train a VAE network. For each gene, the VAE learns and outputs three parameters of a ZINB distribution (mean, dispersion, and proportion of zero). In the cluster initialization step, scAce offeres two manners. With *de novo* initialization, Leiden is used to obtain initial cluster labels; with clustering enhancement, initial cluster labels are obtained by applying a cluster splitting approach to a set of existing clustering results. In the adaptive cluster merging step,  given the pre-trained VAE network and the initial cluster labels, the network parameters, cell embeddings, cluster labels and centroids are iteratively updated by alternately performing network update and cluster merging steps. The final results of cell embeddings and cluster labels are output by scAce after the iteration process stops.
         
         ## Installation
         
-        You can install `scAce` from pypi with:
+        Please install `scAce` from pypi with:
         
         ```
         pip install scace
         ```
-        Or clone this repository and using
+        Or clone this repository and use
         
         ```
         pip install -e .
         ```
         in the root of this repository.
-        ## Usage
+        ## Quick start
         
         Load the data to be analyzed:
         
         ```
         import scanpy as sc
         
         adata = sc.AnnData(data)
@@ -51,27 +51,23 @@
         sc.pp.normalize_per_cell(adata)
         adata.obs['scale_factor'] = adata.obs.n_counts / adata.obs.n_counts.median()
         
         sc.pp.log1p(adata)
         sc.pp.scale(adata)
         ```
         
-        Run scAce algorithm:
+        Run the scAce method:
         
         ```
         from scace import run_scace
         adata = run_scace(adata)
         ```
         
-        The output adata contains cluster labels in `adata.obs['scace_cluster']` and the resulting embedding in `adata.obsm['scace_emb']`, this embedding can be used as input of other downstream task.
+        The output adata contains cluster labels in `adata.obs['scace_cluster']` and the cell embeddings in `adata.obsm['scace_emb']`. The embeddings can be used as input of other downstream analyses.
         
-        To see an example, please refer to `tutorial.ipynb`.
+        <ins>Please refer to `tutorial.ipynb` for a detailed description of scAce's usage.<ins>
         
-        ## Reproduce results
         
-        See folder `reproducibility`.
-        
-        Follow `README.md` in `data` and `pkgs` to prepare data and packages.
         
 Keywords: single-cell RNA-sequencing,clustering,cluster merging
 Platform: any
 Description-Content-Type: text/markdown
```

### Comparing `scace-0.1.0/setup.py` & `scace-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     with open(os.path.join(path, 'README.md'), "r", encoding='utf-8') as f:
         long_description = f.read()
 except Exception as e:
     long_description = "scAce: an adaptive embedding and clustering method for single-cell gene expression data"
 
 setup(
     name="scace",
-    version="0.1.0",
+    version="0.1.1",
     keywords=["single-cell RNA-sequencing", "clustering", "cluster merging"],
     description="scAce: an adaptive embedding and clustering method for single-cell gene expression data",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="MIT Licence",
 
     url="https://github.com/sldyns/scAce",
```

