# Comparing `tmp/doubt-4.3.1.tar.gz` & `tmp/doubt-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doubt-4.3.1.tar", max compression
+gzip compressed data, was "doubt-4.4.0.tar", max compression
```

## Comparing `doubt-4.3.1.tar` & `doubt-4.4.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1056 2022-07-17 15:34:56.352960 doubt-4.3.1/LICENSE
--rw-r--r--   0        0        0     2583 2023-03-20 18:25:20.177518 doubt-4.3.1/README.md
--rw-r--r--   0        0        0     1338 2023-03-20 18:37:11.304481 doubt-4.3.1/pyproject.toml
--rw-r--r--   0        0        0      372 2022-07-17 15:34:56.355332 doubt-4.3.1/src/doubt/__init__.py
--rw-r--r--   0        0        0     1082 2022-07-17 15:34:56.355574 doubt-4.3.1/src/doubt/datasets/__init__.py
--rw-r--r--   0        0        0     2510 2022-07-17 15:34:56.355799 doubt-4.3.1/src/doubt/datasets/airfoil.py
--rw-r--r--   0        0        0     4903 2022-07-17 15:34:56.356034 doubt-4.3.1/src/doubt/datasets/bike_sharing_daily.py
--rw-r--r--   0        0        0     4995 2022-07-17 15:34:56.356216 doubt-4.3.1/src/doubt/datasets/bike_sharing_hourly.py
--rw-r--r--   0        0        0     5661 2022-07-17 15:34:56.356397 doubt-4.3.1/src/doubt/datasets/blog.py
--rw-r--r--   0        0        0     2808 2022-07-17 15:34:56.356560 doubt-4.3.1/src/doubt/datasets/concrete.py
--rw-r--r--   0        0        0     2846 2022-07-17 15:34:56.356716 doubt-4.3.1/src/doubt/datasets/cpu.py
--rw-r--r--   0        0        0     4226 2022-07-17 15:34:56.356886 doubt-4.3.1/src/doubt/datasets/dataset.py
--rw-r--r--   0        0        0     5653 2022-07-17 15:34:56.357060 doubt-4.3.1/src/doubt/datasets/facebook_comments.py
--rw-r--r--   0        0        0     4629 2022-07-17 15:34:56.357231 doubt-4.3.1/src/doubt/datasets/facebook_metrics.py
--rw-r--r--   0        0        0     5825 2022-07-17 15:34:56.357435 doubt-4.3.1/src/doubt/datasets/fish_bioconcentration.py
--rw-r--r--   0        0        0     2857 2022-07-17 15:34:56.357617 doubt-4.3.1/src/doubt/datasets/fish_toxicity.py
--rw-r--r--   0        0        0     3924 2022-07-17 15:34:56.357779 doubt-4.3.1/src/doubt/datasets/forest_fire.py
--rw-r--r--   0        0        0     6646 2022-07-17 15:34:56.357967 doubt-4.3.1/src/doubt/datasets/gas_turbine.py
--rw-r--r--   0        0        0     4273 2022-07-17 15:34:56.358157 doubt-4.3.1/src/doubt/datasets/nanotube.py
--rw-r--r--   0        0        0     2950 2022-07-17 15:34:56.358328 doubt-4.3.1/src/doubt/datasets/new_taipei_housing.py
--rw-r--r--   0        0        0     4667 2022-07-17 15:34:56.358499 doubt-4.3.1/src/doubt/datasets/parkinsons.py
--rw-r--r--   0        0        0     3786 2022-07-17 15:34:56.358663 doubt-4.3.1/src/doubt/datasets/power_plant.py
--rw-r--r--   0        0        0     2857 2022-07-17 15:34:56.358822 doubt-4.3.1/src/doubt/datasets/protein.py
--rw-r--r--   0        0        0     3421 2022-07-17 15:34:56.359001 doubt-4.3.1/src/doubt/datasets/servo.py
--rw-r--r--   0        0        0     4743 2022-07-17 15:34:56.359172 doubt-4.3.1/src/doubt/datasets/solar_flare.py
--rw-r--r--   0        0        0     4463 2022-07-17 15:34:56.359375 doubt-4.3.1/src/doubt/datasets/space_shuttle.py
--rw-r--r--   0        0        0     5313 2022-07-17 15:34:56.359607 doubt-4.3.1/src/doubt/datasets/stocks.py
--rw-r--r--   0        0        0     5421 2022-07-17 15:34:56.359788 doubt-4.3.1/src/doubt/datasets/superconductivity.py
--rw-r--r--   0        0        0     3351 2022-07-17 15:34:56.360044 doubt-4.3.1/src/doubt/datasets/tehran_housing.py
--rw-r--r--   0        0        0     3357 2022-07-17 15:34:56.360230 doubt-4.3.1/src/doubt/datasets/yacht.py
--rw-r--r--   0        0        0      174 2022-07-17 15:34:56.360496 doubt-4.3.1/src/doubt/models/__init__.py
--rw-r--r--   0        0        0       31 2022-07-17 15:34:56.360777 doubt-4.3.1/src/doubt/models/boot/__init__.py
--rw-r--r--   0        0        0    14958 2022-07-17 17:03:47.690418 doubt-4.3.1/src/doubt/models/boot/boot.py
--rw-r--r--   0        0        0       58 2022-07-17 15:34:56.361181 doubt-4.3.1/src/doubt/models/glm/__init__.py
--rw-r--r--   0        0        0     2235 2022-07-17 15:34:56.361351 doubt-4.3.1/src/doubt/models/glm/quantile_loss.py
--rw-r--r--   0        0        0     9222 2022-07-17 17:10:39.834206 doubt-4.3.1/src/doubt/models/glm/quantile_regressor.py
--rw-r--r--   0        0        0      495 2022-07-17 15:34:56.361782 doubt-4.3.1/src/doubt/models/model.py
--rw-r--r--   0        0        0      102 2022-07-17 15:34:56.361953 doubt-4.3.1/src/doubt/models/tree/__init__.py
--rw-r--r--   0        0        0    13354 2023-03-20 18:32:48.084709 doubt-4.3.1/src/doubt/models/tree/forest.py
--rw-r--r--   0        0        0    10540 2023-03-20 18:33:10.883879 doubt-4.3.1/src/doubt/models/tree/tree.py
--rw-r--r--   0        0        0     3821 2022-07-17 15:34:56.362536 doubt-4.3.1/src/doubt/models/tree/utils.py
--rw-r--r--   0        0        0     3667 1970-01-01 00:00:00.000000 doubt-4.3.1/setup.py
--rw-r--r--   0        0        0     3515 1970-01-01 00:00:00.000000 doubt-4.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1056 2022-07-17 15:34:56.352960 doubt-4.4.0/LICENSE
+-rw-r--r--   0        0        0     2583 2023-03-20 18:25:20.177518 doubt-4.4.0/README.md
+-rw-r--r--   0        0        0     1310 2023-04-23 18:26:13.875394 doubt-4.4.0/pyproject.toml
+-rw-r--r--   0        0        0      369 2023-03-20 19:12:08.029301 doubt-4.4.0/src/doubt/__init__.py
+-rw-r--r--   0        0        0     1082 2022-07-17 15:34:56.355574 doubt-4.4.0/src/doubt/datasets/__init__.py
+-rw-r--r--   0        0        0     2510 2022-07-17 15:34:56.355799 doubt-4.4.0/src/doubt/datasets/airfoil.py
+-rw-r--r--   0        0        0     4903 2022-07-17 15:34:56.356034 doubt-4.4.0/src/doubt/datasets/bike_sharing_daily.py
+-rw-r--r--   0        0        0     4995 2022-07-17 15:34:56.356216 doubt-4.4.0/src/doubt/datasets/bike_sharing_hourly.py
+-rw-r--r--   0        0        0     5661 2022-07-17 15:34:56.356397 doubt-4.4.0/src/doubt/datasets/blog.py
+-rw-r--r--   0        0        0     2808 2022-07-17 15:34:56.356560 doubt-4.4.0/src/doubt/datasets/concrete.py
+-rw-r--r--   0        0        0     2846 2022-07-17 15:34:56.356716 doubt-4.4.0/src/doubt/datasets/cpu.py
+-rw-r--r--   0        0        0     4225 2023-03-20 18:57:45.250733 doubt-4.4.0/src/doubt/datasets/dataset.py
+-rw-r--r--   0        0        0     5653 2022-07-17 15:34:56.357060 doubt-4.4.0/src/doubt/datasets/facebook_comments.py
+-rw-r--r--   0        0        0     4629 2022-07-17 15:34:56.357231 doubt-4.4.0/src/doubt/datasets/facebook_metrics.py
+-rw-r--r--   0        0        0     5825 2022-07-17 15:34:56.357435 doubt-4.4.0/src/doubt/datasets/fish_bioconcentration.py
+-rw-r--r--   0        0        0     2857 2022-07-17 15:34:56.357617 doubt-4.4.0/src/doubt/datasets/fish_toxicity.py
+-rw-r--r--   0        0        0     3924 2022-07-17 15:34:56.357779 doubt-4.4.0/src/doubt/datasets/forest_fire.py
+-rw-r--r--   0        0        0     6646 2022-07-17 15:34:56.357967 doubt-4.4.0/src/doubt/datasets/gas_turbine.py
+-rw-r--r--   0        0        0     4273 2022-07-17 15:34:56.358157 doubt-4.4.0/src/doubt/datasets/nanotube.py
+-rw-r--r--   0        0        0     2950 2022-07-17 15:34:56.358328 doubt-4.4.0/src/doubt/datasets/new_taipei_housing.py
+-rw-r--r--   0        0        0     4667 2022-07-17 15:34:56.358499 doubt-4.4.0/src/doubt/datasets/parkinsons.py
+-rw-r--r--   0        0        0     3786 2022-07-17 15:34:56.358663 doubt-4.4.0/src/doubt/datasets/power_plant.py
+-rw-r--r--   0        0        0     2857 2022-07-17 15:34:56.358822 doubt-4.4.0/src/doubt/datasets/protein.py
+-rw-r--r--   0        0        0     3421 2022-07-17 15:34:56.359001 doubt-4.4.0/src/doubt/datasets/servo.py
+-rw-r--r--   0        0        0     4743 2022-07-17 15:34:56.359172 doubt-4.4.0/src/doubt/datasets/solar_flare.py
+-rw-r--r--   0        0        0     4463 2022-07-17 15:34:56.359375 doubt-4.4.0/src/doubt/datasets/space_shuttle.py
+-rw-r--r--   0        0        0     5313 2022-07-17 15:34:56.359607 doubt-4.4.0/src/doubt/datasets/stocks.py
+-rw-r--r--   0        0        0     5421 2022-07-17 15:34:56.359788 doubt-4.4.0/src/doubt/datasets/superconductivity.py
+-rw-r--r--   0        0        0     3351 2022-07-17 15:34:56.360044 doubt-4.4.0/src/doubt/datasets/tehran_housing.py
+-rw-r--r--   0        0        0     3357 2022-07-17 15:34:56.360230 doubt-4.4.0/src/doubt/datasets/yacht.py
+-rw-r--r--   0        0        0      174 2022-07-17 15:34:56.360496 doubt-4.4.0/src/doubt/models/__init__.py
+-rw-r--r--   0        0        0       31 2022-07-17 15:34:56.360777 doubt-4.4.0/src/doubt/models/boot/__init__.py
+-rw-r--r--   0        0        0    16835 2023-04-23 18:24:53.138955 doubt-4.4.0/src/doubt/models/boot/boot.py
+-rw-r--r--   0        0        0       58 2022-07-17 15:34:56.361181 doubt-4.4.0/src/doubt/models/glm/__init__.py
+-rw-r--r--   0        0        0     2235 2022-07-17 15:34:56.361351 doubt-4.4.0/src/doubt/models/glm/quantile_loss.py
+-rw-r--r--   0        0        0     9220 2023-03-20 18:57:45.276816 doubt-4.4.0/src/doubt/models/glm/quantile_regressor.py
+-rw-r--r--   0        0        0      495 2022-07-17 15:34:56.361782 doubt-4.4.0/src/doubt/models/model.py
+-rw-r--r--   0        0        0      102 2022-07-17 15:34:56.361953 doubt-4.4.0/src/doubt/models/tree/__init__.py
+-rw-r--r--   0        0        0    13354 2023-03-20 18:32:48.084709 doubt-4.4.0/src/doubt/models/tree/forest.py
+-rw-r--r--   0        0        0    10540 2023-03-20 18:33:10.883879 doubt-4.4.0/src/doubt/models/tree/tree.py
+-rw-r--r--   0        0        0     3821 2022-07-17 15:34:56.362536 doubt-4.4.0/src/doubt/models/tree/utils.py
+-rw-r--r--   0        0        0     3667 1970-01-01 00:00:00.000000 doubt-4.4.0/setup.py
+-rw-r--r--   0        0        0     3515 1970-01-01 00:00:00.000000 doubt-4.4.0/PKG-INFO
```

### Comparing `doubt-4.3.1/LICENSE` & `doubt-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `doubt-4.3.1/README.md` & `doubt-4.4.0/README.md`

 * *Files identical despite different names*

### Comparing `doubt-4.3.1/pyproject.toml` & `doubt-4.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "doubt"
-version = "4.3.1"
+version = "4.4.0"
 description = "Bringing back uncertainty to machine learning."
 authors = ["Dan Saattrup Nielsen <saattrupdan@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/saattrupdan/doubt"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
 tqdm = "^4.62.0"
 numpy = "^1.23.0"
 pandas = "^1.4.0"
-joblib = "^1.1.0"
+joblib = "^1.2.0"
 scikit-learn = "^1.1.1"
 tables = "^3.7.0"
 xlrd = "^2.0.1"
 openpyxl = "^3.0.10"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pdoc = "^7.1.1"
-pytest = "^6.2.5"
 pre-commit = "^2.17.0"
-black = {extras = ["jupyter"], version = "^22.3.0"}
+black = "^23.1.0"
 requests = "^2.28.0"
 lxml = "^4.9.0"
 isort = "^5.10.1"
 pytest-xdist = "^2.5.0"
-pytest-cov = "^3.0.0"
 readme-coverage-badger = ">=0.1.2,<1.0.0"
 Pygments = "2.11"
+pytest = "^7.2.2"
+pytest-cov = "^4.0.0"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = [
     '--verbose',
     '--durations=10',
     '--color=yes',
```

### Comparing `doubt-4.3.1/src/doubt/datasets/__init__.py` & `doubt-4.4.0/src/doubt/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `doubt-4.3.1/src/doubt/datasets/airfoil.py` & `doubt-4.4.0/src/doubt/datasets/airfoil.py`

 * *Files identical despite different names*

### Comparing `doubt-4.3.1/src/doubt/datasets/bike_sharing_daily.py` & `doubt-4.4.0/src/doubt/datasets/bike_sharing_daily.py`

 * *Files identical despite different names*

### Comparing `doubt-4.3.1/src/doubt/datasets/bike_sharing_hourly.py` & `doubt-4.4.0/src/doubt/datasets/bike_sharing_hourly.py`

 * *Files identical despite different names*

### Comparing `doubt-4.3.1/src/doubt/datasets/blog.py` & `doubt-4.4.0/src/doubt/datasets/blog.py`

 * *Files identical despite different names*

### Comparing `doubt-4.3.1/src/doubt/datasets/concrete.py` & `doubt-4.4.0/src/doubt/datasets/concrete.py`

 * *Files identical despite different names*

### Comparing `doubt-4.3.1/src/doubt/datasets/cpu.py` & `doubt-4.4.0/src/doubt/datasets/cpu.py`

 * *Files identical despite different names*

### Comparing `doubt-4.3.1/src/doubt/datasets/dataset.py` & `doubt-4.4.0/src/doubt/datasets/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
             Dimensions of the data set
         columns (list of strings):
             List of column names in the data set
 """
 
 
 class BaseDataset(ABC):
-
     _url: str
     _features: Iterable
     _targets: Iterable
 
     def __init__(self, cache: Optional[str] = ".dataset_cache"):
         self.cache = cache
         self._data = self.get_data()
```

### Comparing `doubt-4.3.1/src/doubt/datasets/facebook_comments.py` & `doubt-4.4.0/src/doubt/datasets/facebook_comments.py`

 * *Files identical despite different names*

### Comparing `doubt-4.3.1/src/doubt/datasets/facebook_metrics.py` & `doubt-4.4.0/src/doubt/datasets/facebook_metrics.py`

 * *Files identical despite different names*

### Comparing `doubt-4.3.1/src/doubt/datasets/fish_bioconcentration.py` & `doubt-4.4.0/src/doubt/datasets/fish_bioconcentration.py`

 * *Files identical despite different names*

### Comparing `doubt-4.3.1/src/doubt/datasets/fish_toxicity.py` & `doubt-4.4.0/src/doubt/datasets/fish_toxicity.py`

 * *Files identical despite different names*

### Comparing `doubt-4.3.1/src/doubt/datasets/forest_fire.py` & `doubt-4.4.0/src/doubt/datasets/forest_fire.py`

 * *Files identical despite different names*

### Comparing `doubt-4.3.1/src/doubt/datasets/gas_turbine.py` & `doubt-4.4.0/src/doubt/datasets/gas_turbine.py`

 * *Files identical despite different names*

### Comparing `doubt-4.3.1/src/doubt/datasets/nanotube.py` & `doubt-4.4.0/src/doubt/datasets/nanotube.py`

 * *Files identical despite different names*

### Comparing `doubt-4.3.1/src/doubt/datasets/new_taipei_housing.py` & `doubt-4.4.0/src/doubt/datasets/new_taipei_housing.py`

 * *Files identical despite different names*

### Comparing `doubt-4.3.1/src/doubt/datasets/parkinsons.py` & `doubt-4.4.0/src/doubt/datasets/parkinsons.py`

 * *Files identical despite different names*

### Comparing `doubt-4.3.1/src/doubt/datasets/power_plant.py` & `doubt-4.4.0/src/doubt/datasets/power_plant.py`

 * *Files identical despite different names*

### Comparing `doubt-4.3.1/src/doubt/datasets/protein.py` & `doubt-4.4.0/src/doubt/datasets/protein.py`

 * *Files identical despite different names*

### Comparing `doubt-4.3.1/src/doubt/datasets/servo.py` & `doubt-4.4.0/src/doubt/datasets/servo.py`

 * *Files identical despite different names*

### Comparing `doubt-4.3.1/src/doubt/datasets/solar_flare.py` & `doubt-4.4.0/src/doubt/datasets/solar_flare.py`

 * *Files identical despite different names*

### Comparing `doubt-4.3.1/src/doubt/datasets/space_shuttle.py` & `doubt-4.4.0/src/doubt/datasets/space_shuttle.py`

 * *Files identical despite different names*

### Comparing `doubt-4.3.1/src/doubt/datasets/stocks.py` & `doubt-4.4.0/src/doubt/datasets/stocks.py`

 * *Files identical despite different names*

### Comparing `doubt-4.3.1/src/doubt/datasets/superconductivity.py` & `doubt-4.4.0/src/doubt/datasets/superconductivity.py`

 * *Files identical despite different names*

### Comparing `doubt-4.3.1/src/doubt/datasets/tehran_housing.py` & `doubt-4.4.0/src/doubt/datasets/tehran_housing.py`

 * *Files identical despite different names*

### Comparing `doubt-4.3.1/src/doubt/datasets/yacht.py` & `doubt-4.4.0/src/doubt/datasets/yacht.py`

 * *Files identical despite different names*

### Comparing `doubt-4.3.1/src/doubt/models/boot/boot.py` & `doubt-4.4.0/src/doubt/models/boot/boot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Bootstrap wrapper for datasets and models"""
 
 import copy
 import multiprocessing as mp
 from types import MethodType
-from typing import Callable, Optional, Tuple, Union
+from typing import Callable, List, Optional, Tuple, Union
 
 import numpy as np
 from joblib import Parallel, delayed
+from numpy.typing import NDArray
 
 
 class Boot:
     """Bootstrap wrapper for datasets and models.
 
     Datasets can be any sequence of numeric input, from which bootstrapped statistics
     can be calculated, with confidence intervals included.
@@ -44,17 +45,15 @@
             4.06
             >>> np.around(intervals, 2)
             array([3.98, 4.17])
 
         Alternatively, we can output the whole bootstrap distribution::
 
             >>> preds, intervals = boot.compute_statistic(
-            ...     np.mean,
-            ...     n_boots=3,
-            ...     return_all=True
+            ...     np.mean, n_boots=3, return_all=True
             ... )
             >>> round(preds, 2)
             4.06
             >>> np.around(intervals, 2)
             array([4.06, 4.06, 4.06])
 
         Wrap a scikit-learn model and get prediction intervals::
@@ -65,14 +64,32 @@
             >>> linreg = linreg.fit(X, y)
             >>> preds, intervals = linreg.predict([10, 30, 1000, 50], uncertainty=0.05)
             >>> round(preds, 2)
             482.0
             >>> np.around(intervals, 2)
             array([473.5 , 490.14])
 
+        Instead of specifying the uncertainty, we can also specify the precise
+        quantiles that we are interested in::
+
+            >>> preds, intervals = linreg.predict(
+            ...     [10, 30, 1000, 50], quantiles=[0.1, 0.5]
+            ... )
+            >>> np.around(intervals, 2)
+            array([476.45, 481.82])
+
+        Lastly, as with the `compute_statistic` method, we can also output the whole
+        bootstrap distribution with the `return_all` argument::
+
+            >>> preds, bootstrap_samples = linreg.predict(
+            ...     [10, 30, 1000, 50], return_all=True
+            ... )
+            >>> np.around(bootstrap_samples, 2)
+            array([-43.7 , -10.02,  -8.63, ...,   8.28,   9.06,  10.19])
+
     Sources:
         [1]: Friedman, J., Hastie, T., & Tibshirani, R. (2001). The elements of
              statistical learning (Vol. 1, No. 10). New York: Springer series in
              statistics.
         [2]: Kumar, S., & Srivistava, A. N. (2012). Bootstrap prediction intervals in
              non-parametric regression with applications to anomaly detection.
         [3]: https://saattrupdan.github.io/2020-03-01-bootstrap-prediction
@@ -140,15 +157,15 @@
 
 
 def compute_statistic(
     self,
     statistic: Callable[[np.ndarray], float],
     n_boots: Optional[int] = None,
     uncertainty: float = 0.05,
-    quantiles: Optional[np.ndarray] = None,
+    quantiles: Optional[Union[np.ndarray, List[float]]] = None,
     return_all: bool = False,
 ) -> Union[float, Tuple[float, np.ndarray]]:
     """Compute bootstrapped statistic.
 
     Args:
         statistic (callable):
             The statistic to be computed on bootstrapped samples.
@@ -206,38 +223,43 @@
 
 
 def predict(
     self,
     X: np.ndarray,
     n_boots: Optional[int] = None,
     uncertainty: Optional[float] = None,
-    quantiles: Optional[np.ndarray] = None,
-) -> Tuple[Union[float, np.ndarray], np.ndarray]:
+    quantiles: Optional[Union[np.ndarray, List[float]]] = None,
+    return_all: bool = False,
+) -> Union[Union[float, NDArray], Tuple[Union[float, NDArray], NDArray]]:
     """Compute bootstrapped predictions.
 
     Args:
         X (float array):
             The array containing the data set, either of shape (f,) or (n, f), with n
             being the number of samples and f being the number of features.
         n_boots (int or None, optional):
             The number of resamples to bootstrap. If None then it is set to the square
             root of the data set. Defaults to None
         uncertainty (float or None, optional):
             The uncertainty used to compute the prediction interval of the bootstrapped
-            prediction. If None then no prediction intervals are returned. Defaults to
-            None.
+            prediction. For instance, an uncertainty of 0.05 will yield a 95%
+            prediction interval. Will not be used if `quantiles` or `return_all` is
+            used. Defaults to None.
         quantiles (sequence of floats or None, optional):
-            List of quantiles to output, as an alternative to the `uncertainty`
-            argument, and will not be used if that argument is set. If None then
-            `uncertainty` is used. Defaults to None.
+            List of quantiles to output. Will override the value of `uncertainty` if
+            specified. Will not be used if `return_all` is True. Defaults to None.
+        return_all (bool, optional):
+            Whether the raw bootstrapped predictions should be returned. Will override
+            the values of both `quantiles` and `uncertainty`. Defaults to False.
 
     Returns:
         float array or pair of float arrays:
             The bootstrapped predictions, and the confidence intervals if `uncertainty`
-            is not None, or the specified quantiles if `quantiles` is not None.
+            is not None, the specified quantiles if `quantiles` is not None, or the raw
+            bootstrapped values if `return_all` is True.
     """
     # Initialise random number generator
     rng = np.random.default_rng(self.random_seed)
 
     # Ensure that input feature matrix is a Numpy array
     X = np.asarray(X)
 
@@ -248,23 +270,23 @@
         X = np.expand_dims(X, 0)
 
     # Get the full non-bootstrapped predictions of `X`
     preds = self._model(X) if callable(self._model) else self._model.predict(X)
 
     # If no quantiles should be outputted then simply return the predictions of the
     # underlying model
-    if uncertainty is None and quantiles is None:
+    if uncertainty is None and quantiles is None and not return_all:
         return preds
 
     # Ensure that the underlying model has been fitted before predicting. This is only
     # a requirement if `uncertainty` is set, as we need access to `self.X_train`
     if not hasattr(self, "X_train") or self.X_train is None:
         raise RuntimeError(
-            "This model has not been fitted yet! Call fit() "
-            "before predicting new samples."
+            "This model has not been fitted yet! Call fit() before predicting new "
+            "samples."
         )
 
     # Store the number of data points in the training and test datasets
     n_train = self.X_train.shape[0]
 
     # The authors chose the number of bootstrap samples as the square root of the
     # number of samples in the training dataset
@@ -291,24 +313,45 @@
 
     # Centre the bootstrapped predictions across the bootstrap dimension
     bootstrap_preds -= np.mean(bootstrap_preds, axis=0)
 
     # Add up the bootstrap predictions and the hybrid train/val residuals
     C = np.array([m + o for m in bootstrap_preds for o in self.residuals])
 
-    # Calculate the desired quantiles
+    # If we are dealing with a single sample then we replace the predictions with the
+    # first sample
+    if onedim:
+        preds = preds[0]
+
+    # Next, we compute the associated uncertainty data, if requested. Firstly, if
+    # `return_all` is set then we return the raw bootstrapped predictions, being the
+    # `C` array
+    if return_all:
+        if onedim:
+            return preds, C[:, 0]
+        else:
+            return preds, C
+
+    # If the uncertainty has been specified and not the quantiles, then we compute
+    # the quantiles from the uncertainty
     if quantiles is None and uncertainty is not None:
         quantiles = [uncertainty / 2, 1 - uncertainty / 2]
+
+    # Compute the quantiles of the `C` array
     quantile_vals = np.transpose(np.quantile(C, q=quantiles or [], axis=0))
 
-    # Return the predictions and the desired quantiles
+    # Add the quantiles to the predictions to get the final prediction intervals
+    # as the uncertainty data
     if onedim:
-        return preds[0], (preds + quantile_vals)[0]
+        intervals = preds + quantile_vals[0]
     else:
-        return preds, np.expand_dims(preds, axis=1) + quantile_vals
+        intervals = np.expand_dims(preds, axis=1) + quantile_vals
+
+    # Return the predictions and the prediction intervals
+    return preds, intervals
 
 
 def fit(self, X: np.ndarray, y: np.ndarray, n_boots: Optional[int] = None):
     """Fits the model to the data.
 
     Args:
         X (float array):
```

### Comparing `doubt-4.3.1/src/doubt/models/glm/quantile_loss.py` & `doubt-4.4.0/src/doubt/models/glm/quantile_loss.py`

 * *Files identical despite different names*

### Comparing `doubt-4.3.1/src/doubt/models/glm/quantile_regressor.py` & `doubt-4.4.0/src/doubt/models/glm/quantile_regressor.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,14 @@
         self,
         model: Union[LinearRegression, _GeneralizedLinearRegressor],
         max_iter: Optional[int] = None,
         uncertainty: float = 0.05,
         quantiles: Optional[np.ndarray] = None,
         alpha: float = 0.4,
     ):
-
         self.uncertainty = uncertainty
         self.alpha = alpha
 
         self._model = model
         self._scaler = StandardScaler()
 
         # Set `max_iter` to be the model's `max_iter` attribute if it exists, and
@@ -143,15 +142,14 @@
         # weights
         model_weights = self._model.coef_
         model_intercept = self._model.intercept_
         beta_init = np.concatenate((model_weights, [model_intercept]))
 
         # Fit all quantile estimates
         for q in self.quantiles:
-
             args = (X_arr, y_arr, q, self._inverse_link_function)
             result = minimize(
                 self._objective_function,
                 beta_init,
                 args=args,
                 method="BFGS",
                 options={"maxiter": self.max_iter},
```

### Comparing `doubt-4.3.1/src/doubt/models/tree/forest.py` & `doubt-4.4.0/src/doubt/models/tree/forest.py`

 * *Files identical despite different names*

### Comparing `doubt-4.3.1/src/doubt/models/tree/tree.py` & `doubt-4.4.0/src/doubt/models/tree/tree.py`

 * *Files identical despite different names*

### Comparing `doubt-4.3.1/src/doubt/models/tree/utils.py` & `doubt-4.4.0/src/doubt/models/tree/utils.py`

 * *Files identical despite different names*

### Comparing `doubt-4.3.1/setup.py` & `doubt-4.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,26 +12,26 @@
  'doubt.models.glm',
  'doubt.models.tree']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['joblib>=1.1.0,<2.0.0',
+['joblib>=1.2.0,<2.0.0',
  'numpy>=1.23.0,<2.0.0',
  'openpyxl>=3.0.10,<4.0.0',
  'pandas>=1.4.0,<2.0.0',
  'scikit-learn>=1.1.1,<2.0.0',
  'tables>=3.7.0,<4.0.0',
  'tqdm>=4.62.0,<5.0.0',
  'xlrd>=2.0.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'doubt',
-    'version': '4.3.1',
+    'version': '4.4.0',
     'description': 'Bringing back uncertainty to machine learning.',
     'long_description': '# Doubt\n\n*Bringing back uncertainty to machine learning.*\n\n______________________________________________________________________\n[![PyPI Status](https://badge.fury.io/py/doubt.svg)](https://pypi.org/project/doubt/)\n[![Documentation](https://img.shields.io/badge/docs-passing-green)](https://saattrupdan.github.io/doubt/doubt.html)\n[![License](https://img.shields.io/github/license/saattrupdan/doubt)](https://github.com/saattrupdan/doubt/blob/main/LICENSE)\n[![LastCommit](https://img.shields.io/github/last-commit/saattrupdan/doubt)](https://github.com/saattrupdan/doubt/commits/main)\n[![Code Coverage](https://img.shields.io/badge/Coverage-67%25-yellow.svg)](https://github.com/saattrupdan/doubt/tree/dev/tests)\n[![Conference](https://img.shields.io/badge/Conference-AAAI23-blue)](https://arxiv.org/abs/2201.11676)\n\nA Python package to include prediction intervals in the predictions of machine\nlearning models, to quantify their uncertainty.\n\n\n## Installation\n\nIf you do not already have HDF5 installed, then start by installing that. On MacOS this\ncan be done using `sudo port install hdf5` after\n[MacPorts](https://www.macports.org/install.php) have been installed. On Ubuntu you can\nget HDF5 with `sudo apt-get install python-dev python3-dev libhdf5-serial-dev`. After\nthat, you can install `doubt` with `pip`:\n\n```shell\npip install doubt\n```\n\n\n## Features\n\n- Bootstrap wrapper for all Scikit-Learn models\n    - Can also be used to calculate usual bootstrapped statistics of a dataset\n- Quantile Regression for all generalised linear models\n- Quantile Regression Forests\n- A uniform dataset API, with 24 regression datasets and counting\n\n\n## Quick Start\n\nIf you already have a model in Scikit-Learn, then you can simply\nwrap it in a `Boot` to enable predicting with prediction intervals:\n\n```python\n>>> from sklearn.linear_model import LinearRegression\n>>> from doubt import Boot\n>>> from doubt.datasets import PowerPlant\n>>>\n>>> X, y = PowerPlant().split()\n>>> clf = Boot(LinearRegression())\n>>> clf = clf.fit(X, y)\n>>> clf.predict([10, 30, 1000, 50], uncertainty=0.05)\n(481.9203102126274, array([473.43314309, 490.0313962 ]))\n```\n\nAlternatively, you can use one of the standalone models with uncertainty\noutputs. For instance, a `QuantileRegressionForest`:\n\n```python\n>>> from doubt import QuantileRegressionForest as QRF\n>>> from doubt.datasets import Concrete\n>>> import numpy as np\n>>>\n>>> X, y = Concrete().split()\n>>> clf = QRF(max_leaf_nodes=8)\n>>> clf.fit(X, y)\n>>> clf.predict(np.ones(8), uncertainty=0.25)\n(16.933590347847982, array([ 8.93456428, 26.0664534 ]))\n```\n',
     'author': 'Dan Saattrup Nielsen',
     'author_email': 'saattrupdan@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/saattrupdan/doubt',
```

### Comparing `doubt-4.3.1/PKG-INFO` & `doubt-4.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: doubt
-Version: 4.3.1
+Version: 4.4.0
 Summary: Bringing back uncertainty to machine learning.
 Home-page: https://github.com/saattrupdan/doubt
 License: MIT
 Author: Dan Saattrup Nielsen
 Author-email: saattrupdan@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: joblib (>=1.1.0,<2.0.0)
+Requires-Dist: joblib (>=1.2.0,<2.0.0)
 Requires-Dist: numpy (>=1.23.0,<2.0.0)
 Requires-Dist: openpyxl (>=3.0.10,<4.0.0)
 Requires-Dist: pandas (>=1.4.0,<2.0.0)
 Requires-Dist: scikit-learn (>=1.1.1,<2.0.0)
 Requires-Dist: tables (>=3.7.0,<4.0.0)
 Requires-Dist: tqdm (>=4.62.0,<5.0.0)
 Requires-Dist: xlrd (>=2.0.1,<3.0.0)
```

