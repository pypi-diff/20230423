# Comparing `tmp/forust-0.2.1.tar.gz` & `tmp/forust-0.2.2.tar.gz`

## Comparing `forust-0.2.1.tar` & `forust-0.2.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 forust-0.2.1/local_dependencies/forust-ml/Cargo.toml
--rw-r--r--   0      501       20     5608 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/.github/workflows/CI.yml
--rw-r--r--   0      501       20      262 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/.gitignore
--rw-r--r--   0      501       20      320 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/.pre-commit-config.yaml
--rw-r--r--   0      501       20    11341 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/LICENSE
--rw-r--r--   0      501       20    10881 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/README.md
--rw-r--r--   0      501       20     3857 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/benches/forust_benchmarks.rs
--rw-r--r--   0      501       20   396909 2023-04-23 02:43:43.000000 forust-0.2.1/local_dependencies/forust-ml/dist/forust-0.2.1-cp311-cp311-macosx_10_7_x86_64.whl
--rw-r--r--   0      501       20   745373 2023-04-23 02:42:47.000000 forust-0.2.1/local_dependencies/forust-ml/dist/forust-0.2.1.tar.gz
--rw-r--r--   0      501       20    16121 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/resources/pdp_plot_age.png
--rw-r--r--   0      501       20    10758 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png
--rw-r--r--   0      501       20    57018 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/resources/titanic.csv
--rw-r--r--   0      501       20   655700 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/resources/tree-image-crop.png
--rw-r--r--   0      501       20     2556 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/rs-example.md
--rw-r--r--   0      501       20     1179 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/scripts/make_resources.py
--rw-r--r--   0      501       20       53 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/scripts/run-python-tests.ps1
--rw-r--r--   0      501       20       53 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/scripts/run-python-tests.sh
--rw-r--r--   0      501       20     5456 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/src/binning.rs
--rw-r--r--   0      501       20      248 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/src/constraints.rs
--rw-r--r--   0      501       20     7678 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/src/data.rs
--rw-r--r--   0      501       20      473 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/src/errors.rs
--rw-r--r--   0      501       20    17082 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/src/gradientbooster.rs
--rw-r--r--   0      501       20     8639 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/src/histogram.rs
--rw-r--r--   0      501       20      318 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/src/lib.rs
--rw-r--r--   0      501       20     5901 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/src/node.rs
--rw-r--r--   0      501       20     4125 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/src/objective.rs
--rw-r--r--   0      501       20     3146 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/src/partial_dependence.rs
--rw-r--r--   0      501       20    27105 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/src/splitter.rs
--rw-r--r--   0      501       20    13817 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/src/tree.rs
--rw-r--r--   0      501       20    28561 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/src/utils.rs
--rw-r--r--   0        0        0      391 1970-01-01 00:00:00.000000 forust-0.2.1/Cargo.toml
--rw-r--r--   0      501       20      685 2023-04-23 02:39:52.000000 forust-0.2.1/.gitignore
--rw-r--r--   0      501       20    10881 2023-04-23 02:40:40.000000 forust-0.2.1/README.md
--rw-r--r--   0      501       20    15483 2023-04-23 02:39:52.000000 forust-0.2.1/forust/__init__.py
--rw-r--r--   0      501       20      785 2023-04-23 02:39:52.000000 forust-0.2.1/pyproject.toml
--rw-r--r--   0      501       20     7353 2023-04-23 02:39:52.000000 forust-0.2.1/scratch.py
--rw-r--r--   0      501       20     8439 2023-04-23 02:39:52.000000 forust-0.2.1/src/lib.rs
--rw-r--r--   0      501       20     7940 2023-04-23 02:39:52.000000 forust-0.2.1/tests/test_booster.py
--rw-r--r--   0      501       20    11341 2023-04-23 02:40:40.000000 forust-0.2.1/LICENSE
--rw-r--r--   0      501       20    10881 2023-04-23 02:40:40.000000 forust-0.2.1/README.md
--rw-r--r--   0        0        0    11665 1970-01-01 00:00:00.000000 forust-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 forust-0.2.2/local_dependencies/forust-ml/Cargo.toml
+-rw-r--r--   0      501       20     5608 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      262 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/.gitignore
+-rw-r--r--   0      501       20      320 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/.pre-commit-config.yaml
+-rw-r--r--   0      501       20    11341 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/LICENSE
+-rw-r--r--   0      501       20    10881 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/README.md
+-rw-r--r--   0      501       20     3857 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/benches/forust_benchmarks.rs
+-rw-r--r--   0      501       20   397862 2023-04-23 21:38:22.000000 forust-0.2.2/local_dependencies/forust-ml/dist/forust-0.2.2-cp311-cp311-macosx_10_7_x86_64.whl
+-rw-r--r--   0      501       20   746003 2023-04-23 21:37:25.000000 forust-0.2.2/local_dependencies/forust-ml/dist/forust-0.2.2.tar.gz
+-rw-r--r--   0      501       20    16121 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/resources/pdp_plot_age.png
+-rw-r--r--   0      501       20    10758 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png
+-rw-r--r--   0      501       20    57018 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/resources/titanic.csv
+-rw-r--r--   0      501       20   655700 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/resources/tree-image-crop.png
+-rw-r--r--   0      501       20     2556 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/rs-example.md
+-rw-r--r--   0      501       20     1179 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/scripts/make_resources.py
+-rw-r--r--   0      501       20       53 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/scripts/run-python-tests.ps1
+-rw-r--r--   0      501       20       53 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/scripts/run-python-tests.sh
+-rw-r--r--   0      501       20     5456 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/src/binning.rs
+-rw-r--r--   0      501       20      248 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/src/constraints.rs
+-rw-r--r--   0      501       20     8384 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/src/data.rs
+-rw-r--r--   0      501       20      473 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/src/errors.rs
+-rw-r--r--   0      501       20    19236 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/src/gradientbooster.rs
+-rw-r--r--   0      501       20     8639 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/src/histogram.rs
+-rw-r--r--   0      501       20      318 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/src/lib.rs
+-rw-r--r--   0      501       20     5901 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/src/node.rs
+-rw-r--r--   0      501       20     4125 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/src/objective.rs
+-rw-r--r--   0      501       20     3146 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/src/partial_dependence.rs
+-rw-r--r--   0      501       20    27105 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/src/splitter.rs
+-rw-r--r--   0      501       20    14132 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/src/tree.rs
+-rw-r--r--   0      501       20    28561 2023-04-23 21:34:32.000000 forust-0.2.2/local_dependencies/forust-ml/src/utils.rs
+-rw-r--r--   0        0        0      391 1970-01-01 00:00:00.000000 forust-0.2.2/Cargo.toml
+-rw-r--r--   0      501       20      685 2023-04-23 21:34:32.000000 forust-0.2.2/.gitignore
+-rw-r--r--   0      501       20    10881 2023-04-23 21:35:16.000000 forust-0.2.2/README.md
+-rw-r--r--   0      501       20    15483 2023-04-23 21:34:32.000000 forust-0.2.2/forust/__init__.py
+-rw-r--r--   0      501       20      785 2023-04-23 21:34:32.000000 forust-0.2.2/pyproject.toml
+-rw-r--r--   0      501       20     7353 2023-04-23 21:34:32.000000 forust-0.2.2/scratch.py
+-rw-r--r--   0      501       20     8439 2023-04-23 21:34:32.000000 forust-0.2.2/src/lib.rs
+-rw-r--r--   0      501       20     7940 2023-04-23 21:34:32.000000 forust-0.2.2/tests/test_booster.py
+-rw-r--r--   0      501       20    11341 2023-04-23 21:35:16.000000 forust-0.2.2/LICENSE
+-rw-r--r--   0      501       20    10881 2023-04-23 21:35:16.000000 forust-0.2.2/README.md
+-rw-r--r--   0        0        0    11665 1970-01-01 00:00:00.000000 forust-0.2.2/PKG-INFO
```

### Comparing `forust-0.2.1/local_dependencies/forust-ml/Cargo.toml` & `forust-0.2.2/local_dependencies/forust-ml/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "forust-ml"
-version = "0.2.1"
+version = "0.2.2"
 edition = "2021"
 authors = ["James Inlow <james.d.inlow@gmail.com>"]
 homepage = "https://github.com/jinlow/forust"
 description = "A lightweight gradient boosting implementation in Rust."
 license-file = "LICENSE"
 readme = "README.md"
 repository = "https://github.com/jinlow/forust"
```

### Comparing `forust-0.2.1/local_dependencies/forust-ml/.github/workflows/CI.yml` & `forust-0.2.2/local_dependencies/forust-ml/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `forust-0.2.1/local_dependencies/forust-ml/LICENSE` & `forust-0.2.2/local_dependencies/forust-ml/LICENSE`

 * *Files identical despite different names*

### Comparing `forust-0.2.1/local_dependencies/forust-ml/README.md` & `forust-0.2.2/local_dependencies/forust-ml/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 The package can be installed directly from [pypi](https://pypi.org/project/forust/).
 ```shell
 pip install forust
 ```
 
 To use in a rust project add the following to your Cargo.toml file.
 ```toml
-forust-ml = "0.2.1"
+forust-ml = "0.2.2"
 ```
 
 ## Usage
 The `GradientBooster` class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
 
 It can be initialized with the following arguments.
```

#### html2text {}

```diff
@@ -13,15 +13,15 @@
 understand the XGBoost algorithm, additionally to have a fun project to work on
 in rust, and because I wanted to be able to experiment with adding new features
 to the algorithm in a smaller simpler codebase. All of the rust code for the
 package can be found in the [src](src/) directory, while all of the python
 wrapper code is in the [py-forust](py-forust/) directory. ## Installation The
 package can be installed directly from [pypi](https://pypi.org/project/forust/
 ). ```shell pip install forust ``` To use in a rust project add the following
-to your Cargo.toml file. ```toml forust-ml = "0.2.1" ``` ## Usage The
+to your Cargo.toml file. ```toml forust-ml = "0.2.2" ``` ## Usage The
 `GradientBooster` class is currently the only public facing class in the
 package, and can be used to train gradient boosted decision tree ensembles with
 multiple objective functions. It can be initialized with the following
 arguments. - `objective_type` ***(str, optional)***: The name of objective
 function used to optimize. Valid options include "LogLoss" to use logistic loss
 as the objective function (binary classification), or "SquaredLoss" to use
 Squared Error as the objective function (continuous regression). Defaults to
```

### Comparing `forust-0.2.1/local_dependencies/forust-ml/benches/forust_benchmarks.rs` & `forust-0.2.2/local_dependencies/forust-ml/benches/forust_benchmarks.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.1/local_dependencies/forust-ml/resources/pdp_plot_age.png` & `forust-0.2.2/local_dependencies/forust-ml/resources/pdp_plot_age.png`

 * *Files identical despite different names*

### Comparing `forust-0.2.1/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png` & `forust-0.2.2/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png`

 * *Files identical despite different names*

### Comparing `forust-0.2.1/local_dependencies/forust-ml/resources/titanic.csv` & `forust-0.2.2/local_dependencies/forust-ml/resources/titanic.csv`

 * *Files identical despite different names*

### Comparing `forust-0.2.1/local_dependencies/forust-ml/resources/tree-image-crop.png` & `forust-0.2.2/local_dependencies/forust-ml/resources/tree-image-crop.png`

 * *Files identical despite different names*

### Comparing `forust-0.2.1/local_dependencies/forust-ml/rs-example.md` & `forust-0.2.2/local_dependencies/forust-ml/rs-example.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ## A Complete Rust Example
 
 To run this example, add the following code to your `Cargo.toml` file.
 ```toml
 [dependencies]
-forust-ml = "0.2.1"
+forust-ml = "0.2.2"
 polars = "0.24"
 reqwest = { version = "0.11", features = ["blocking"] }
 ```
 
 The following is a runable example using `polars` for data processing. The actual data manipulation can be performed with any tool, the only vital part, is the data be in column major format.
 ```rust
 use forust_ml::{GradientBooster, Matrix};
```

### Comparing `forust-0.2.1/local_dependencies/forust-ml/scripts/make_resources.py` & `forust-0.2.2/local_dependencies/forust-ml/scripts/make_resources.py`

 * *Files identical despite different names*

### Comparing `forust-0.2.1/local_dependencies/forust-ml/src/binning.rs` & `forust-0.2.2/local_dependencies/forust-ml/src/binning.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.1/local_dependencies/forust-ml/src/data.rs` & `forust-0.2.2/local_dependencies/forust-ml/src/data.rs`

 * *Files 3% similar despite different names*

```diff
@@ -115,14 +115,22 @@
 
     fn item_index(&self, i: usize, j: usize) -> usize {
         let mut idx = self.stride2 * i;
         idx += j * self.stride1;
         idx
     }
 
+    /// Get access to a row of the data, as an iterator.
+    pub fn get_row_iter(
+        &self,
+        row: usize,
+    ) -> std::iter::StepBy<std::iter::Skip<std::slice::Iter<T>>> {
+        self.data.iter().skip(row).step_by(self.rows)
+    }
+
     /// Get a slice of a column in the matrix.
     ///
     /// * `col` - The index of the column to select.
     /// * `start_row` - The index of the start of the slice.
     /// * `end_row` - The index of the end of the slice of the column to select.
     pub fn get_col_slice(&self, col: usize, start_row: usize, end_row: usize) -> &[T] {
         let i = self.item_index(start_row, col);
@@ -134,14 +142,24 @@
     ///
     /// * `col` - The index of the column to get.
     pub fn get_col(&self, col: usize) -> &[T] {
         self.get_col_slice(col, 0, self.rows)
     }
 }
 
+impl<'a, T> Matrix<'a, T>
+where
+    T: Copy,
+{
+    /// Get a row of the data as a vector.
+    pub fn get_row(&self, row: usize) -> Vec<T> {
+        self.get_row_iter(row).copied().collect()
+    }
+}
+
 /// A lightweight row major matrix, this is primarily
 /// for returning data to the user, it is especially
 /// suited for appending rows to, such as when building
 /// up a matrix of contributions to return to the
 /// user, the added benefit is it will be even
 /// faster to return to numpy.
 // pub struct RowMajorMatrix<T> {
@@ -223,15 +241,14 @@
         JaggedMatrix {
             data: Vec::new(),
             ends: Vec::new(),
             cols: 0,
             n_records: 0,
         }
     }
-
     /// Get the column of a jagged array.
     pub fn get_col(&self, col: usize) -> &[T] {
         assert!(col < self.ends.len());
         let (i, j) = if col == 0 {
             (0, self.ends[col])
         } else {
             (self.ends[col - 1], self.ends[col])
@@ -282,14 +299,23 @@
     fn test_matrix_get_col() {
         let v = vec![1, 2, 3, 5, 6, 7];
         let m = Matrix::new(&v, 3, 2);
         assert_eq!(m.get_col(1), &vec![5, 6, 7]);
     }
 
     #[test]
+    fn test_matrix_row() {
+        let v = vec![1, 2, 3, 5, 6, 7];
+        let m = Matrix::new(&v, 3, 2);
+        assert_eq!(m.get_row(2), vec![3, 7]);
+        assert_eq!(m.get_row(0), vec![1, 5]);
+        assert_eq!(m.get_row(1), vec![2, 6]);
+    }
+
+    #[test]
     fn test_jaggedmatrix_get_col() {
         let vecs = vec![vec![0], vec![5, 4, 3, 2], vec![4, 5]];
         let jmatrix = JaggedMatrix::from_vecs(&vecs);
         assert_eq!(jmatrix.get_col(1), vec![5, 4, 3, 2]);
         assert_eq!(jmatrix.get_col(0), vec![0]);
         assert_eq!(jmatrix.get_col(2), vec![4, 5]);
     }
```

### Comparing `forust-0.2.1/local_dependencies/forust-ml/src/gradientbooster.rs` & `forust-0.2.2/local_dependencies/forust-ml/src/gradientbooster.rs`

 * *Files 6% similar despite different names*

```diff
@@ -212,14 +212,38 @@
             for (p_, val) in init_preds.iter_mut().zip(tree.predict(data, parallel)) {
                 *p_ += val;
             }
         });
         init_preds
     }
 
+    // pub fn predict(&self, data: &Matrix<f64>, parallel: bool) -> Vec<f64> {
+    //     // After we disconvered it's faster materializing the row once, and then
+    //     // Passing that to each tree, let's see if we can do the same with the booster
+    //     // prediction...
+    //     // Clean this up..
+    //     let mut init_preds = vec![self.base_score; data.rows];
+    //     if parallel {
+    //         init_preds.par_iter_mut().enumerate().for_each(|(i, p)| {
+    //             let pred_row = data.get_row(i);
+    //             for t in &self.trees {
+    //                 *p += t.predict_row_from_row_slice(&pred_row);
+    //             }
+    //         });
+    //     } else {
+    //         init_preds.iter_mut().enumerate().for_each(|(i, p)| {
+    //             let pred_row = data.get_row(i);
+    //             for t in &self.trees {
+    //                 *p += t.predict_row_from_row_slice(&pred_row);
+    //             }
+    //         });
+    //     }
+    //     init_preds
+    // }
+
     /// Generate predictions on data using the gradient booster.
     ///
     /// * `data` -  Either a pandas DataFrame, or a 2 dimensional numpy array.
     pub fn predict_contributions(&self, data: &Matrix<f64>, parallel: bool) -> Vec<f64> {
         let weights: Vec<Vec<f64>> = if parallel {
             self.trees
                 .par_iter()
@@ -228,17 +252,49 @@
         } else {
             self.trees
                 .iter()
                 .map(|t| t.distribute_leaf_weights())
                 .collect()
         };
         let mut contribs = vec![0.; (data.cols + 1) * data.rows];
-        self.trees.iter().zip(weights.iter()).for_each(|(t, w)| {
-            t.predict_contributions(data, &mut contribs, w, parallel);
-        });
+
+        // Add the bias term to every bias value...
+        let bias_idx = data.cols + 1;
+        contribs
+            .iter_mut()
+            .skip(bias_idx - 1)
+            .step_by(bias_idx)
+            .for_each(|v| *v += self.base_score);
+
+        // Clean this up..
+        // materializing a row, and then passing that to all of the
+        // trees seems to be the fastest approach (5X faster), we should test
+        // something like this for normal predictions.
+        if parallel {
+            data.index
+                .par_iter()
+                .zip(contribs.par_chunks_mut(data.cols + 1))
+                .for_each(|(row, c)| {
+                    let r_ = data.get_row(*row);
+                    self.trees.iter().zip(weights.iter()).for_each(|(t, w)| {
+                        t.predict_contributions_row(&r_, c, w);
+                    });
+                });
+        } else {
+            data.index
+                .iter()
+                .zip(contribs.chunks_mut(data.cols + 1))
+                .for_each(|(row, c)| {
+                    let r_ = data.get_row(*row);
+                    self.trees.iter().zip(weights.iter()).for_each(|(t, w)| {
+                        t.predict_contributions_row(&r_, c, w);
+                    });
+                });
+        }
+
         contribs
     }
 
     /// Given a value, return the partial dependence value of that value for that
     /// feature in the model.
     ///
     /// * `feature` - The index of the feature.
```

### Comparing `forust-0.2.1/local_dependencies/forust-ml/src/histogram.rs` & `forust-0.2.2/local_dependencies/forust-ml/src/histogram.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.1/local_dependencies/forust-ml/src/node.rs` & `forust-0.2.2/local_dependencies/forust-ml/src/node.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.1/local_dependencies/forust-ml/src/objective.rs` & `forust-0.2.2/local_dependencies/forust-ml/src/objective.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.1/local_dependencies/forust-ml/src/partial_dependence.rs` & `forust-0.2.2/local_dependencies/forust-ml/src/partial_dependence.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.1/local_dependencies/forust-ml/src/splitter.rs` & `forust-0.2.2/local_dependencies/forust-ml/src/splitter.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.1/local_dependencies/forust-ml/src/tree.rs` & `forust-0.2.2/local_dependencies/forust-ml/src/tree.rs`

 * *Files 2% similar despite different names*

```diff
@@ -114,31 +114,25 @@
                 for n in new_nodes {
                     self.nodes.push(n.as_node());
                     growable.push_front(n)
                 }
             }
         }
     }
-    pub fn predict_contributions_row(
-        &self,
-        data: &Matrix<f64>,
-        row: usize,
-        contribs: &mut [f64],
-        weights: &[f64],
-    ) {
+    pub fn predict_contributions_row(&self, row: &[f64], contribs: &mut [f64], weights: &[f64]) {
         // Add the bias term first...
-        contribs[data.cols] += weights[0];
+        contribs[contribs.len() - 1] += weights[0];
         let mut node_idx = 0;
         loop {
             let node = &self.nodes[node_idx];
             if node.is_leaf {
                 break;
             }
             // Get change of weight given child's weight.
-            let child_idx = node.get_child_idx(data.get(row, node.split_feature));
+            let child_idx = node.get_child_idx(&row[node.split_feature]);
             let node_weight = weights[node_idx];
             let child_weight = weights[child_idx];
             let delta = child_weight - node_weight;
             contribs[node.split_feature] += delta;
             node_idx = child_idx
         }
     }
@@ -150,29 +144,30 @@
         weights: &[f64],
     ) {
         // There needs to always be at least 2 trees
         data.index
             .iter()
             .zip(contribs.chunks_mut(data.cols + 1))
             .for_each(|(row, contribs)| {
-                self.predict_contributions_row(data, *row, contribs, weights)
+                self.predict_contributions_row(&data.get_row(*row), contribs, weights)
             })
     }
+
     fn predict_contributions_parallel(
         &self,
         data: &Matrix<f64>,
         contribs: &mut [f64],
         weights: &[f64],
     ) {
         // There needs to always be at least 2 trees
         data.index
             .par_iter()
             .zip(contribs.par_chunks_mut(data.cols + 1))
             .for_each(|(row, contribs)| {
-                self.predict_contributions_row(data, *row, contribs, weights)
+                self.predict_contributions_row(&data.get_row(*row), contribs, weights)
             })
     }
 
     pub fn predict_contributions(
         &self,
         data: &Matrix<f64>,
         contribs: &mut [f64],
@@ -194,14 +189,26 @@
                 return node.weight_value as f64;
             } else {
                 node_idx = node.get_child_idx(data.get(row, node.split_feature));
             }
         }
     }
 
+    pub fn predict_row_from_row_slice(&self, row: &[f64]) -> f64 {
+        let mut node_idx = 0;
+        loop {
+            let node = &self.nodes[node_idx];
+            if node.is_leaf {
+                return node.weight_value as f64;
+            } else {
+                node_idx = node.get_child_idx(&row[node.split_feature]);
+            }
+        }
+    }
+
     fn predict_single_threaded(&self, data: &Matrix<f64>) -> Vec<f64> {
         data.index
             .iter()
             .map(|i| self.predict_row(data, *i))
             .collect()
     }
```

### Comparing `forust-0.2.1/local_dependencies/forust-ml/src/utils.rs` & `forust-0.2.2/local_dependencies/forust-ml/src/utils.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.1/.gitignore` & `forust-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `forust-0.2.1/README.md` & `forust-0.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 The package can be installed directly from [pypi](https://pypi.org/project/forust/).
 ```shell
 pip install forust
 ```
 
 To use in a rust project add the following to your Cargo.toml file.
 ```toml
-forust-ml = "0.2.1"
+forust-ml = "0.2.2"
 ```
 
 ## Usage
 The `GradientBooster` class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
 
 It can be initialized with the following arguments.
```

#### html2text {}

```diff
@@ -13,15 +13,15 @@
 understand the XGBoost algorithm, additionally to have a fun project to work on
 in rust, and because I wanted to be able to experiment with adding new features
 to the algorithm in a smaller simpler codebase. All of the rust code for the
 package can be found in the [src](src/) directory, while all of the python
 wrapper code is in the [py-forust](py-forust/) directory. ## Installation The
 package can be installed directly from [pypi](https://pypi.org/project/forust/
 ). ```shell pip install forust ``` To use in a rust project add the following
-to your Cargo.toml file. ```toml forust-ml = "0.2.1" ``` ## Usage The
+to your Cargo.toml file. ```toml forust-ml = "0.2.2" ``` ## Usage The
 `GradientBooster` class is currently the only public facing class in the
 package, and can be used to train gradient boosted decision tree ensembles with
 multiple objective functions. It can be initialized with the following
 arguments. - `objective_type` ***(str, optional)***: The name of objective
 function used to optimize. Valid options include "LogLoss" to use logistic loss
 as the objective function (binary classification), or "SquaredLoss" to use
 Squared Error as the objective function (continuous regression). Defaults to
```

### Comparing `forust-0.2.1/forust/__init__.py` & `forust-0.2.2/forust/__init__.py`

 * *Files identical despite different names*

### Comparing `forust-0.2.1/pyproject.toml` & `forust-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `forust-0.2.1/scratch.py` & `forust-0.2.2/scratch.py`

 * *Files identical despite different names*

### Comparing `forust-0.2.1/src/lib.rs` & `forust-0.2.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.1/tests/test_booster.py` & `forust-0.2.2/tests/test_booster.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,15 +274,15 @@
         max_depth=5,
         l2=1,
         min_leaf_weight=1,
         gamma=1,
         objective_type="LogLoss",
         nbins=500,
         parallel=False,
-        base_score=0.0,
+        base_score=0.5,
     )
     fmod.fit(X, y=y)
     fmod_preds = fmod.predict(X)
     fmod_contribs = fmod.predict_contributions(X)
     fmod_preds[~np.isclose(fmod_contribs.sum(1), fmod_preds, rtol=5)]
     fmod_contribs.sum(1)[~np.isclose(fmod_contribs.sum(1), fmod_preds, rtol=5)]
     assert fmod_contribs.shape[1] == X.shape[1] + 1
@@ -295,15 +295,15 @@
         reg_lambda=1,
         min_child_weight=1,
         gamma=1,
         objective="binary:logitraw",
         eval_metric="auc",
         tree_method="hist",
         max_bin=10000,
-        base_score=0.0,
+        base_score=0.5,
     )
     xmod.fit(X, y)
     xmod_preds = xmod.predict(X, output_margin=True)
     import xgboost as xgb
 
     xmod_contribs = xmod.get_booster().predict(
         xgb.DMatrix(X), approx_contribs=True, pred_contribs=True
```

### Comparing `forust-0.2.1/LICENSE` & `forust-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `forust-0.2.1/PKG-INFO` & `forust-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forust
-Version: 0.2.1
+Version: 0.2.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: numpy>=1.21
 Requires-Dist: pandas>=1.3
 Requires-Dist: maturin; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
@@ -43,15 +43,15 @@
 The package can be installed directly from [pypi](https://pypi.org/project/forust/).
 ```shell
 pip install forust
 ```
 
 To use in a rust project add the following to your Cargo.toml file.
 ```toml
-forust-ml = "0.2.1"
+forust-ml = "0.2.2"
 ```
 
 ## Usage
 The `GradientBooster` class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
 
 It can be initialized with the following arguments.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: forust Version: 0.2.1 Classifier: Programming
+Metadata-Version: 2.1 Name: forust Version: 0.2.2 Classifier: Programming
 Language :: Rust Classifier: Programming Language :: Python :: Implementation
 :: CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: numpy>=1.21 Requires-Dist: pandas>=1.3 Requires-Dist: maturin;
 extra == 'dev' Requires-Dist: pytest; extra == 'dev' Requires-Dist: seaborn;
 extra == 'dev' Requires-Dist: xgboost==1.6.1; extra == 'dev' Requires-Dist:
 scikit-learn; extra == 'dev' Provides-Extra: dev License-File: LICENSE Summary:
 A lightweight gradient boosting implementation in Rust. Keywords:
@@ -24,15 +24,15 @@
 understand the XGBoost algorithm, additionally to have a fun project to work on
 in rust, and because I wanted to be able to experiment with adding new features
 to the algorithm in a smaller simpler codebase. All of the rust code for the
 package can be found in the [src](src/) directory, while all of the python
 wrapper code is in the [py-forust](py-forust/) directory. ## Installation The
 package can be installed directly from [pypi](https://pypi.org/project/forust/
 ). ```shell pip install forust ``` To use in a rust project add the following
-to your Cargo.toml file. ```toml forust-ml = "0.2.1" ``` ## Usage The
+to your Cargo.toml file. ```toml forust-ml = "0.2.2" ``` ## Usage The
 `GradientBooster` class is currently the only public facing class in the
 package, and can be used to train gradient boosted decision tree ensembles with
 multiple objective functions. It can be initialized with the following
 arguments. - `objective_type` ***(str, optional)***: The name of objective
 function used to optimize. Valid options include "LogLoss" to use logistic loss
 as the objective function (binary classification), or "SquaredLoss" to use
 Squared Error as the objective function (continuous regression). Defaults to
```

