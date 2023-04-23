# Comparing `tmp/forust-0.2.0.tar.gz` & `tmp/forust-0.2.1.tar.gz`

## Comparing `forust-0.2.0.tar` & `forust-0.2.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 forust-0.2.0/local_dependencies/forust-ml/Cargo.toml
--rw-r--r--   0      501       20     5584 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/.github/workflows/CI.yml
--rw-r--r--   0      501       20      262 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/.gitignore
--rw-r--r--   0      501       20      320 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/.pre-commit-config.yaml
--rw-r--r--   0      501       20    11341 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/LICENSE
--rw-r--r--   0      501       20    10117 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/README.md
--rw-r--r--   0      501       20     3857 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/benches/forust_benchmarks.rs
--rw-r--r--   0      501       20   403349 2023-04-20 00:37:01.000000 forust-0.2.0/local_dependencies/forust-ml/dist/forust-0.2.0-cp310-cp310-macosx_10_7_x86_64.whl
--rw-r--r--   0      501       20   743715 2023-04-20 00:36:03.000000 forust-0.2.0/local_dependencies/forust-ml/dist/forust-0.2.0.tar.gz
--rw-r--r--   0      501       20    16121 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/resources/pdp_plot_age.png
--rw-r--r--   0      501       20    10758 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png
--rw-r--r--   0      501       20    57018 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/resources/titanic.csv
--rw-r--r--   0      501       20   655700 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/resources/tree-image-crop.png
--rw-r--r--   0      501       20     2556 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/rs-example.md
--rw-r--r--   0      501       20     1179 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/scripts/make_resources.py
--rw-r--r--   0      501       20       53 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/scripts/run-python-tests.ps1
--rw-r--r--   0      501       20       53 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/scripts/run-python-tests.sh
--rw-r--r--   0      501       20     5456 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/src/binning.rs
--rw-r--r--   0      501       20      248 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/src/constraints.rs
--rw-r--r--   0      501       20     7196 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/src/data.rs
--rw-r--r--   0      501       20      473 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/src/errors.rs
--rw-r--r--   0      501       20    16106 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/src/gradientbooster.rs
--rw-r--r--   0      501       20     8639 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/src/histogram.rs
--rw-r--r--   0      501       20      318 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/src/lib.rs
--rw-r--r--   0      501       20     5813 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/src/node.rs
--rw-r--r--   0      501       20     4125 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/src/objective.rs
--rw-r--r--   0      501       20     3650 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/src/partial_dependence.rs
--rw-r--r--   0      501       20    27732 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/src/splitter.rs
--rw-r--r--   0      501       20    10708 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/src/tree.rs
--rw-r--r--   0      501       20    28270 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/src/utils.rs
--rw-r--r--   0        0        0      391 1970-01-01 00:00:00.000000 forust-0.2.0/Cargo.toml
--rw-r--r--   0      501       20      685 2023-04-20 00:32:57.000000 forust-0.2.0/.gitignore
--rw-r--r--   0      501       20    10117 2023-04-20 00:33:45.000000 forust-0.2.0/README.md
--rw-r--r--   0      501       20    13982 2023-04-20 00:32:57.000000 forust-0.2.0/forust/__init__.py
--rw-r--r--   0      501       20      785 2023-04-20 00:32:57.000000 forust-0.2.0/pyproject.toml
--rw-r--r--   0      501       20     7353 2023-04-20 00:32:57.000000 forust-0.2.0/scratch.py
--rw-r--r--   0      501       20     7927 2023-04-20 00:32:57.000000 forust-0.2.0/src/lib.rs
--rw-r--r--   0      501       20     6632 2023-04-20 00:32:57.000000 forust-0.2.0/tests/test_booster.py
--rw-r--r--   0      501       20    11341 2023-04-20 00:33:45.000000 forust-0.2.0/LICENSE
--rw-r--r--   0      501       20    10117 2023-04-20 00:33:45.000000 forust-0.2.0/README.md
--rw-r--r--   0        0        0    10901 1970-01-01 00:00:00.000000 forust-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 forust-0.2.1/local_dependencies/forust-ml/Cargo.toml
+-rw-r--r--   0      501       20     5608 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      262 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/.gitignore
+-rw-r--r--   0      501       20      320 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/.pre-commit-config.yaml
+-rw-r--r--   0      501       20    11341 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/LICENSE
+-rw-r--r--   0      501       20    10881 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/README.md
+-rw-r--r--   0      501       20     3857 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/benches/forust_benchmarks.rs
+-rw-r--r--   0      501       20   396909 2023-04-23 02:43:43.000000 forust-0.2.1/local_dependencies/forust-ml/dist/forust-0.2.1-cp311-cp311-macosx_10_7_x86_64.whl
+-rw-r--r--   0      501       20   745373 2023-04-23 02:42:47.000000 forust-0.2.1/local_dependencies/forust-ml/dist/forust-0.2.1.tar.gz
+-rw-r--r--   0      501       20    16121 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/resources/pdp_plot_age.png
+-rw-r--r--   0      501       20    10758 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png
+-rw-r--r--   0      501       20    57018 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/resources/titanic.csv
+-rw-r--r--   0      501       20   655700 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/resources/tree-image-crop.png
+-rw-r--r--   0      501       20     2556 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/rs-example.md
+-rw-r--r--   0      501       20     1179 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/scripts/make_resources.py
+-rw-r--r--   0      501       20       53 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/scripts/run-python-tests.ps1
+-rw-r--r--   0      501       20       53 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/scripts/run-python-tests.sh
+-rw-r--r--   0      501       20     5456 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/src/binning.rs
+-rw-r--r--   0      501       20      248 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/src/constraints.rs
+-rw-r--r--   0      501       20     7678 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/src/data.rs
+-rw-r--r--   0      501       20      473 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/src/errors.rs
+-rw-r--r--   0      501       20    17082 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/src/gradientbooster.rs
+-rw-r--r--   0      501       20     8639 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/src/histogram.rs
+-rw-r--r--   0      501       20      318 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/src/lib.rs
+-rw-r--r--   0      501       20     5901 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/src/node.rs
+-rw-r--r--   0      501       20     4125 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/src/objective.rs
+-rw-r--r--   0      501       20     3146 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/src/partial_dependence.rs
+-rw-r--r--   0      501       20    27105 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/src/splitter.rs
+-rw-r--r--   0      501       20    13817 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/src/tree.rs
+-rw-r--r--   0      501       20    28561 2023-04-23 02:39:52.000000 forust-0.2.1/local_dependencies/forust-ml/src/utils.rs
+-rw-r--r--   0        0        0      391 1970-01-01 00:00:00.000000 forust-0.2.1/Cargo.toml
+-rw-r--r--   0      501       20      685 2023-04-23 02:39:52.000000 forust-0.2.1/.gitignore
+-rw-r--r--   0      501       20    10881 2023-04-23 02:40:40.000000 forust-0.2.1/README.md
+-rw-r--r--   0      501       20    15483 2023-04-23 02:39:52.000000 forust-0.2.1/forust/__init__.py
+-rw-r--r--   0      501       20      785 2023-04-23 02:39:52.000000 forust-0.2.1/pyproject.toml
+-rw-r--r--   0      501       20     7353 2023-04-23 02:39:52.000000 forust-0.2.1/scratch.py
+-rw-r--r--   0      501       20     8439 2023-04-23 02:39:52.000000 forust-0.2.1/src/lib.rs
+-rw-r--r--   0      501       20     7940 2023-04-23 02:39:52.000000 forust-0.2.1/tests/test_booster.py
+-rw-r--r--   0      501       20    11341 2023-04-23 02:40:40.000000 forust-0.2.1/LICENSE
+-rw-r--r--   0      501       20    10881 2023-04-23 02:40:40.000000 forust-0.2.1/README.md
+-rw-r--r--   0        0        0    11665 1970-01-01 00:00:00.000000 forust-0.2.1/PKG-INFO
```

### Comparing `forust-0.2.0/local_dependencies/forust-ml/Cargo.toml` & `forust-0.2.1/local_dependencies/forust-ml/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [package]
 name = "forust-ml"
-version = "0.2.0"
+version = "0.2.1"
 edition = "2021"
 authors = ["James Inlow <james.d.inlow@gmail.com>"]
 homepage = "https://github.com/jinlow/forust"
 description = "A lightweight gradient boosting implementation in Rust."
 license-file = "LICENSE"
 readme = "README.md"
 repository = "https://github.com/jinlow/forust"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
-rayon = "1.5"
-thiserror = "1.0.31"
+rayon = "1.7"
+thiserror = "1.0"
 serde_json = {version = "1.0", features = ["float_roundtrip"] }
 serde = { version = "1.0", features = ["derive"] }
 
 [dev-dependencies]
 criterion = "0.4"
 rand = "0.8.5"
```

### Comparing `forust-0.2.0/local_dependencies/forust-ml/.github/workflows/CI.yml` & `forust-0.2.1/local_dependencies/forust-ml/.github/workflows/CI.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 name: Test and Deploy
 on: [pull_request, push]
 
 jobs:
   windows-build-tests:
     strategy:
       matrix:
-        pyversion: ["3.8", "3.9", "3.10"]
+        pyversion: ["3.8", "3.9", "3.10", "3.11"]
     runs-on: "windows-latest"
     steps:
       - uses: actions/checkout@v2
       - name: Install latests stable Rust
         uses: actions-rs/toolchain@v1
         with:
           toolchain: stable
@@ -54,15 +54,15 @@
         with:
           command: publish
           args: --username ${{ secrets.PYPI_USERNAME }} --password ${{ secrets.PYPI_PASSWORD }} --interpreter python --skip-existing --manifest-path py-forust/Cargo.toml
 
   macos-build-test:
     strategy:
       matrix:
-        pyversion: ["3.8", "3.9", "3.10"]
+        pyversion: ["3.8", "3.9", "3.10", "3.11"]
     runs-on: "macos-latest"
     steps:
       - uses: actions/checkout@v2
       - name: Install latests stable Rust
         uses: actions-rs/toolchain@v1
         with:
           toolchain: stable
@@ -109,15 +109,15 @@
           target: x86_64
           args: --username ${{ secrets.PYPI_USERNAME }} --password ${{ secrets.PYPI_PASSWORD }} --interpreter python --skip-existing --manifest-path py-forust/Cargo.toml
 
   linux-build-test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        pyversion: ["3.8", "3.9", "3.10"]
+        pyversion: ["3.8", "3.9", "3.10", "3.11"]
         # target: [x86_64, i686]
     steps:
       - uses: actions/checkout@v2
       - name: Install latests stable Rust
         uses: actions-rs/toolchain@v1
         with:
           toolchain: stable
```

### Comparing `forust-0.2.0/local_dependencies/forust-ml/LICENSE` & `forust-0.2.1/local_dependencies/forust-ml/LICENSE`

 * *Files identical despite different names*

### Comparing `forust-0.2.0/local_dependencies/forust-ml/README.md` & `forust-0.2.1/local_dependencies/forust-ml/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 The package can be installed directly from [pypi](https://pypi.org/project/forust/).
 ```shell
 pip install forust
 ```
 
 To use in a rust project add the following to your Cargo.toml file.
 ```toml
-forust-ml = "0.2.0"
+forust-ml = "0.2.1"
 ```
 
 ## Usage
 The `GradientBooster` class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
 
 It can be initialized with the following arguments.
 
@@ -80,14 +80,21 @@
 from forust import GradientBooster
 model = GradientBooster(objective_type="LogLoss")
 model.fit(X, y)
 
 # Predict on data
 model.predict(X.head())
 # array([-1.94919663,  2.25863229,  0.32963671,  2.48732194, -3.00371813])
+
+# predict contributions
+model.predict_contributions(X.head())
+# array([[-0.63014213,  0.33880048, -0.16520798, -0.07798772, -0.85083578,
+#        -1.07720813],
+#       [ 1.05406709,  0.08825999,  0.21662544, -0.12083538,  0.35209258,
+#        -1.07720813],
 ```
 
 The `fit` method accepts the following arguments.
  - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data.
  - `y` ***(ArrayLike)***: Either a pandas Series, or a 1 dimensional numpy array. If "LogLoss" was
    the objective type specified, then this should only contain 1 or 0 values, where 1 is the positive class being predicted. If "SquaredLoss" is the objective type, then any continuous variable can be
    provided.
@@ -98,14 +105,21 @@
 The predict method accepts the following arguments.
  - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data.
  - `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict
    function should run in parallel on multiple threads. If `None` is
    passed, the `parallel` attribute of the booster will be used.
    Defaults to `None`.
 
+The `predict_contributions` method will predict with the fitted booster on new data, returning the feature contribution matrix. The last column is the bias term.
+ - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data.
+ - `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict
+   function should run in parallel on multiple threads. If `None` is
+   passed, the `parallel` attribute of the booster will be used.
+   Defaults to `None`.
+
 ### Inspecting the Model
 
 Once the booster has been fit, each individual tree structure can be retrieved in text form, using the `text_dump` method. This method returns a list, the same length as the number of trees in the model.
 
 ```python
 model.text_dump()[0]
 # 0:[0 < 3] yes=1,no=2,missing=2,gain=91.50833,cover=209.388307
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
-to your Cargo.toml file. ```toml forust-ml = "0.2.0" ``` ## Usage The
+to your Cargo.toml file. ```toml forust-ml = "0.2.1" ``` ## Usage The
 `GradientBooster` class is currently the only public facing class in the
 package, and can be used to train gradient boosted decision tree ensembles with
 multiple objective functions. It can be initialized with the following
 arguments. - `objective_type` ***(str, optional)***: The name of objective
 function used to optimize. Valid options include "LogLoss" to use logistic loss
 as the objective function (binary classification), or "SquaredLoss" to use
 Squared Error as the objective function (continuous regression). Defaults to
@@ -66,31 +66,41 @@
 dataset. In the case of this example, the predictions are the log odds of a
 given record being 1. ```python # Small example dataset from seaborn import
 load_dataset df = load_dataset("titanic") X = df.select_dtypes("number").drop
 (columns=["survived"]) y = df["survived"] # Initialize a booster with defaults.
 from forust import GradientBooster model = GradientBooster
 (objective_type="LogLoss") model.fit(X, y) # Predict on data model.predict
 (X.head()) # array([-1.94919663, 2.25863229, 0.32963671, 2.48732194, -
-3.00371813]) ``` The `fit` method accepts the following arguments. - `X` ***
+3.00371813]) # predict contributions model.predict_contributions(X.head()) #
+array([[-0.63014213, 0.33880048, -0.16520798, -0.07798772, -0.85083578, # -
+1.07720813], # [ 1.05406709, 0.08825999, 0.21662544, -0.12083538, 0.35209258, #
+-1.07720813], ``` The `fit` method accepts the following arguments. - `X` ***
 (FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with
 numeric data. - `y` ***(ArrayLike)***: Either a pandas Series, or a 1
 dimensional numpy array. If "LogLoss" was the objective type specified, then
 this should only contain 1 or 0 values, where 1 is the positive class being
 predicted. If "SquaredLoss" is the objective type, then any continuous variable
 can be provided. - `sample_weight` ***(Optional[ArrayLike], optional)***:
 Instance weights to use when training the model. If None is passed, a weight of
 1 will be used for every record. Defaults to None. The predict method accepts
 the following arguments. - `X` ***(FrameLike)***: Either a pandas DataFrame, or
 a 2 dimensional numpy array, with numeric data. - `parallel` ***(Optional
 [bool], optional)***: Optionally specify if the predict function should run in
 parallel on multiple threads. If `None` is passed, the `parallel` attribute of
-the booster will be used. Defaults to `None`. ### Inspecting the Model Once the
-booster has been fit, each individual tree structure can be retrieved in text
-form, using the `text_dump` method. This method returns a list, the same length
-as the number of trees in the model. ```python model.text_dump()[0] # 0:[0 < 3]
+the booster will be used. Defaults to `None`. The `predict_contributions`
+method will predict with the fitted booster on new data, returning the feature
+contribution matrix. The last column is the bias term. - `X` ***(FrameLike)***:
+Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data. -
+`parallel` ***(Optional[bool], optional)***: Optionally specify if the predict
+function should run in parallel on multiple threads. If `None` is passed, the
+`parallel` attribute of the booster will be used. Defaults to `None`. ###
+Inspecting the Model Once the booster has been fit, each individual tree
+structure can be retrieved in text form, using the `text_dump` method. This
+method returns a list, the same length as the number of trees in the model.
+```python model.text_dump()[0] # 0:[0 < 3]
 yes=1,no=2,missing=2,gain=91.50833,cover=209.388307 # 1:[4 < 13.7917]
 yes=3,no=4,missing=4,gain=28.185467,cover=94.00148 # 3:[1 < 18]
 yes=7,no=8,missing=8,gain=1.4576768,cover=22.090348 # 7:[1 < 17]
 yes=15,no=16,missing=16,gain=0.691266,cover=0.705011 # 15:leaf=-
 0.15120,cover=0.23500 # 16:leaf=0.154097,cover=0.470007 ``` The `json_dump`
 method performs the same action, but returns the model as a json representation
 rather than a text string. To see an estimate for how a given feature is used
```

### Comparing `forust-0.2.0/local_dependencies/forust-ml/benches/forust_benchmarks.rs` & `forust-0.2.1/local_dependencies/forust-ml/benches/forust_benchmarks.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.0/local_dependencies/forust-ml/resources/pdp_plot_age.png` & `forust-0.2.1/local_dependencies/forust-ml/resources/pdp_plot_age.png`

 * *Files identical despite different names*

### Comparing `forust-0.2.0/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png` & `forust-0.2.1/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png`

 * *Files identical despite different names*

### Comparing `forust-0.2.0/local_dependencies/forust-ml/resources/titanic.csv` & `forust-0.2.1/local_dependencies/forust-ml/resources/titanic.csv`

 * *Files identical despite different names*

### Comparing `forust-0.2.0/local_dependencies/forust-ml/resources/tree-image-crop.png` & `forust-0.2.1/local_dependencies/forust-ml/resources/tree-image-crop.png`

 * *Files identical despite different names*

### Comparing `forust-0.2.0/local_dependencies/forust-ml/rs-example.md` & `forust-0.2.1/local_dependencies/forust-ml/rs-example.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ## A Complete Rust Example
 
 To run this example, add the following code to your `Cargo.toml` file.
 ```toml
 [dependencies]
-forust-ml = "0.2.0"
+forust-ml = "0.2.1"
 polars = "0.24"
 reqwest = { version = "0.11", features = ["blocking"] }
 ```
 
 The following is a runable example using `polars` for data processing. The actual data manipulation can be performed with any tool, the only vital part, is the data be in column major format.
 ```rust
 use forust_ml::{GradientBooster, Matrix};
```

### Comparing `forust-0.2.0/local_dependencies/forust-ml/scripts/make_resources.py` & `forust-0.2.1/local_dependencies/forust-ml/scripts/make_resources.py`

 * *Files identical despite different names*

### Comparing `forust-0.2.0/local_dependencies/forust-ml/src/binning.rs` & `forust-0.2.1/local_dependencies/forust-ml/src/binning.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.0/local_dependencies/forust-ml/src/data.rs` & `forust-0.2.1/local_dependencies/forust-ml/src/data.rs`

 * *Files 8% similar despite different names*

```diff
@@ -89,14 +89,15 @@
     pub rows: usize,
     pub cols: usize,
     stride1: usize,
     stride2: usize,
 }
 
 impl<'a, T> Matrix<'a, T> {
+    // Defaults to column major
     pub fn new(data: &'a [T], rows: usize, cols: usize) -> Self {
         Matrix {
             data,
             index: (0..rows).collect(),
             rows,
             cols,
             stride1: rows,
@@ -133,14 +134,28 @@
     ///
     /// * `col` - The index of the column to get.
     pub fn get_col(&self, col: usize) -> &[T] {
         self.get_col_slice(col, 0, self.rows)
     }
 }
 
+/// A lightweight row major matrix, this is primarily
+/// for returning data to the user, it is especially
+/// suited for appending rows to, such as when building
+/// up a matrix of contributions to return to the
+/// user, the added benefit is it will be even
+/// faster to return to numpy.
+// pub struct RowMajorMatrix<T> {
+//     pub data: Vec<T>,
+//     pub rows: usize,
+//     pub cols: usize,
+//     stride1: usize,
+//     stride2: usize,
+// }
+
 impl<'a, T> fmt::Display for Matrix<'a, T>
 where
     T: FromStr + std::fmt::Display,
     <T as FromStr>::Err: 'static + std::error::Error,
 {
     // This trait requires `fmt` with this exact signature.
     /// Format a Matrix.
```

### Comparing `forust-0.2.0/local_dependencies/forust-ml/src/gradientbooster.rs` & `forust-0.2.1/local_dependencies/forust-ml/src/gradientbooster.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 use crate::binning::bin_matrix;
 use crate::constraints::ConstraintMap;
 use crate::data::Matrix;
 use crate::errors::ForustError;
 use crate::objective::{gradient_hessian_callables, ObjectiveType};
 use crate::splitter::MissingImputerSplitter;
 use crate::tree::Tree;
+use rayon::prelude::*;
 use serde::{Deserialize, Serialize};
 use std::fs;
 
 /// Gradient Booster object
 ///
 /// * `objective_type` - The name of objective function used to optimize.
 ///   Valid options include "LogLoss" to use logistic loss as the objective function,
@@ -211,14 +212,36 @@
             for (p_, val) in init_preds.iter_mut().zip(tree.predict(data, parallel)) {
                 *p_ += val;
             }
         });
         init_preds
     }
 
+    /// Generate predictions on data using the gradient booster.
+    ///
+    /// * `data` -  Either a pandas DataFrame, or a 2 dimensional numpy array.
+    pub fn predict_contributions(&self, data: &Matrix<f64>, parallel: bool) -> Vec<f64> {
+        let weights: Vec<Vec<f64>> = if parallel {
+            self.trees
+                .par_iter()
+                .map(|t| t.distribute_leaf_weights())
+                .collect()
+        } else {
+            self.trees
+                .iter()
+                .map(|t| t.distribute_leaf_weights())
+                .collect()
+        };
+        let mut contribs = vec![0.; (data.cols + 1) * data.rows];
+        self.trees.iter().zip(weights.iter()).for_each(|(t, w)| {
+            t.predict_contributions(data, &mut contribs, w, parallel);
+        });
+        contribs
+    }
+
     /// Given a value, return the partial dependence value of that value for that
     /// feature in the model.
     ///
     /// * `feature` - The index of the feature.
     /// * `value` - The value for which to calculate the partial dependence.
     pub fn value_partial_dependence(&self, feature: usize, value: f64) -> f64 {
         let pd: f64 = self
@@ -386,14 +409,16 @@
         let mut booster = GradientBooster::default();
         booster.iterations = 10;
         booster.nbins = 300;
         booster.max_depth = 3;
         let sample_weight = vec![1.; y.len()];
         booster.fit(&data, &y, &sample_weight).unwrap();
         let preds = booster.predict(&data, false);
+        let contribs = booster.predict_contributions(&data, false);
+        assert_eq!(contribs.len(), (data.cols + 1) * data.rows);
         println!("{}", booster.trees[0]);
         println!("{}", booster.trees[0].nodes.len());
         println!("{}", booster.trees.last().unwrap().nodes.len());
         println!("{:?}", &preds[0..10]);
     }
 
     #[test]
```

### Comparing `forust-0.2.0/local_dependencies/forust-ml/src/histogram.rs` & `forust-0.2.1/local_dependencies/forust-ml/src/histogram.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.0/local_dependencies/forust-ml/src/node.rs` & `forust-0.2.1/local_dependencies/forust-ml/src/node.rs`

 * *Files 27% similar despite different names*

```diff
@@ -19,45 +19,65 @@
     pub missing_node: usize,
     pub left_child: usize,
     pub right_child: usize,
     pub start_idx: usize,
     pub stop_idx: usize,
     pub lower_bound: f32,
     pub upper_bound: f32,
+    pub is_leaf: bool,
 }
 
 #[derive(Deserialize, Serialize)]
-pub struct ParentNode {
+pub struct Node {
     pub num: usize,
     pub weight_value: f32,
     pub hessian_sum: f32,
     pub depth: usize,
     pub split_value: f64,
     pub split_feature: usize,
     pub split_gain: f32,
     pub missing_node: usize,
     pub left_child: usize,
     pub right_child: usize,
+    pub is_leaf: bool,
+}
+
+impl Node {
+    /// Update all the info that is needed if this node is a
+    /// parent node, this consumes the SplitableNode.
+    pub fn make_parent_node(&mut self, split_node: SplittableNode) {
+        self.is_leaf = false;
+        self.missing_node = split_node.missing_node;
+        self.split_value = split_node.split_value;
+        self.split_feature = split_node.split_feature;
+        self.split_gain = split_node.split_gain;
+        self.left_child = split_node.left_child;
+        self.right_child = split_node.right_child;
+    }
+    /// Get the path that should be traveled down, given a value.
+    pub fn get_child_idx(&self, v: &f64) -> usize {
+        if v.is_nan() {
+            self.missing_node
+        } else if v < &self.split_value {
+            self.left_child
+        } else {
+            //  if v >= &self.split_value
+            self.right_child
+        }
+    }
 }
 
 #[derive(Deserialize, Serialize)]
 pub struct LeafNode {
     pub num: usize,
     pub weight_value: f32,
     pub hessian_sum: f32,
     pub depth: usize,
 }
 
-#[derive(Deserialize, Serialize)]
-pub enum TreeNode {
-    Parent(ParentNode),
-    Leaf(LeafNode),
-    Splittable(SplittableNode),
-}
-
 impl SplittableNode {
     pub fn from_node_info(
         num: usize,
         histograms: HistogramMatrix,
         depth: usize,
         start_idx: usize,
         stop_idx: usize,
@@ -77,17 +97,20 @@
             missing_node: 0,
             left_child: 0,
             right_child: 0,
             start_idx,
             stop_idx,
             lower_bound: node_info.bounds.0,
             upper_bound: node_info.bounds.1,
+            is_leaf: true,
         }
     }
 
+    /// Create a default splitable node,
+    /// we default to the node being a leaf.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         num: usize,
         histograms: HistogramMatrix,
         weight_value: f32,
         gain_value: f32,
         gradient_sum: f32,
@@ -112,14 +135,15 @@
             missing_node: 0,
             left_child: 0,
             right_child: 0,
             start_idx,
             stop_idx,
             lower_bound,
             upper_bound,
+            is_leaf: true,
         }
     }
 
     pub fn update_children(
         &mut self,
         left_child: usize,
         right_child: usize,
@@ -132,72 +156,51 @@
         self.split_value = split_info.split_value;
         self.missing_node = match split_info.missing_node {
             MissingInfo::Left => left_child,
             MissingInfo::Right => right_child,
             MissingInfo::Branch(_) => todo!(),
             MissingInfo::EmptyBranch => todo!(),
         };
+        self.is_leaf = false;
     }
-    pub fn as_leaf_node(&self) -> TreeNode {
-        TreeNode::Leaf(LeafNode {
-            num: self.num,
-            weight_value: self.weight_value,
-            hessian_sum: self.hessian_sum,
-            depth: self.depth,
-        })
-    }
-    pub fn as_parent_node(&self) -> TreeNode {
-        TreeNode::Parent(ParentNode {
+    pub fn as_node(&self) -> Node {
+        Node {
             num: self.num,
             weight_value: self.weight_value,
             hessian_sum: self.hessian_sum,
             depth: self.depth,
             missing_node: self.missing_node,
             split_value: self.split_value,
             split_feature: self.split_feature,
             split_gain: self.split_gain,
             left_child: self.left_child,
             right_child: self.right_child,
-        })
+            is_leaf: self.is_leaf,
+        }
     }
 }
 
-impl fmt::Display for TreeNode {
+impl fmt::Display for Node {
     // This trait requires `fmt` with this exact signature.
     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
-        match self {
-            TreeNode::Leaf(leaf) => write!(
+        if self.is_leaf {
+            write!(
                 f,
                 "{}:leaf={},cover={}",
-                leaf.num, leaf.weight_value, leaf.hessian_sum
-            ),
-            TreeNode::Parent(parent) => {
-                write!(
-                    f,
-                    "{}:[{} < {}] yes={},no={},missing={},gain={},cover={}",
-                    parent.num,
-                    parent.split_feature,
-                    parent.split_value,
-                    parent.left_child,
-                    parent.right_child,
-                    parent.missing_node,
-                    parent.split_gain,
-                    parent.hessian_sum
-                )
-            }
-            TreeNode::Splittable(node) => {
-                write!(
-                    f,
-                    "SPLITTABLE - {}:[{} < {}] yes={},no={},missing={},gain={},cover={}",
-                    node.num,
-                    node.split_feature,
-                    node.split_value,
-                    node.missing_node,
-                    node.left_child,
-                    node.right_child,
-                    node.split_gain,
-                    node.hessian_sum
-                )
-            }
+                self.num, self.weight_value, self.hessian_sum
+            )
+        } else {
+            write!(
+                f,
+                "{}:[{} < {}] yes={},no={},missing={},gain={},cover={}",
+                self.num,
+                self.split_feature,
+                self.split_value,
+                self.left_child,
+                self.right_child,
+                self.missing_node,
+                self.split_gain,
+                self.hessian_sum
+            )
         }
     }
 }
```

### Comparing `forust-0.2.0/local_dependencies/forust-ml/src/objective.rs` & `forust-0.2.1/local_dependencies/forust-ml/src/objective.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.0/local_dependencies/forust-ml/src/partial_dependence.rs` & `forust-0.2.1/local_dependencies/forust-ml/src/partial_dependence.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,57 @@
-use crate::node::TreeNode;
 use crate::tree::Tree;
 
 /// Partial Dependence Calculator
 // struct PDCalculator {
 //     partial_dependence: f32,
 //     base_score: f64,
 //     tree_prediction: f64,
 
 // }
 
 fn get_node_cover(tree: &Tree, node_idx: usize) -> f32 {
-    match &tree.nodes[node_idx] {
-        TreeNode::Leaf(n) => n.hessian_sum,
-        TreeNode::Parent(n) => n.hessian_sum,
-        TreeNode::Splittable(_) => unreachable!(),
-    }
+    tree.nodes[node_idx].hessian_sum
 }
 
 pub fn tree_partial_dependence(
     tree: &Tree,
     node_idx: usize,
     feature: usize,
     value: f64,
     proportion: f32,
 ) -> f64 {
-    let node = &tree.nodes[node_idx];
-    match node {
-        TreeNode::Leaf(n) => f64::from(proportion * n.weight_value),
-        TreeNode::Parent(n) => {
-            if n.split_feature == feature {
-                let child = if value.is_nan() {
-                    n.missing_node
-                } else if value < n.split_value {
-                    n.left_child
-                } else {
-                    n.right_child
-                };
-                tree_partial_dependence(tree, child, feature, value, proportion)
-            } else {
-                let left_cover = get_node_cover(tree, n.left_child);
-                let right_cover = get_node_cover(tree, n.right_child);
-                let total_cover = left_cover + right_cover;
-
-                tree_partial_dependence(
-                    tree,
-                    n.left_child,
-                    feature,
-                    value,
-                    proportion * (left_cover / total_cover),
-                ) + tree_partial_dependence(
-                    tree,
-                    n.right_child,
-                    feature,
-                    value,
-                    proportion * (right_cover / total_cover),
-                )
-            }
-        }
-        TreeNode::Splittable(_) => unreachable!(),
+    let n = &tree.nodes[node_idx];
+    if n.is_leaf {
+        f64::from(proportion * n.weight_value)
+    } else if n.split_feature == feature {
+        let child = if value.is_nan() {
+            n.missing_node
+        } else if value < n.split_value {
+            n.left_child
+        } else {
+            n.right_child
+        };
+        tree_partial_dependence(tree, child, feature, value, proportion)
+    } else {
+        let left_cover = get_node_cover(tree, n.left_child);
+        let right_cover = get_node_cover(tree, n.right_child);
+        let total_cover = left_cover + right_cover;
+        tree_partial_dependence(
+            tree,
+            n.left_child,
+            feature,
+            value,
+            proportion * (left_cover / total_cover),
+        ) + tree_partial_dependence(
+            tree,
+            n.right_child,
+            feature,
+            value,
+            proportion * (right_cover / total_cover),
+        )
     }
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
     use crate::binning::bin_matrix;
```

### Comparing `forust-0.2.0/local_dependencies/forust-ml/src/splitter.rs` & `forust-0.2.1/local_dependencies/forust-ml/src/splitter.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-use std::collections::VecDeque;
-
 use crate::constraints::{Constraint, ConstraintMap};
 use crate::data::{JaggedMatrix, Matrix};
 use crate::histogram::HistogramMatrix;
 use crate::node::SplittableNode;
-use crate::node::TreeNode;
 use crate::utils::{constrained_weight, cull_gain, gain_given_weight, pivot_on_split, weight};
 
 #[derive(Debug)]
 pub struct SplitInfo {
     pub split_gain: f32,
     pub split_feature: usize,
     pub split_value: f64,
@@ -182,42 +179,31 @@
         node: &mut SplittableNode,
         index: &mut [usize],
         data: &Matrix<u16>,
         cuts: &JaggedMatrix<f64>,
         grad: &[f32],
         hess: &[f32],
         parallel: bool,
-        growable_buffer: &mut VecDeque<usize>,
-    ) -> Vec<TreeNode>;
+    ) -> Vec<SplittableNode>;
 
     #[allow(clippy::too_many_arguments)]
     fn split_node(
         &self,
         n_nodes: &usize,
         node: &mut SplittableNode,
         index: &mut [usize],
         data: &Matrix<u16>,
         cuts: &JaggedMatrix<f64>,
         grad: &[f32],
         hess: &[f32],
         parallel: bool,
-        growable_buffer: &mut VecDeque<usize>,
-    ) -> Vec<TreeNode> {
+    ) -> Vec<SplittableNode> {
         match self.best_split(node) {
             Some(split_info) => self.handle_split_info(
-                split_info,
-                n_nodes,
-                node,
-                index,
-                data,
-                cuts,
-                grad,
-                hess,
-                parallel,
-                growable_buffer,
+                split_info, n_nodes, node, index, data, cuts, grad, hess, parallel,
             ),
             None => Vec::new(),
         }
     }
 }
 
 /// Missing branch splitter
@@ -350,16 +336,15 @@
         node: &mut SplittableNode,
         index: &mut [usize],
         data: &Matrix<u16>,
         cuts: &JaggedMatrix<f64>,
         grad: &[f32],
         hess: &[f32],
         parallel: bool,
-        growable_buffer: &mut VecDeque<usize>,
-    ) -> Vec<TreeNode> {
+    ) -> Vec<SplittableNode> {
         todo!()
     }
 }
 
 /// Missing imputer splitter
 /// Splitter that imputes missing values, by sending
 /// them down either the right or left branch, depending
@@ -556,16 +541,15 @@
         node: &mut SplittableNode,
         index: &mut [usize],
         data: &Matrix<u16>,
         cuts: &JaggedMatrix<f64>,
         grad: &[f32],
         hess: &[f32],
         parallel: bool,
-        growable_buffer: &mut VecDeque<usize>,
-    ) -> Vec<TreeNode> {
+    ) -> Vec<SplittableNode> {
         let left_idx = *n_nodes;
         let right_idx = left_idx + 1;
 
         let missing_right = match split_info.missing_node {
             MissingInfo::Left => false,
             MissingInfo::Right => true,
             MissingInfo::Branch(_) => todo!(),
@@ -637,21 +621,15 @@
             right_idx,
             right_histograms,
             node.depth + 1,
             split_idx,
             node.stop_idx,
             split_info.right_node,
         );
-        growable_buffer.push_front(left_idx);
-        growable_buffer.push_front(right_idx);
-        // It has children, so we know it's going to be a parent node
-        vec![
-            TreeNode::Splittable(left_node),
-            TreeNode::Splittable(right_node),
-        ]
+        vec![left_node, right_node]
     }
 
     fn get_constraint(&self, feature: &usize) -> Option<&Constraint> {
         self.constraints_map.get(feature)
     }
 
     fn get_gamma(&self) -> f32 {
```

### Comparing `forust-0.2.0/local_dependencies/forust-ml/src/tree.rs` & `forust-0.2.1/local_dependencies/forust-ml/src/tree.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 use crate::data::{JaggedMatrix, Matrix};
 use crate::histogram::HistogramMatrix;
-use crate::node::{SplittableNode, TreeNode};
+use crate::node::{Node, SplittableNode};
 use crate::partial_dependence::tree_partial_dependence;
 use crate::splitter::Splitter;
 use crate::utils::fast_f64_sum;
 use crate::utils::{gain, weight};
 use rayon::prelude::*;
 use serde::{Deserialize, Serialize};
 use std::collections::VecDeque;
 use std::fmt::{self, Display};
 
 #[derive(Deserialize, Serialize)]
 pub struct Tree {
-    pub nodes: Vec<TreeNode>,
+    pub nodes: Vec<Node>,
 }
 
 impl Default for Tree {
     fn default() -> Self {
         Self::new()
     }
 }
@@ -59,102 +59,145 @@
             0,
             0,
             data.rows,
             f32::NEG_INFINITY,
             f32::INFINITY,
         );
         // Add the first node to the tree nodes.
-        self.nodes.push(TreeNode::Splittable(root_node));
+        self.nodes.push(root_node.as_node());
         let mut n_leaves = 1;
-        let mut growable = VecDeque::new();
-        growable.push_front(0);
+        let mut growable: VecDeque<SplittableNode> = VecDeque::new();
+        growable.push_front(root_node);
         while !growable.is_empty() {
             if n_leaves >= max_leaves {
-                // Clear the rest of the node idxs that
-                // are not needed.
-                for i in growable.iter() {
-                    let n = &self.nodes[*i];
-                    if let TreeNode::Splittable(node) = n {
-                        self.nodes[*i] = node.as_leaf_node();
-                    }
-                }
                 break;
             }
 
             // We know there is a value here, because of how the
             // while loop is setup.
-            let n_idx = growable
+            // Grab a splitable node from the stack
+            // If we can split it, and update the corresponding
+            // tree nodes children.
+            let mut node = growable
                 .pop_back()
                 .expect("Growable buffer should not be empty.");
-
-            let n = self.nodes.get_mut(n_idx);
+            let n_idx = node.num;
             // This will only be splittable nodes
-            if let Some(TreeNode::Splittable(node)) = n {
-                let depth = node.depth + 1;
 
-                // If we have hit max depth, skip this node
-                // but keep going, because there may be other
-                // valid shallower nodes.
-                if depth > max_depth {
-                    self.nodes[n_idx] = node.as_leaf_node();
-                    continue;
-                }
+            let depth = node.depth + 1;
+
+            // If we have hit max depth, skip this node
+            // but keep going, because there may be other
+            // valid shallower nodes.
+            if depth > max_depth {
+                // self.nodes[n_idx] = node.as_leaf_node();
+                continue;
+            }
 
-                // For max_leaves, subtract 1 from the n_leaves
-                // every time we pop from the growable stack
-                // then, if we can add two children, add two to
-                // n_leaves. If we can't split the node any
-                // more, then just add 1 back to n_leaves
-                n_leaves -= 1;
-
-                let new_nodes = splitter.split_node(
-                    &n_nodes,
-                    node,
-                    &mut index,
-                    data,
-                    cuts,
-                    grad,
-                    hess,
-                    parallel,
-                    &mut growable,
-                );
-
-                let n_new_nodes = new_nodes.len();
-                if n_new_nodes == 0 {
-                    n_leaves += 1;
-                    self.nodes[n_idx] = node.as_leaf_node();
-                } else {
-                    self.nodes[n_idx] = node.as_parent_node();
-                    n_leaves += n_new_nodes;
-                    n_nodes += n_new_nodes;
-                    self.nodes.extend(new_nodes);
+            // For max_leaves, subtract 1 from the n_leaves
+            // every time we pop from the growable stack
+            // then, if we can add two children, add two to
+            // n_leaves. If we can't split the node any
+            // more, then just add 1 back to n_leaves
+            n_leaves -= 1;
+
+            let new_nodes = splitter.split_node(
+                &n_nodes, &mut node, &mut index, data, cuts, grad, hess, parallel,
+            );
+
+            let n_new_nodes = new_nodes.len();
+            if n_new_nodes == 0 {
+                n_leaves += 1;
+            } else {
+                self.nodes[n_idx].make_parent_node(node);
+                n_leaves += n_new_nodes;
+                n_nodes += n_new_nodes;
+                for n in new_nodes {
+                    self.nodes.push(n.as_node());
+                    growable.push_front(n)
                 }
             }
         }
     }
+    pub fn predict_contributions_row(
+        &self,
+        data: &Matrix<f64>,
+        row: usize,
+        contribs: &mut [f64],
+        weights: &[f64],
+    ) {
+        // Add the bias term first...
+        contribs[data.cols] += weights[0];
+        let mut node_idx = 0;
+        loop {
+            let node = &self.nodes[node_idx];
+            if node.is_leaf {
+                break;
+            }
+            // Get change of weight given child's weight.
+            let child_idx = node.get_child_idx(data.get(row, node.split_feature));
+            let node_weight = weights[node_idx];
+            let child_weight = weights[child_idx];
+            let delta = child_weight - node_weight;
+            contribs[node.split_feature] += delta;
+            node_idx = child_idx
+        }
+    }
+
+    fn predict_contributions_single_threaded(
+        &self,
+        data: &Matrix<f64>,
+        contribs: &mut [f64],
+        weights: &[f64],
+    ) {
+        // There needs to always be at least 2 trees
+        data.index
+            .iter()
+            .zip(contribs.chunks_mut(data.cols + 1))
+            .for_each(|(row, contribs)| {
+                self.predict_contributions_row(data, *row, contribs, weights)
+            })
+    }
+    fn predict_contributions_parallel(
+        &self,
+        data: &Matrix<f64>,
+        contribs: &mut [f64],
+        weights: &[f64],
+    ) {
+        // There needs to always be at least 2 trees
+        data.index
+            .par_iter()
+            .zip(contribs.par_chunks_mut(data.cols + 1))
+            .for_each(|(row, contribs)| {
+                self.predict_contributions_row(data, *row, contribs, weights)
+            })
+    }
+
+    pub fn predict_contributions(
+        &self,
+        data: &Matrix<f64>,
+        contribs: &mut [f64],
+        weights: &[f64],
+        parallel: bool,
+    ) {
+        if parallel {
+            self.predict_contributions_parallel(data, contribs, weights)
+        } else {
+            self.predict_contributions_single_threaded(data, contribs, weights)
+        }
+    }
 
-    pub fn predict_row(&self, data: &Matrix<f64>, row: usize) -> f64 {
+    fn predict_row(&self, data: &Matrix<f64>, row: usize) -> f64 {
         let mut node_idx = 0;
         loop {
-            let n = &self.nodes[node_idx];
-            match n {
-                TreeNode::Leaf(node) => {
-                    return node.weight_value as f64;
-                }
-                TreeNode::Parent(node) => {
-                    let v = data.get(row, node.split_feature);
-                    if v.is_nan() {
-                        node_idx = node.missing_node;
-                    } else if v < &node.split_value {
-                        node_idx = node.left_child;
-                    } else if v >= &node.split_value {
-                        node_idx = node.right_child;
-                    }
-                }
-                _ => unreachable!(),
+            let node = &self.nodes[node_idx];
+            if node.is_leaf {
+                return node.weight_value as f64;
+            } else {
+                node_idx = node.get_child_idx(data.get(row, node.split_feature));
             }
         }
     }
 
     fn predict_single_threaded(&self, data: &Matrix<f64>) -> Vec<f64> {
         data.index
             .iter()
@@ -176,53 +219,66 @@
             self.predict_single_threaded(data)
         }
     }
 
     pub fn value_partial_dependence(&self, feature: usize, value: f64) -> f64 {
         tree_partial_dependence(self, 0, feature, value, 1.0)
     }
+    fn distribute_node_leaf_weights(&self, i: usize, weights: &mut [f64]) -> f64 {
+        let node = &self.nodes[i];
+        let mut w = node.weight_value as f64;
+        if !node.is_leaf {
+            let left_node = &self.nodes[node.left_child];
+            let right_node = &self.nodes[node.right_child];
+            w = ((left_node.hessian_sum as f64
+                * self.distribute_node_leaf_weights(node.left_child, weights))
+                + (right_node.hessian_sum as f64
+                    * self.distribute_node_leaf_weights(node.right_child, weights)))
+                / (node.hessian_sum as f64);
+        }
+        weights[i] = w;
+        w
+    }
+    pub fn distribute_leaf_weights(&self) -> Vec<f64> {
+        let mut weights = vec![0.; self.nodes.len()];
+        self.distribute_node_leaf_weights(0, &mut weights);
+        weights
+    }
 }
 
 impl Display for Tree {
     // This trait requires `fmt` with this exact signature.
     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
         let mut print_buffer: Vec<usize> = vec![0];
         let mut r = String::new();
         while !print_buffer.is_empty() {
             // This will always be populated, because we confirm
             // that the buffer is not empty.
             let idx = print_buffer.pop().unwrap();
-            let n = &self.nodes[idx];
-            match n {
-                TreeNode::Leaf(node) => {
-                    r += format!("{}{}\n", "      ".repeat(node.depth).as_str(), n).as_str();
-                }
-                TreeNode::Parent(node) => {
-                    r += format!("{}{}\n", "      ".repeat(node.depth).as_str(), n).as_str();
-                    print_buffer.push(node.right_child);
-                    print_buffer.push(node.left_child);
-                }
-                TreeNode::Splittable(node) => {
-                    r += format!("{}{}\n", "      ".repeat(node.depth).as_str(), n).as_str();
-                    print_buffer.push(node.right_child);
-                    print_buffer.push(node.left_child);
-                }
+            let node = &self.nodes[idx];
+            if node.is_leaf {
+                r += format!("{}{}\n", "      ".repeat(node.depth).as_str(), node).as_str();
+            } else {
+                r += format!("{}{}\n", "      ".repeat(node.depth).as_str(), node).as_str();
+                print_buffer.push(node.right_child);
+                print_buffer.push(node.left_child);
             }
         }
         write!(f, "{}", r)
     }
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
     use crate::binning::bin_matrix;
     use crate::constraints::{Constraint, ConstraintMap};
     use crate::objective::{LogLoss, ObjectiveFunction};
     use crate::splitter::MissingImputerSplitter;
+    use crate::utils::precision_round;
     use std::fs;
     #[test]
     fn test_tree_fit() {
         let file = fs::read_to_string("resources/contiguous_no_missing.csv")
             .expect("Something went wrong reading the file");
         let data_vec: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
         let file = fs::read_to_string("resources/performance.csv")
@@ -245,18 +301,36 @@
         let mut tree = Tree::new();
 
         let b = bin_matrix(&data, &w, 300).unwrap();
         let bdata = Matrix::new(&b.binned_data, data.rows, data.cols);
 
         tree.fit(&bdata, &b.cuts, &g, &h, &splitter, usize::MAX, 5, true);
 
-        println!("{}", tree);
-        let preds = tree.predict(&data, false);
-        println!("{:?}", &preds[0..10]);
-        assert_eq!(25, tree.nodes.len())
+        // println!("{}", tree);
+        // let preds = tree.predict(&data, false);
+        // println!("{:?}", &preds[0..10]);
+        assert_eq!(25, tree.nodes.len());
+        // Test contributions prediction...
+        let weights = tree.distribute_leaf_weights();
+        let mut contribs = vec![0.; (data.cols + 1) * data.rows];
+        tree.predict_contributions(&data, &mut contribs, &weights, false);
+        let full_preds = tree.predict(&data, true);
+        assert_eq!(contribs.len(), (data.cols + 1) * data.rows);
+
+        let contribs_preds: Vec<f64> = contribs
+            .chunks(data.cols + 1)
+            .map(|i| i.iter().sum())
+            .collect();
+        println!("{:?}", &contribs[0..10]);
+        println!("{:?}", &contribs_preds[0..10]);
+
+        assert_eq!(contribs_preds.len(), full_preds.len());
+        for (i, j) in full_preds.iter().zip(contribs_preds) {
+            assert_eq!(precision_round(*i, 7), precision_round(j, 7));
+        }
     }
 
     #[test]
     fn test_tree_fit_monotone() {
         let file = fs::read_to_string("resources/contiguous_no_missing.csv")
             .expect("Something went wrong reading the file");
         let data_vec: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
@@ -291,9 +365,24 @@
         pred_data_vec.sort_by(|a, b| a.partial_cmp(b).unwrap());
         pred_data_vec.dedup();
         let pred_data = Matrix::new(&pred_data_vec, pred_data_vec.len(), 1);
 
         let preds = tree.predict(&pred_data, false);
         let increasing = preds.windows(2).all(|a| a[0] >= a[1]);
         assert!(increasing);
+
+        let weights = tree.distribute_leaf_weights();
+
+        let mut contribs = vec![0.; (data.cols + 1) * data.rows];
+        tree.predict_contributions(&data, &mut contribs, &weights, false);
+        let full_preds = tree.predict(&data, true);
+        assert_eq!(contribs.len(), (data.cols + 1) * data.rows);
+        let contribs_preds: Vec<f64> = contribs
+            .chunks(data.cols + 1)
+            .map(|i| i.iter().sum())
+            .collect();
+        assert_eq!(contribs_preds.len(), full_preds.len());
+        for (i, j) in full_preds.iter().zip(contribs_preds) {
+            assert_eq!(precision_round(*i, 7), precision_round(j, 7));
+        }
     }
 }
```

### Comparing `forust-0.2.0/local_dependencies/forust-ml/src/utils.rs` & `forust-0.2.1/local_dependencies/forust-ml/src/utils.rs`

 * *Files 1% similar despite different names*

```diff
@@ -351,22 +351,33 @@
             Ordering::Greater
         }
     } else {
         split_value.cmp(&cmp_value)
     }
 }
 
+#[inline]
+pub fn precision_round(n: f64, precision: i32) -> f64 {
+    let p = (10.0_f64).powi(precision);
+    (n * p).round() / p
+}
+
 #[cfg(test)]
 mod tests {
     use super::*;
     use rand::rngs::StdRng;
     use rand::seq::SliceRandom;
     use rand::Rng;
     use rand::SeedableRng;
     #[test]
+    fn test_round() {
+        assert_eq!(0.3, precision_round(0.3333, 1));
+        assert_eq!(0.2343, precision_round(0.2343123123123, 4));
+    }
+    #[test]
     fn test_percentiles() {
         let v = vec![4., 5., 6., 1., 2., 3., 7., 8., 9., 10.];
         let w = vec![1.; v.len()];
         let p = vec![0.3, 0.5, 0.75, 1.0];
         let p = percentiles(&v, &w, &p);
         assert_eq!(p, vec![3.0, 5.0, 8.0, 10.0]);
     }
```

### Comparing `forust-0.2.0/.gitignore` & `forust-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `forust-0.2.0/README.md` & `forust-0.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 The package can be installed directly from [pypi](https://pypi.org/project/forust/).
 ```shell
 pip install forust
 ```
 
 To use in a rust project add the following to your Cargo.toml file.
 ```toml
-forust-ml = "0.2.0"
+forust-ml = "0.2.1"
 ```
 
 ## Usage
 The `GradientBooster` class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
 
 It can be initialized with the following arguments.
 
@@ -80,14 +80,21 @@
 from forust import GradientBooster
 model = GradientBooster(objective_type="LogLoss")
 model.fit(X, y)
 
 # Predict on data
 model.predict(X.head())
 # array([-1.94919663,  2.25863229,  0.32963671,  2.48732194, -3.00371813])
+
+# predict contributions
+model.predict_contributions(X.head())
+# array([[-0.63014213,  0.33880048, -0.16520798, -0.07798772, -0.85083578,
+#        -1.07720813],
+#       [ 1.05406709,  0.08825999,  0.21662544, -0.12083538,  0.35209258,
+#        -1.07720813],
 ```
 
 The `fit` method accepts the following arguments.
  - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data.
  - `y` ***(ArrayLike)***: Either a pandas Series, or a 1 dimensional numpy array. If "LogLoss" was
    the objective type specified, then this should only contain 1 or 0 values, where 1 is the positive class being predicted. If "SquaredLoss" is the objective type, then any continuous variable can be
    provided.
@@ -98,14 +105,21 @@
 The predict method accepts the following arguments.
  - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data.
  - `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict
    function should run in parallel on multiple threads. If `None` is
    passed, the `parallel` attribute of the booster will be used.
    Defaults to `None`.
 
+The `predict_contributions` method will predict with the fitted booster on new data, returning the feature contribution matrix. The last column is the bias term.
+ - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data.
+ - `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict
+   function should run in parallel on multiple threads. If `None` is
+   passed, the `parallel` attribute of the booster will be used.
+   Defaults to `None`.
+
 ### Inspecting the Model
 
 Once the booster has been fit, each individual tree structure can be retrieved in text form, using the `text_dump` method. This method returns a list, the same length as the number of trees in the model.
 
 ```python
 model.text_dump()[0]
 # 0:[0 < 3] yes=1,no=2,missing=2,gain=91.50833,cover=209.388307
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
-to your Cargo.toml file. ```toml forust-ml = "0.2.0" ``` ## Usage The
+to your Cargo.toml file. ```toml forust-ml = "0.2.1" ``` ## Usage The
 `GradientBooster` class is currently the only public facing class in the
 package, and can be used to train gradient boosted decision tree ensembles with
 multiple objective functions. It can be initialized with the following
 arguments. - `objective_type` ***(str, optional)***: The name of objective
 function used to optimize. Valid options include "LogLoss" to use logistic loss
 as the objective function (binary classification), or "SquaredLoss" to use
 Squared Error as the objective function (continuous regression). Defaults to
@@ -66,31 +66,41 @@
 dataset. In the case of this example, the predictions are the log odds of a
 given record being 1. ```python # Small example dataset from seaborn import
 load_dataset df = load_dataset("titanic") X = df.select_dtypes("number").drop
 (columns=["survived"]) y = df["survived"] # Initialize a booster with defaults.
 from forust import GradientBooster model = GradientBooster
 (objective_type="LogLoss") model.fit(X, y) # Predict on data model.predict
 (X.head()) # array([-1.94919663, 2.25863229, 0.32963671, 2.48732194, -
-3.00371813]) ``` The `fit` method accepts the following arguments. - `X` ***
+3.00371813]) # predict contributions model.predict_contributions(X.head()) #
+array([[-0.63014213, 0.33880048, -0.16520798, -0.07798772, -0.85083578, # -
+1.07720813], # [ 1.05406709, 0.08825999, 0.21662544, -0.12083538, 0.35209258, #
+-1.07720813], ``` The `fit` method accepts the following arguments. - `X` ***
 (FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with
 numeric data. - `y` ***(ArrayLike)***: Either a pandas Series, or a 1
 dimensional numpy array. If "LogLoss" was the objective type specified, then
 this should only contain 1 or 0 values, where 1 is the positive class being
 predicted. If "SquaredLoss" is the objective type, then any continuous variable
 can be provided. - `sample_weight` ***(Optional[ArrayLike], optional)***:
 Instance weights to use when training the model. If None is passed, a weight of
 1 will be used for every record. Defaults to None. The predict method accepts
 the following arguments. - `X` ***(FrameLike)***: Either a pandas DataFrame, or
 a 2 dimensional numpy array, with numeric data. - `parallel` ***(Optional
 [bool], optional)***: Optionally specify if the predict function should run in
 parallel on multiple threads. If `None` is passed, the `parallel` attribute of
-the booster will be used. Defaults to `None`. ### Inspecting the Model Once the
-booster has been fit, each individual tree structure can be retrieved in text
-form, using the `text_dump` method. This method returns a list, the same length
-as the number of trees in the model. ```python model.text_dump()[0] # 0:[0 < 3]
+the booster will be used. Defaults to `None`. The `predict_contributions`
+method will predict with the fitted booster on new data, returning the feature
+contribution matrix. The last column is the bias term. - `X` ***(FrameLike)***:
+Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data. -
+`parallel` ***(Optional[bool], optional)***: Optionally specify if the predict
+function should run in parallel on multiple threads. If `None` is passed, the
+`parallel` attribute of the booster will be used. Defaults to `None`. ###
+Inspecting the Model Once the booster has been fit, each individual tree
+structure can be retrieved in text form, using the `text_dump` method. This
+method returns a list, the same length as the number of trees in the model.
+```python model.text_dump()[0] # 0:[0 < 3]
 yes=1,no=2,missing=2,gain=91.50833,cover=209.388307 # 1:[4 < 13.7917]
 yes=3,no=4,missing=4,gain=28.185467,cover=94.00148 # 3:[1 < 18]
 yes=7,no=8,missing=8,gain=1.4576768,cover=22.090348 # 7:[1 < 17]
 yes=15,no=16,missing=16,gain=0.691266,cover=0.705011 # 15:leaf=-
 0.15120,cover=0.23500 # 16:leaf=0.154097,cover=0.470007 ``` The `json_dump`
 method performs the same action, but returns the model as a json representation
 rather than a text string. To see an estimate for how a given feature is used
```

### Comparing `forust-0.2.0/forust/__init__.py` & `forust-0.2.1/forust/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,23 @@
         flat_data: np.ndarray,
         rows: int,
         cols: int,
         parallel: bool = True,
     ) -> np.ndarray:
         raise NotImplementedError()
 
+    def predict_contributions(
+        self,
+        flat_data: np.ndarray,
+        rows: int,
+        cols: int,
+        parallel: bool = True,
+    ) -> np.ndarray:
+        raise NotImplementedError
+
     def value_partial_dependence(
         self,
         feature: int,
         value: float,
     ) -> float:
         raise NotImplementedError()
 
@@ -234,14 +243,45 @@
         return self.booster.predict(
             flat_data=flat_data,
             rows=rows,
             cols=cols,
             parallel=parallel_,
         )
 
+    def predict_contributions(
+        self, X: FrameLike, parallel: Union[bool, None] = None
+    ) -> np.ndarray:
+        """Predict with the fitted booster on new data, returning the feature
+        contribution matrix. The last column is the bias term.
+
+        Args:
+            X (FrameLike): Either a pandas DataFrame, or a 2 dimensional numpy array.
+            parallel (Union[bool, None], optional): Optionally specify if the predict
+                function should run in parallel on multiple threads. If `None` is
+                passed, the `parallel` attribute of the booster will be used.
+                Defaults to `None`.
+
+        Returns:
+            np.ndarray: Returns a numpy array of the predictions.
+        """
+        X_ = X.to_numpy() if isinstance(X, pd.DataFrame) else X
+        if not np.issubdtype(X_.dtype, "float64"):
+            X_ = X_.astype(dtype="float64", copy=False)
+
+        parallel_ = self.parallel if parallel is None else parallel
+        flat_data = X_.ravel(order="F")
+        rows, cols = X_.shape
+        contributions = self.booster.predict_contributions(
+            flat_data=flat_data,
+            rows=rows,
+            cols=cols,
+            parallel=parallel_,
+        )
+        return np.reshape(contributions, (X_.shape[0], X_.shape[1] + 1))
+
     def partial_dependence(self, X: FrameLike, feature: Union[str, int]) -> np.ndarray:
         """Calculate the partial dependence values of a feature. For each unique
         value of the feature, this gives the estimate of the predicted value for that
         feature, with the effects of all features averaged out. This information gives
         an estimate of how a given feature impacts the model.
 
         Args:
```

### Comparing `forust-0.2.0/pyproject.toml` & `forust-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `forust-0.2.0/scratch.py` & `forust-0.2.1/scratch.py`

 * *Files identical despite different names*

### Comparing `forust-0.2.0/src/lib.rs` & `forust-0.2.1/src/lib.rs`

 * *Files 7% similar despite different names*

```diff
@@ -108,14 +108,30 @@
         parallel: Option<bool>,
     ) -> PyResult<&'py PyArray1<f64>> {
         let flat_data = flat_data.as_slice()?;
         let data = Matrix::new(flat_data, rows, cols);
         let parallel = parallel.unwrap_or(true);
         Ok(self.booster.predict(&data, parallel).into_pyarray(py))
     }
+    pub fn predict_contributions<'py>(
+        &self,
+        py: Python<'py>,
+        flat_data: PyReadonlyArray1<f64>,
+        rows: usize,
+        cols: usize,
+        parallel: Option<bool>,
+    ) -> PyResult<&'py PyArray1<f64>> {
+        let flat_data = flat_data.as_slice()?;
+        let data = Matrix::new(flat_data, rows, cols);
+        let parallel = parallel.unwrap_or(true);
+        Ok(self
+            .booster
+            .predict_contributions(&data, parallel)
+            .into_pyarray(py))
+    }
 
     pub fn value_partial_dependence(&self, feature: usize, value: f64) -> PyResult<f64> {
         Ok(self.booster.value_partial_dependence(feature, value))
     }
 
     pub fn text_dump(&self) -> PyResult<Vec<String>> {
         let mut trees = Vec::new();
```

### Comparing `forust-0.2.0/tests/test_booster.py` & `forust-0.2.1/tests/test_booster.py`

 * *Files 9% similar despite different names*

```diff
@@ -259,7 +259,53 @@
     for f, m in mono_.items():
         p_d = fmod.partial_dependence(X, feature=f)
         p_d = p_d[~np.isnan(p_d[:, 0])]
         if m < 0:
             assert np.all(p_d[0:-1, 1] >= p_d[1:, 1])
         else:
             assert np.all(p_d[0:-1, 1] <= p_d[1:, 1])
+
+
+def test_booster_to_xgboosts_with_contributions(X_y):
+    X, y = X_y
+    X = X
+    fmod = GradientBooster(
+        iterations=100,
+        learning_rate=0.3,
+        max_depth=5,
+        l2=1,
+        min_leaf_weight=1,
+        gamma=1,
+        objective_type="LogLoss",
+        nbins=500,
+        parallel=False,
+        base_score=0.0,
+    )
+    fmod.fit(X, y=y)
+    fmod_preds = fmod.predict(X)
+    fmod_contribs = fmod.predict_contributions(X)
+    fmod_preds[~np.isclose(fmod_contribs.sum(1), fmod_preds, rtol=5)]
+    fmod_contribs.sum(1)[~np.isclose(fmod_contribs.sum(1), fmod_preds, rtol=5)]
+    assert fmod_contribs.shape[1] == X.shape[1] + 1
+    assert np.allclose(fmod_contribs.sum(1), fmod_preds)
+
+    xmod = XGBClassifier(
+        n_estimators=100,
+        learning_rate=0.3,
+        max_depth=5,
+        reg_lambda=1,
+        min_child_weight=1,
+        gamma=1,
+        objective="binary:logitraw",
+        eval_metric="auc",
+        tree_method="hist",
+        max_bin=10000,
+        base_score=0.0,
+    )
+    xmod.fit(X, y)
+    xmod_preds = xmod.predict(X, output_margin=True)
+    import xgboost as xgb
+
+    xmod_contribs = xmod.get_booster().predict(
+        xgb.DMatrix(X), approx_contribs=True, pred_contribs=True
+    )
+    assert np.allclose(fmod_contribs, xmod_contribs, atol=0.000001)
```

### Comparing `forust-0.2.0/LICENSE` & `forust-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `forust-0.2.0/PKG-INFO` & `forust-0.2.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forust
-Version: 0.2.0
+Version: 0.2.1
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
-forust-ml = "0.2.0"
+forust-ml = "0.2.1"
 ```
 
 ## Usage
 The `GradientBooster` class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
 
 It can be initialized with the following arguments.
 
@@ -101,14 +101,21 @@
 from forust import GradientBooster
 model = GradientBooster(objective_type="LogLoss")
 model.fit(X, y)
 
 # Predict on data
 model.predict(X.head())
 # array([-1.94919663,  2.25863229,  0.32963671,  2.48732194, -3.00371813])
+
+# predict contributions
+model.predict_contributions(X.head())
+# array([[-0.63014213,  0.33880048, -0.16520798, -0.07798772, -0.85083578,
+#        -1.07720813],
+#       [ 1.05406709,  0.08825999,  0.21662544, -0.12083538,  0.35209258,
+#        -1.07720813],
 ```
 
 The `fit` method accepts the following arguments.
  - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data.
  - `y` ***(ArrayLike)***: Either a pandas Series, or a 1 dimensional numpy array. If "LogLoss" was
    the objective type specified, then this should only contain 1 or 0 values, where 1 is the positive class being predicted. If "SquaredLoss" is the objective type, then any continuous variable can be
    provided.
@@ -119,14 +126,21 @@
 The predict method accepts the following arguments.
  - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data.
  - `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict
    function should run in parallel on multiple threads. If `None` is
    passed, the `parallel` attribute of the booster will be used.
    Defaults to `None`.
 
+The `predict_contributions` method will predict with the fitted booster on new data, returning the feature contribution matrix. The last column is the bias term.
+ - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data.
+ - `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict
+   function should run in parallel on multiple threads. If `None` is
+   passed, the `parallel` attribute of the booster will be used.
+   Defaults to `None`.
+
 ### Inspecting the Model
 
 Once the booster has been fit, each individual tree structure can be retrieved in text form, using the `text_dump` method. This method returns a list, the same length as the number of trees in the model.
 
 ```python
 model.text_dump()[0]
 # 0:[0 < 3] yes=1,no=2,missing=2,gain=91.50833,cover=209.388307
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: forust Version: 0.2.0 Classifier: Programming
+Metadata-Version: 2.1 Name: forust Version: 0.2.1 Classifier: Programming
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
-to your Cargo.toml file. ```toml forust-ml = "0.2.0" ``` ## Usage The
+to your Cargo.toml file. ```toml forust-ml = "0.2.1" ``` ## Usage The
 `GradientBooster` class is currently the only public facing class in the
 package, and can be used to train gradient boosted decision tree ensembles with
 multiple objective functions. It can be initialized with the following
 arguments. - `objective_type` ***(str, optional)***: The name of objective
 function used to optimize. Valid options include "LogLoss" to use logistic loss
 as the objective function (binary classification), or "SquaredLoss" to use
 Squared Error as the objective function (continuous regression). Defaults to
@@ -77,31 +77,41 @@
 dataset. In the case of this example, the predictions are the log odds of a
 given record being 1. ```python # Small example dataset from seaborn import
 load_dataset df = load_dataset("titanic") X = df.select_dtypes("number").drop
 (columns=["survived"]) y = df["survived"] # Initialize a booster with defaults.
 from forust import GradientBooster model = GradientBooster
 (objective_type="LogLoss") model.fit(X, y) # Predict on data model.predict
 (X.head()) # array([-1.94919663, 2.25863229, 0.32963671, 2.48732194, -
-3.00371813]) ``` The `fit` method accepts the following arguments. - `X` ***
+3.00371813]) # predict contributions model.predict_contributions(X.head()) #
+array([[-0.63014213, 0.33880048, -0.16520798, -0.07798772, -0.85083578, # -
+1.07720813], # [ 1.05406709, 0.08825999, 0.21662544, -0.12083538, 0.35209258, #
+-1.07720813], ``` The `fit` method accepts the following arguments. - `X` ***
 (FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with
 numeric data. - `y` ***(ArrayLike)***: Either a pandas Series, or a 1
 dimensional numpy array. If "LogLoss" was the objective type specified, then
 this should only contain 1 or 0 values, where 1 is the positive class being
 predicted. If "SquaredLoss" is the objective type, then any continuous variable
 can be provided. - `sample_weight` ***(Optional[ArrayLike], optional)***:
 Instance weights to use when training the model. If None is passed, a weight of
 1 will be used for every record. Defaults to None. The predict method accepts
 the following arguments. - `X` ***(FrameLike)***: Either a pandas DataFrame, or
 a 2 dimensional numpy array, with numeric data. - `parallel` ***(Optional
 [bool], optional)***: Optionally specify if the predict function should run in
 parallel on multiple threads. If `None` is passed, the `parallel` attribute of
-the booster will be used. Defaults to `None`. ### Inspecting the Model Once the
-booster has been fit, each individual tree structure can be retrieved in text
-form, using the `text_dump` method. This method returns a list, the same length
-as the number of trees in the model. ```python model.text_dump()[0] # 0:[0 < 3]
+the booster will be used. Defaults to `None`. The `predict_contributions`
+method will predict with the fitted booster on new data, returning the feature
+contribution matrix. The last column is the bias term. - `X` ***(FrameLike)***:
+Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data. -
+`parallel` ***(Optional[bool], optional)***: Optionally specify if the predict
+function should run in parallel on multiple threads. If `None` is passed, the
+`parallel` attribute of the booster will be used. Defaults to `None`. ###
+Inspecting the Model Once the booster has been fit, each individual tree
+structure can be retrieved in text form, using the `text_dump` method. This
+method returns a list, the same length as the number of trees in the model.
+```python model.text_dump()[0] # 0:[0 < 3]
 yes=1,no=2,missing=2,gain=91.50833,cover=209.388307 # 1:[4 < 13.7917]
 yes=3,no=4,missing=4,gain=28.185467,cover=94.00148 # 3:[1 < 18]
 yes=7,no=8,missing=8,gain=1.4576768,cover=22.090348 # 7:[1 < 17]
 yes=15,no=16,missing=16,gain=0.691266,cover=0.705011 # 15:leaf=-
 0.15120,cover=0.23500 # 16:leaf=0.154097,cover=0.470007 ``` The `json_dump`
 method performs the same action, but returns the model as a json representation
 rather than a text string. To see an estimate for how a given feature is used
```

