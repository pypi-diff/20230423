# Comparing `tmp/scSAMP-0.1.4.tar.gz` & `tmp/scSAMP-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scSAMP-0.1.4.tar", last modified: Sat Apr 22 08:32:39 2023, max compression
+gzip compressed data, was "scSAMP-0.1.5.tar", last modified: Sun Apr 23 06:15:44 2023, max compression
```

## Comparing `scSAMP-0.1.4.tar` & `scSAMP-0.1.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 tianpei    (501) staff       (20)        0 2023-04-22 08:32:39.373021 scSAMP-0.1.4/
--rw-r--r--   0 tianpei    (501) staff       (20)     1081 2023-04-21 10:55:20.000000 scSAMP-0.1.4/LICENSE
--rw-r--r--   0 tianpei    (501) staff       (20)      658 2023-04-22 08:32:39.372763 scSAMP-0.1.4/PKG-INFO
--rw-r--r--   0 tianpei    (501) staff       (20)      423 2023-04-22 07:09:56.000000 scSAMP-0.1.4/README.md
-drwxr-xr-x   0 tianpei    (501) staff       (20)        0 2023-04-22 08:32:39.365607 scSAMP-0.1.4/docs/
--rw-r--r--   0 tianpei    (501) staff       (20)        0 2023-04-04 02:37:34.000000 scSAMP-0.1.4/docs/__init__.py
-drwxr-xr-x   0 tianpei    (501) staff       (20)        0 2023-04-22 08:32:39.367018 scSAMP-0.1.4/scSAMP/
--rw-r--r--   0 tianpei    (501) staff       (20)      346 2023-04-22 08:29:40.000000 scSAMP-0.1.4/scSAMP/__init__.py
--rw-r--r--   0 tianpei    (501) staff       (20)     1675 2023-04-04 06:15:14.000000 scSAMP-0.1.4/scSAMP/_config.py
--rw-r--r--   0 tianpei    (501) staff       (20)     1175 2023-04-22 07:01:57.000000 scSAMP-0.1.4/scSAMP/_decorator.py
--rw-r--r--   0 tianpei    (501) staff       (20)     4040 2023-04-22 07:01:57.000000 scSAMP-0.1.4/scSAMP/_utils.py
-drwxr-xr-x   0 tianpei    (501) staff       (20)        0 2023-04-22 08:32:39.369888 scSAMP-0.1.4/scSAMP/evaluation/
--rw-r--r--   0 tianpei    (501) staff       (20)        0 2023-04-22 08:27:20.000000 scSAMP-0.1.4/scSAMP/evaluation/__init__.py
--rw-r--r--   0 tianpei    (501) staff       (20)     5852 2023-04-22 07:01:57.000000 scSAMP-0.1.4/scSAMP/evaluation/_batch.py
--rw-r--r--   0 tianpei    (501) staff       (20)     1509 2023-04-22 06:18:17.000000 scSAMP-0.1.4/scSAMP/evaluation/_score.py
-drwxr-xr-x   0 tianpei    (501) staff       (20)        0 2023-04-22 08:32:39.370591 scSAMP-0.1.4/scSAMP/evaluation/model/
--rw-r--r--   0 tianpei    (501) staff       (20)        0 2023-04-22 08:29:40.000000 scSAMP-0.1.4/scSAMP/evaluation/model/__init__.py
--rw-r--r--   0 tianpei    (501) staff       (20)    13735 2023-04-22 06:18:17.000000 scSAMP-0.1.4/scSAMP/evaluation/model/_actinn.py
-drwxr-xr-x   0 tianpei    (501) staff       (20)        0 2023-04-22 08:32:39.372097 scSAMP-0.1.4/scSAMP/processing/
--rw-r--r--   0 tianpei    (501) staff       (20)        0 2023-04-22 08:27:20.000000 scSAMP-0.1.4/scSAMP/processing/__init__.py
--rw-r--r--   0 tianpei    (501) staff       (20)     1154 2023-04-04 05:32:09.000000 scSAMP-0.1.4/scSAMP/processing/_balance.py
--rw-r--r--   0 tianpei    (501) staff       (20)     3423 2023-04-04 05:27:17.000000 scSAMP-0.1.4/scSAMP/processing/_factors.py
--rw-r--r--   0 tianpei    (501) staff       (20)     7836 2023-04-22 06:18:17.000000 scSAMP-0.1.4/scSAMP/processing/_preprocessing.py
--rw-r--r--   0 tianpei    (501) staff       (20)    12469 2023-04-22 07:01:57.000000 scSAMP-0.1.4/scSAMP/processing/_sampler.py
-drwxr-xr-x   0 tianpei    (501) staff       (20)        0 2023-04-22 08:32:39.369136 scSAMP-0.1.4/scSAMP.egg-info/
--rw-r--r--   0 tianpei    (501) staff       (20)      658 2023-04-22 08:32:39.000000 scSAMP-0.1.4/scSAMP.egg-info/PKG-INFO
--rw-r--r--   0 tianpei    (501) staff       (20)      593 2023-04-22 08:32:39.000000 scSAMP-0.1.4/scSAMP.egg-info/SOURCES.txt
--rw-r--r--   0 tianpei    (501) staff       (20)        1 2023-04-22 08:32:39.000000 scSAMP-0.1.4/scSAMP.egg-info/dependency_links.txt
--rw-r--r--   0 tianpei    (501) staff       (20)       88 2023-04-22 08:32:39.000000 scSAMP-0.1.4/scSAMP.egg-info/requires.txt
--rw-r--r--   0 tianpei    (501) staff       (20)       12 2023-04-22 08:32:39.000000 scSAMP-0.1.4/scSAMP.egg-info/top_level.txt
--rw-r--r--   0 tianpei    (501) staff       (20)       38 2023-04-22 08:32:39.373106 scSAMP-0.1.4/setup.cfg
--rw-r--r--   0 tianpei    (501) staff       (20)     3878 2023-04-22 08:32:33.000000 scSAMP-0.1.4/setup.py
-drwxr-xr-x   0 tianpei    (501) staff       (20)        0 2023-04-22 08:32:39.372430 scSAMP-0.1.4/test/
--rw-r--r--   0 tianpei    (501) staff       (20)      117 2023-04-22 08:07:35.000000 scSAMP-0.1.4/test/test.py
+drwxr-xr-x   0 tianpei    (501) staff       (20)        0 2023-04-23 06:15:44.213048 scSAMP-0.1.5/
+-rw-r--r--   0 tianpei    (501) staff       (20)     1081 2023-04-21 10:55:20.000000 scSAMP-0.1.5/LICENSE
+-rw-r--r--   0 tianpei    (501) staff       (20)      658 2023-04-23 06:15:44.212606 scSAMP-0.1.5/PKG-INFO
+-rw-r--r--   0 tianpei    (501) staff       (20)      426 2023-04-22 08:39:32.000000 scSAMP-0.1.5/README.md
+drwxr-xr-x   0 tianpei    (501) staff       (20)        0 2023-04-23 06:15:44.202132 scSAMP-0.1.5/docs/
+-rw-r--r--   0 tianpei    (501) staff       (20)        0 2023-04-04 02:37:34.000000 scSAMP-0.1.5/docs/__init__.py
+drwxr-xr-x   0 tianpei    (501) staff       (20)        0 2023-04-23 06:15:44.203787 scSAMP-0.1.5/scSAMP/
+-rw-r--r--   0 tianpei    (501) staff       (20)      423 2023-04-23 06:11:25.000000 scSAMP-0.1.5/scSAMP/__init__.py
+-rw-r--r--   0 tianpei    (501) staff       (20)     1740 2023-04-22 16:24:40.000000 scSAMP-0.1.5/scSAMP/_config.py
+-rw-r--r--   0 tianpei    (501) staff       (20)     1175 2023-04-22 07:01:57.000000 scSAMP-0.1.5/scSAMP/_decorator.py
+-rw-r--r--   0 tianpei    (501) staff       (20)     4066 2023-04-23 03:00:12.000000 scSAMP-0.1.5/scSAMP/_utils.py
+drwxr-xr-x   0 tianpei    (501) staff       (20)        0 2023-04-23 06:15:44.207601 scSAMP-0.1.5/scSAMP/evaluation/
+-rw-r--r--   0 tianpei    (501) staff       (20)        0 2023-04-22 08:27:20.000000 scSAMP-0.1.5/scSAMP/evaluation/__init__.py
+-rw-r--r--   0 tianpei    (501) staff       (20)     6096 2023-04-23 06:02:51.000000 scSAMP-0.1.5/scSAMP/evaluation/_batch.py
+-rw-r--r--   0 tianpei    (501) staff       (20)     1509 2023-04-22 06:18:17.000000 scSAMP-0.1.5/scSAMP/evaluation/_score.py
+drwxr-xr-x   0 tianpei    (501) staff       (20)        0 2023-04-23 06:15:44.208489 scSAMP-0.1.5/scSAMP/evaluation/model/
+-rw-r--r--   0 tianpei    (501) staff       (20)        0 2023-04-22 08:29:40.000000 scSAMP-0.1.5/scSAMP/evaluation/model/__init__.py
+-rw-r--r--   0 tianpei    (501) staff       (20)    13735 2023-04-22 06:18:17.000000 scSAMP-0.1.5/scSAMP/evaluation/model/_actinn.py
+drwxr-xr-x   0 tianpei    (501) staff       (20)        0 2023-04-23 06:15:44.211099 scSAMP-0.1.5/scSAMP/processing/
+-rw-r--r--   0 tianpei    (501) staff       (20)        0 2023-04-22 08:27:20.000000 scSAMP-0.1.5/scSAMP/processing/__init__.py
+-rw-r--r--   0 tianpei    (501) staff       (20)     1154 2023-04-04 05:32:09.000000 scSAMP-0.1.5/scSAMP/processing/_balance.py
+-rw-r--r--   0 tianpei    (501) staff       (20)     3423 2023-04-04 05:27:17.000000 scSAMP-0.1.5/scSAMP/processing/_factors.py
+-rw-r--r--   0 tianpei    (501) staff       (20)     9363 2023-04-23 05:34:31.000000 scSAMP-0.1.5/scSAMP/processing/_preprocessing.py
+-rw-r--r--   0 tianpei    (501) staff       (20)    14000 2023-04-23 05:22:14.000000 scSAMP-0.1.5/scSAMP/processing/_sampler.py
+drwxr-xr-x   0 tianpei    (501) staff       (20)        0 2023-04-23 06:15:44.206272 scSAMP-0.1.5/scSAMP.egg-info/
+-rw-r--r--   0 tianpei    (501) staff       (20)      658 2023-04-23 06:15:44.000000 scSAMP-0.1.5/scSAMP.egg-info/PKG-INFO
+-rw-r--r--   0 tianpei    (501) staff       (20)      593 2023-04-23 06:15:44.000000 scSAMP-0.1.5/scSAMP.egg-info/SOURCES.txt
+-rw-r--r--   0 tianpei    (501) staff       (20)        1 2023-04-23 06:15:44.000000 scSAMP-0.1.5/scSAMP.egg-info/dependency_links.txt
+-rw-r--r--   0 tianpei    (501) staff       (20)       88 2023-04-23 06:15:44.000000 scSAMP-0.1.5/scSAMP.egg-info/requires.txt
+-rw-r--r--   0 tianpei    (501) staff       (20)       12 2023-04-23 06:15:44.000000 scSAMP-0.1.5/scSAMP.egg-info/top_level.txt
+-rw-r--r--   0 tianpei    (501) staff       (20)       38 2023-04-23 06:15:44.213191 scSAMP-0.1.5/setup.cfg
+-rw-r--r--   0 tianpei    (501) staff       (20)     3878 2023-04-23 06:12:39.000000 scSAMP-0.1.5/setup.py
+drwxr-xr-x   0 tianpei    (501) staff       (20)        0 2023-04-23 06:15:44.211627 scSAMP-0.1.5/test/
+-rw-r--r--   0 tianpei    (501) staff       (20)      117 2023-04-22 08:07:35.000000 scSAMP-0.1.5/test/test.py
```

### Comparing `scSAMP-0.1.4/LICENSE` & `scSAMP-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scSAMP-0.1.4/PKG-INFO` & `scSAMP-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scSAMP
-Version: 0.1.4
+Version: 0.1.5
 Summary: scRNA-seq data sampling toolkit.
 Home-page: https://github.com/Tptrix29/scSAMP
 Author: Pei Tian
 Author-email: 1953776@tongji.edu.cn
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `scSAMP-0.1.4/scSAMP/_config.py` & `scSAMP-0.1.5/scSAMP/_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 
 
 class SamplingStrategy(Enum):
     """
     Sample strategy collection.
 
     :Options:
+        - ``random``: Random sampling
         - ``stratify``: Classical stratified sampling
         - ``balance``: Stratified sampling with balanced ratio
         - ``compactness``: Adjusted sampling with intra-cluster compactness factor
         - ``complexity``: Adjusted sampling with inter-cluster complexity factor
         - ``concave``: Adjusted sampling with concave integration of compactness factor and complexity factor
         - ``convex``: Adjusted sampling with convex integration of compactness factor and complexity factor
         - ``entropy``: Adjusted sampling with entropy weight integration of compactness factor and complexity factor
 
     Notes
     -----
 
 
     """
+    RANDOM: str = "random"
     STRATIFY: str = "stratify"
     BALANCE: str = "balance"
     COMPACTNESS: str = "compactness"
     COMPLEXITY: str = "complexity"
     CONCAVE: str = "concave"
     CONVEX: str = "convex"
     ENTROPY: str = "entropy"
```

### Comparing `scSAMP-0.1.4/scSAMP/_decorator.py` & `scSAMP-0.1.5/scSAMP/_decorator.py`

 * *Files identical despite different names*

### Comparing `scSAMP-0.1.4/scSAMP/_utils.py` & `scSAMP-0.1.5/scSAMP/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,17 +108,17 @@
 
     if isinstance(source_file, str):
         source_file = [source_file]
     for file in source_file:
         re_file = result_dir + file.split('/')[-1].split('.')[0] + '.h5ad'
         print(f'Loading Data from {file}...')
         if source_format == 'csv':
-            data = pd.read_csv(file, header=0)
+            data = pd.read_csv(file, header=0, index_col=0)
         elif source_format == 'tab':
-            data = pd.read_table(file, header=0)
+            data = pd.read_table(file, header=0, index_col=0)
         else:
             raise ValueError('Invalid source file format.')
         print(f'Data Loaded from {file}.')
         data.index = [str(i) for i in data.index]
         cell_type = data[type_label]
         data.drop(columns=[type_label], inplace=True)
         adata = AnnData(data, dtype=np.float64)
```

### Comparing `scSAMP-0.1.4/scSAMP/evaluation/_batch.py` & `scSAMP-0.1.5/scSAMP/evaluation/_batch.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,41 +48,45 @@
         self.total_iter = self.ratio_range.shape[0] * len(SamplingStrategy)
 
         self.sampler: SamplingProcessor = SamplingProcessor(reference=ref, cluster_col=col, ratio=1)
 
     def eval(
             self,
             classifier: str,
+            sampling_strategy_collection: Optional[list] = None,
             **kwargs
     ) -> None:
         """
         Evaluation with certain classifier.
 
         Parameters
         ----------
-        classifier :class:`scSAMP.config.EvaluationStrategy`
+        classifier: :class:`scSAMP.EvaluationStrategy`
             classification model name
+        sampling_strategy_collection: list
+            choose specific sampling strategies
 
         Returns
         -------
 
         """
         _check_obs_key(self.query, self.pred_col)
 
         if classifier not in [val for val in EvaluationStrategy]:
             raise(ValueError(f"Invalid Evaluation Strategy '{classifier}'."))
 
+        if not sampling_strategy_collection:
+            sampling_strategy_collection = [str(s) for s in SamplingStrategy]
         X_test = self.query.X
         y_test = self.query.obs[self.pred_col]
         i = 1
         for r in self.ratio_range:
-            for sampling in SamplingStrategy:
+            for sampling in sampling_strategy_collection:
                 print(f"{i} / {self.total_iter} ----------------------------------")
                 i += 1
-                sampling = str(sampling)
                 self.sampler._reset_ratio(r)
                 self.train = self.sampler.sampling(strategy=sampling)
                 X_train = self.train.X
                 y_train = self.train.obs[self.pred_col]
 
                 # Evaluation
                 if classifier == EvaluationStrategy.SVM:
```

### Comparing `scSAMP-0.1.4/scSAMP/evaluation/_score.py` & `scSAMP-0.1.5/scSAMP/evaluation/_score.py`

 * *Files identical despite different names*

### Comparing `scSAMP-0.1.4/scSAMP/evaluation/model/_actinn.py` & `scSAMP-0.1.5/scSAMP/evaluation/model/_actinn.py`

 * *Files identical despite different names*

### Comparing `scSAMP-0.1.4/scSAMP/processing/_balance.py` & `scSAMP-0.1.5/scSAMP/processing/_balance.py`

 * *Files identical despite different names*

### Comparing `scSAMP-0.1.4/scSAMP/processing/_factors.py` & `scSAMP-0.1.5/scSAMP/processing/_factors.py`

 * *Files identical despite different names*

### Comparing `scSAMP-0.1.4/scSAMP/processing/_preprocessing.py` & `scSAMP-0.1.5/scSAMP/processing/_preprocessing.py`

 * *Files 13% similar despite different names*

```diff
@@ -61,29 +61,29 @@
         Returns
         -------
         Preprocessed reference dataset
         """
         pass
 
     @abstractmethod
-    def queryPreprocessor(self, query: AnnData) -> AnnData:
+    def queryPreprocessor(self, ref: AnnData, query: AnnData) -> tuple[AnnData, AnnData]:
         """
         Preprocessing query dataset.
 
         Parameters
         ----------
         query :class:`anndata.AnnData`
             query dataset
         Returns
         -------
         Preprocessed query dataset
         """
         pass
 
-    def basicProcessing(self, adata) -> None:
+    def basicProcessing(self, adata: AnnData) -> None:
         """
         Basic Preprocessing
 
         Parameters
         ----------
         adata :class:`anndata.AnnData`
             reference data
@@ -92,25 +92,65 @@
         -------
 
         """
         sc.pp.filter_cells(adata, min_genes=self.basic_params['genes_threshold'])
         sc.pp.normalize_total(adata, target_sum=self.basic_params['target_threshold'])
         sc.pp.log1p(adata)
 
+    def normalize(self, adata: AnnData):
+        sc.pp.filter_cells(adata, min_genes=self.basic_params['genes_threshold'])
+        sc.pp.normalize_total(adata, target_sum=self.basic_params['target_threshold'])
+
     def test_prior(self) -> None:
         """
         Ensure the reference dataset is preprocessed.
 
         Returns
         -------
 
         """
         if not self.is_prior:
             raise (ValueError("Use 'refPreprocessing' to get index first."))
 
+    def feature_intersection(
+            self, ref: AnnData, query: AnnData
+    ) -> tuple[AnnData, AnnData]:
+        intersections: pd.Index = pd.Index(set(self.gene_index).intersection(set(query.var.index)))
+        print(f"There are {len(self.gene_index) - len(intersections)} gene(s) only exist in reference dataset. "
+              f"(Filter out)")
+        return ref[:, intersections], query[:, intersections]
+
+
+class NormalizationPreprocessor(BasePreprocessor):
+    """
+    Normalization preprocessor.
+
+    Steps:
+    1. Filter cells
+    2. Normalization
+    """
+    def __init__(self):
+        super().__init__()
+
+    def display_params(self):
+        super().display_params()
+
+    def refPreprocessing(self, ref: AnnData) -> AnnData:
+        super().normalize(adata=ref)
+        self.gene_index = ref.var_names
+        self.is_prior = True
+        return ref
+
+    def queryPreprocessor(self, ref: AnnData, query: AnnData) -> tuple[AnnData, AnnData]:
+        super().test_prior()
+        ref, query = super().feature_intersection(ref, query)
+        super().normalize(adata=query)
+        sc.pp.scale(query, max_value=self.basic_params['max_threshold'])
+        return ref, query
+
 
 class BasicPreprocessor(BasePreprocessor):
     """
     Basic preprocessing class.
 
     Attributes
     ------------
@@ -142,20 +182,20 @@
         sc.pp.filter_genes(ref, min_cells=self.basic_params['cells_threshold'])
         super().basicProcessing(adata=ref)
         sc.pp.scale(ref, max_value=self.basic_params['max_threshold'])
         self.gene_index = ref.var_names
         self.is_prior = True
         return ref
 
-    def queryPreprocessor(self, query: AnnData) -> AnnData:
+    def queryPreprocessor(self, ref: AnnData, query: AnnData) -> tuple[AnnData, AnnData]:
         super().test_prior()
-        new_query = query[:, self.gene_index]
-        super().basicProcessing(adata=new_query)
-        sc.pp.scale(new_query, max_value=self.basic_params['max_threshold'])
-        return new_query
+        ref, query = super().feature_intersection(ref, query)
+        super().basicProcessing(adata=query)
+        sc.pp.scale(query, max_value=self.basic_params['max_threshold'])
+        return ref, query
 
 
 class HVGPreprocessor(BasePreprocessor):
     """
     Preprocessing class for HVG (Highly Variable Gene) selection.
     Attributes
     ------------
@@ -196,20 +236,20 @@
         sc.pp.highly_variable_genes(ref, n_top_genes=self.n_hvg, inplace=True)
         self.gene_index = ref.var[ref.var['highly_variable']].index
         self.is_prior = True
         ref = ref[:, self.gene_index]
         sc.pp.scale(ref, max_value=self.basic_params['max_threshold'])
         return ref
 
-    def queryPreprocessor(self, query: AnnData) -> AnnData:
+    def queryPreprocessor(self, ref: AnnData, query: AnnData) -> tuple[AnnData, AnnData]:
         super().test_prior()
         super().basicProcessing(adata=query)
-        new_query = query[:, self.gene_index]
-        sc.pp.scale(new_query, max_value=self.basic_params['max_threshold'])
-        return new_query
+        ref, query = super().feature_intersection(ref, query)
+        sc.pp.scale(query, max_value=self.basic_params['max_threshold'])
+        return ref, query
 
 
 class PCAPreprocessor(BasePreprocessor):
     """
     Preprocessing class for PCA (Principle Components Analysis).
 
     Attributes
@@ -258,26 +298,29 @@
 
     def refPreprocessing(self, ref: AnnData) -> AnnData:
         super().basicProcessing(adata=ref)
         sc.pp.highly_variable_genes(ref, n_top_genes=self.n_hvg, inplace=True)
         self.gene_index = ref.var[ref.var['highly_variable']].index
         ref = ref[:, self.gene_index]
         sc.pp.scale(ref, max_value=self.basic_params['max_threshold'])
-        sc.tl.pca(ref, svd_solver='arpack')
         self.is_prior = True
-        self.trans_matrix = ref.varm["PCs"][:, :self.n_pc]
-        new_ref = ref[:, :self.n_pc]
-        new_ref.var.index = ["PC" + str(i+1) for i in range(self.n_pc)]
-        new_ref.X = ref.obsm["X_pca"][:, :self.n_pc]
-        return new_ref
+        return ref
 
-    def queryPreprocessor(self, query: AnnData) -> AnnData:
+    def queryPreprocessor(self, ref: AnnData, query: AnnData) -> tuple[AnnData, AnnData]:
         super().test_prior()
         super().basicProcessing(adata=query)
-        new_query = query[:, self.gene_index]
-        sc.pp.scale(new_query, max_value=self.basic_params['max_threshold'])
-        target_query = new_query[:, :self.n_pc]
-        target_query.var.index = ["PC" + str(i+1) for i in range(self.n_pc)]
-        target_query.X = new_query.X.dot(self.trans_matrix)
-        return target_query
+        ref, query = super().feature_intersection(ref, query)
+        sc.pp.scale(query, max_value=self.basic_params['max_threshold'])
+
+        sc.tl.pca(ref, svd_solver='arpack')
+        self.trans_matrix = ref.varm["PCs"][:, :self.n_pc]
+        ref = self.pc_transform(ref)
+        query = self.pc_transform(query)
+        return ref, query
+
+    def pc_transform(self, adata: AnnData) -> AnnData:
+        target = adata[:, :self.n_pc]
+        target.var.index = ["PC" + str(i+1) for i in range(self.n_pc)]
+        target.X = adata.X.dot(self.trans_matrix)
+        return target
```

### Comparing `scSAMP-0.1.4/scSAMP/processing/_sampler.py` & `scSAMP-0.1.5/scSAMP/processing/_sampler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import pandas as pd
 import anndata as ad
 from anndata import AnnData
-from typing import Optional
+from typing import Optional, Union
 from imblearn.over_sampling import SMOTE
 
 from .._utils import settings, _check_obs_key, _check_ratio
 from ..processing._balance import balance_power
 from ..processing import _factors as fc
 from .._config import SamplingStrategy
 from .._decorator import time_logging
@@ -30,14 +30,16 @@
         Sampling selection label of specific method and ratio (latest applied).
     oversampling_dataset: :class:`anndata.AnnData`
         Oversampling dataset, generated by :class:`imblearn.over_sampling.SMOTE`
     metadata: :class:`pandas.DataFrame`
         Metadata of cluster-specific factors.
     random_state: int
         Random state.
+    FORCE: boolean
+        Force oversampling neighbor to be minmum cluster size - 1 (> 1).
 
     Notes
     -----
     This is a beta version. ()
 
     Examples
     --------
@@ -56,14 +58,15 @@
     ):
         if ratio:
             _check_ratio(ratio)
         self.sampling_ratio: Optional[float] = ratio
         self.reference: AnnData = reference
         self.cluster_label: str = cluster_col
         self.random_state: int = random_state
+        self.FORCE: bool = False
 
         self.raw_count: int = self.reference.obs.shape[0]
 
         self.latest_label: str = 'NoSampling'
         self.oversampling_dataset: Optional[AnnData] = None
 
         # change index
@@ -79,14 +82,17 @@
             raise ValueError("Choose 1 parameter to define sampling size.")
         if ratio:
             _check_ratio(ratio)
             self._reset_ratio(ratio)
         if n and n > 0:
             self._reset_ratio(n / self.raw_count)
 
+    def set_FORCE(self, force):
+        self.FORCE = force
+
     def sampling(
             self,
             strategy: str,
     ) -> AnnData:
         """
         Sampling function with strategy parameter.
 
@@ -105,15 +111,17 @@
             raise(ValueError(f"Invalid Sampling Strategy '{strategy}'."))
 
         if self.latest_label:
             if self.oversampling_dataset:
                 self.oversampling_dataset.obs[self.latest_label] = False
         self.latest_label = self.cluster_label + '_' + strategy
 
-        if strategy == SamplingStrategy.STRATIFY or self.sampling_ratio >= 0.5:
+        if strategy == SamplingStrategy.RANDOM:
+            return self._random_sampling()
+        elif strategy == SamplingStrategy.STRATIFY or self.sampling_ratio >= 0.5:
             return self._stratify()
         if strategy == SamplingStrategy.BALANCE:
             return self._imbalance_sampling(balance_power(self.metadata['ratio']))
         else:
             self._check_factor(strategy)
             return self._imbalance_sampling(self.metadata[strategy+'_balanced'])
 
@@ -142,25 +150,25 @@
         return part1
 
     def generate_factors(self) -> None:
         """
         Generate cluster-specific factors.
         """
         for s in SamplingStrategy:
-            if s != SamplingStrategy.BALANCE and s != SamplingStrategy.STRATIFY:
+            if s != SamplingStrategy.BALANCE and s != SamplingStrategy.STRATIFY and s != SamplingStrategy.RANDOM:
                 self._check_factor(str(s))
 
     def _check_factor(self, factor_type: str) -> None:
         """
         Optimize generation of specific factor.
 
         Parameters
         ----------
         factor_type
-            Type of factor chosen from :class:`scSAMP.config.SamplingStrategy`
+            Type of factor chosen from :class:`scSAMP.SamplingStrategy`
         """
         factor_type = str(factor_type)
         if factor_type not in self.metadata.columns:
             if factor_type == SamplingStrategy.COMPACTNESS:
                 _, self.metadata[str(SamplingStrategy.COMPACTNESS)] = \
                     fc.compactness_factor(self.reference.obs, self.reference.X, self.cluster_label)
             elif factor_type == SamplingStrategy.COMPLEXITY:
@@ -179,31 +187,57 @@
                         self.metadata[str(SamplingStrategy.COMPLEXITY)])
                 elif factor_type == SamplingStrategy.ENTROPY:
                     self.metadata[str(SamplingStrategy.ENTROPY)] = fc.entropy_2var(
                         self.metadata[str(SamplingStrategy.COMPACTNESS)],
                         self.metadata[str(SamplingStrategy.COMPLEXITY)])
             self.metadata[factor_type + '_balanced'] = balance_power(self.metadata[factor_type])
 
+    def _check_sample_size(self):
+        minmum = min(self.metadata["count"])
+        if minmum == 1:
+            raise ValueError(f"Cluster with one sample exists in dataset, can't apply oversampling.")
+        if minmum <= 5:
+            if not self.FORCE:
+                raise ValueError(f"Some cluster's size is too small, oversampling is not recommended. "
+                                 f"Use 'SamplingProcessor.set_FORCE(True)' to apply oversampling")
+            else:
+                print(f"Some cluster's size is too small, "
+                      f"oversampling is not recommended but forced to be run.")
+
     @time_logging(mode="oversampling")
     def _generate_oversampling(self) -> None:
         """
         Generate oversampling dataset by SMOTE.
 
         SMOTE is the most stable oversampling method (Generate fully-balanced dataset)
         """
-        X_resampled, y_resampled = SMOTE(random_state=self.random_state) \
+        self._check_sample_size()
+        k: int = 5
+        if self.FORCE:
+            k = int(min(k, min(self.metadata["count"]-1)))
+        X_resampled, y_resampled = SMOTE(random_state=self.random_state, k_neighbors=k) \
             .fit_resample(self.reference.X, self.reference.obs[self.cluster_label])
         X_resampled, y_resampled = X_resampled[self.raw_count:, :], y_resampled[self.raw_count:]
         print(y_resampled.shape[0])
         self.oversampling_dataset = AnnData(X=X_resampled,
                                             obs=pd.DataFrame({
                                                 self.cluster_label: y_resampled,
                                                 self.latest_label: True,
                                             }))
 
+    def _random_sampling(self) -> AnnData:
+        """ Random sampling method. """
+        ind = self.reference.obs.sample(frac=self.sampling_ratio).index
+
+        self.reference.obs[self.latest_label] = self.reference.obs.index
+        self.reference.obs[self.latest_label] = pd.Categorical(self.reference.obs.apply(
+            lambda x: True if x[self.latest_label] in ind else False, axis=1
+        ))
+        return self.get_target_dataset()
+
     def _stratify(self) -> AnnData:
         """ Classical stratified sampling method. """
         ind = pd.DataFrame(self.reference.obs[self.cluster_label])\
             .groupby(self.cluster_label).apply(
                 lambda x: x.sample(frac=self.sampling_ratio,
                                    random_state=self.random_state)
             ).index.droplevel(0)
```

### Comparing `scSAMP-0.1.4/scSAMP.egg-info/PKG-INFO` & `scSAMP-0.1.5/scSAMP.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scSAMP
-Version: 0.1.4
+Version: 0.1.5
 Summary: scRNA-seq data sampling toolkit.
 Home-page: https://github.com/Tptrix29/scSAMP
 Author: Pei Tian
 Author-email: 1953776@tongji.edu.cn
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `scSAMP-0.1.4/scSAMP.egg-info/SOURCES.txt` & `scSAMP-0.1.5/scSAMP.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scSAMP-0.1.4/setup.py` & `scSAMP-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'scSAMP'
 DESCRIPTION = 'scRNA-seq data sampling toolkit.'
 URL = 'https://github.com/Tptrix29/scSAMP'
 EMAIL = '1953776@tongji.edu.cn'
 AUTHOR = 'Pei Tian'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.4'
+VERSION = '0.1.5'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "numpy", "pandas", "matplotlib", "scikit-learn",
     "pyreadr", "anndata", "tensorflow", "imbalanced-learn", "scanpy"
 ]
```

