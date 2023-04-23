# Comparing `tmp/doubt-4.4.0.tar.gz` & `tmp/doubt-4.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doubt-4.4.0.tar", max compression
+gzip compressed data, was "doubt-4.4.1.tar", max compression
```

## Comparing `doubt-4.4.0.tar` & `doubt-4.4.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1056 2022-07-17 15:34:56.352960 doubt-4.4.0/LICENSE
--rw-r--r--   0        0        0     2583 2023-03-20 18:25:20.177518 doubt-4.4.0/README.md
--rw-r--r--   0        0        0     1310 2023-04-23 18:26:13.875394 doubt-4.4.0/pyproject.toml
--rw-r--r--   0        0        0      369 2023-03-20 19:12:08.029301 doubt-4.4.0/src/doubt/__init__.py
--rw-r--r--   0        0        0     1082 2022-07-17 15:34:56.355574 doubt-4.4.0/src/doubt/datasets/__init__.py
--rw-r--r--   0        0        0     2510 2022-07-17 15:34:56.355799 doubt-4.4.0/src/doubt/datasets/airfoil.py
--rw-r--r--   0        0        0     4903 2022-07-17 15:34:56.356034 doubt-4.4.0/src/doubt/datasets/bike_sharing_daily.py
--rw-r--r--   0        0        0     4995 2022-07-17 15:34:56.356216 doubt-4.4.0/src/doubt/datasets/bike_sharing_hourly.py
--rw-r--r--   0        0        0     5661 2022-07-17 15:34:56.356397 doubt-4.4.0/src/doubt/datasets/blog.py
--rw-r--r--   0        0        0     2808 2022-07-17 15:34:56.356560 doubt-4.4.0/src/doubt/datasets/concrete.py
--rw-r--r--   0        0        0     2846 2022-07-17 15:34:56.356716 doubt-4.4.0/src/doubt/datasets/cpu.py
--rw-r--r--   0        0        0     4225 2023-03-20 18:57:45.250733 doubt-4.4.0/src/doubt/datasets/dataset.py
--rw-r--r--   0        0        0     5653 2022-07-17 15:34:56.357060 doubt-4.4.0/src/doubt/datasets/facebook_comments.py
--rw-r--r--   0        0        0     4629 2022-07-17 15:34:56.357231 doubt-4.4.0/src/doubt/datasets/facebook_metrics.py
--rw-r--r--   0        0        0     5825 2022-07-17 15:34:56.357435 doubt-4.4.0/src/doubt/datasets/fish_bioconcentration.py
--rw-r--r--   0        0        0     2857 2022-07-17 15:34:56.357617 doubt-4.4.0/src/doubt/datasets/fish_toxicity.py
--rw-r--r--   0        0        0     3924 2022-07-17 15:34:56.357779 doubt-4.4.0/src/doubt/datasets/forest_fire.py
--rw-r--r--   0        0        0     6646 2022-07-17 15:34:56.357967 doubt-4.4.0/src/doubt/datasets/gas_turbine.py
--rw-r--r--   0        0        0     4273 2022-07-17 15:34:56.358157 doubt-4.4.0/src/doubt/datasets/nanotube.py
--rw-r--r--   0        0        0     2950 2022-07-17 15:34:56.358328 doubt-4.4.0/src/doubt/datasets/new_taipei_housing.py
--rw-r--r--   0        0        0     4667 2022-07-17 15:34:56.358499 doubt-4.4.0/src/doubt/datasets/parkinsons.py
--rw-r--r--   0        0        0     3786 2022-07-17 15:34:56.358663 doubt-4.4.0/src/doubt/datasets/power_plant.py
--rw-r--r--   0        0        0     2857 2022-07-17 15:34:56.358822 doubt-4.4.0/src/doubt/datasets/protein.py
--rw-r--r--   0        0        0     3421 2022-07-17 15:34:56.359001 doubt-4.4.0/src/doubt/datasets/servo.py
--rw-r--r--   0        0        0     4743 2022-07-17 15:34:56.359172 doubt-4.4.0/src/doubt/datasets/solar_flare.py
--rw-r--r--   0        0        0     4463 2022-07-17 15:34:56.359375 doubt-4.4.0/src/doubt/datasets/space_shuttle.py
--rw-r--r--   0        0        0     5313 2022-07-17 15:34:56.359607 doubt-4.4.0/src/doubt/datasets/stocks.py
--rw-r--r--   0        0        0     5421 2022-07-17 15:34:56.359788 doubt-4.4.0/src/doubt/datasets/superconductivity.py
--rw-r--r--   0        0        0     3351 2022-07-17 15:34:56.360044 doubt-4.4.0/src/doubt/datasets/tehran_housing.py
--rw-r--r--   0        0        0     3357 2022-07-17 15:34:56.360230 doubt-4.4.0/src/doubt/datasets/yacht.py
--rw-r--r--   0        0        0      174 2022-07-17 15:34:56.360496 doubt-4.4.0/src/doubt/models/__init__.py
--rw-r--r--   0        0        0       31 2022-07-17 15:34:56.360777 doubt-4.4.0/src/doubt/models/boot/__init__.py
--rw-r--r--   0        0        0    16835 2023-04-23 18:24:53.138955 doubt-4.4.0/src/doubt/models/boot/boot.py
--rw-r--r--   0        0        0       58 2022-07-17 15:34:56.361181 doubt-4.4.0/src/doubt/models/glm/__init__.py
--rw-r--r--   0        0        0     2235 2022-07-17 15:34:56.361351 doubt-4.4.0/src/doubt/models/glm/quantile_loss.py
--rw-r--r--   0        0        0     9220 2023-03-20 18:57:45.276816 doubt-4.4.0/src/doubt/models/glm/quantile_regressor.py
--rw-r--r--   0        0        0      495 2022-07-17 15:34:56.361782 doubt-4.4.0/src/doubt/models/model.py
--rw-r--r--   0        0        0      102 2022-07-17 15:34:56.361953 doubt-4.4.0/src/doubt/models/tree/__init__.py
--rw-r--r--   0        0        0    13354 2023-03-20 18:32:48.084709 doubt-4.4.0/src/doubt/models/tree/forest.py
--rw-r--r--   0        0        0    10540 2023-03-20 18:33:10.883879 doubt-4.4.0/src/doubt/models/tree/tree.py
--rw-r--r--   0        0        0     3821 2022-07-17 15:34:56.362536 doubt-4.4.0/src/doubt/models/tree/utils.py
--rw-r--r--   0        0        0     3667 1970-01-01 00:00:00.000000 doubt-4.4.0/setup.py
--rw-r--r--   0        0        0     3515 1970-01-01 00:00:00.000000 doubt-4.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1056 2022-07-17 15:34:56.352960 doubt-4.4.1/LICENSE
+-rw-r--r--   0        0        0     2583 2023-03-20 18:25:20.177518 doubt-4.4.1/README.md
+-rw-r--r--   0        0        0     1310 2023-04-23 18:38:39.796211 doubt-4.4.1/pyproject.toml
+-rw-r--r--   0        0        0      369 2023-03-20 19:12:08.029301 doubt-4.4.1/src/doubt/__init__.py
+-rw-r--r--   0        0        0     1082 2022-07-17 15:34:56.355574 doubt-4.4.1/src/doubt/datasets/__init__.py
+-rw-r--r--   0        0        0     2510 2022-07-17 15:34:56.355799 doubt-4.4.1/src/doubt/datasets/airfoil.py
+-rw-r--r--   0        0        0     4903 2022-07-17 15:34:56.356034 doubt-4.4.1/src/doubt/datasets/bike_sharing_daily.py
+-rw-r--r--   0        0        0     4995 2022-07-17 15:34:56.356216 doubt-4.4.1/src/doubt/datasets/bike_sharing_hourly.py
+-rw-r--r--   0        0        0     5661 2022-07-17 15:34:56.356397 doubt-4.4.1/src/doubt/datasets/blog.py
+-rw-r--r--   0        0        0     2808 2022-07-17 15:34:56.356560 doubt-4.4.1/src/doubt/datasets/concrete.py
+-rw-r--r--   0        0        0     2846 2022-07-17 15:34:56.356716 doubt-4.4.1/src/doubt/datasets/cpu.py
+-rw-r--r--   0        0        0     4225 2023-03-20 18:57:45.250733 doubt-4.4.1/src/doubt/datasets/dataset.py
+-rw-r--r--   0        0        0     5653 2022-07-17 15:34:56.357060 doubt-4.4.1/src/doubt/datasets/facebook_comments.py
+-rw-r--r--   0        0        0     4629 2022-07-17 15:34:56.357231 doubt-4.4.1/src/doubt/datasets/facebook_metrics.py
+-rw-r--r--   0        0        0     5825 2022-07-17 15:34:56.357435 doubt-4.4.1/src/doubt/datasets/fish_bioconcentration.py
+-rw-r--r--   0        0        0     2857 2022-07-17 15:34:56.357617 doubt-4.4.1/src/doubt/datasets/fish_toxicity.py
+-rw-r--r--   0        0        0     3924 2022-07-17 15:34:56.357779 doubt-4.4.1/src/doubt/datasets/forest_fire.py
+-rw-r--r--   0        0        0     6646 2022-07-17 15:34:56.357967 doubt-4.4.1/src/doubt/datasets/gas_turbine.py
+-rw-r--r--   0        0        0     4273 2022-07-17 15:34:56.358157 doubt-4.4.1/src/doubt/datasets/nanotube.py
+-rw-r--r--   0        0        0     2950 2022-07-17 15:34:56.358328 doubt-4.4.1/src/doubt/datasets/new_taipei_housing.py
+-rw-r--r--   0        0        0     4667 2022-07-17 15:34:56.358499 doubt-4.4.1/src/doubt/datasets/parkinsons.py
+-rw-r--r--   0        0        0     3786 2022-07-17 15:34:56.358663 doubt-4.4.1/src/doubt/datasets/power_plant.py
+-rw-r--r--   0        0        0     2857 2022-07-17 15:34:56.358822 doubt-4.4.1/src/doubt/datasets/protein.py
+-rw-r--r--   0        0        0     3421 2022-07-17 15:34:56.359001 doubt-4.4.1/src/doubt/datasets/servo.py
+-rw-r--r--   0        0        0     4743 2022-07-17 15:34:56.359172 doubt-4.4.1/src/doubt/datasets/solar_flare.py
+-rw-r--r--   0        0        0     4463 2022-07-17 15:34:56.359375 doubt-4.4.1/src/doubt/datasets/space_shuttle.py
+-rw-r--r--   0        0        0     5313 2022-07-17 15:34:56.359607 doubt-4.4.1/src/doubt/datasets/stocks.py
+-rw-r--r--   0        0        0     5421 2022-07-17 15:34:56.359788 doubt-4.4.1/src/doubt/datasets/superconductivity.py
+-rw-r--r--   0        0        0     3351 2022-07-17 15:34:56.360044 doubt-4.4.1/src/doubt/datasets/tehran_housing.py
+-rw-r--r--   0        0        0     3357 2022-07-17 15:34:56.360230 doubt-4.4.1/src/doubt/datasets/yacht.py
+-rw-r--r--   0        0        0      174 2022-07-17 15:34:56.360496 doubt-4.4.1/src/doubt/models/__init__.py
+-rw-r--r--   0        0        0       31 2022-07-17 15:34:56.360777 doubt-4.4.1/src/doubt/models/boot/__init__.py
+-rw-r--r--   0        0        0    16837 2023-04-23 18:36:29.040992 doubt-4.4.1/src/doubt/models/boot/boot.py
+-rw-r--r--   0        0        0       58 2022-07-17 15:34:56.361181 doubt-4.4.1/src/doubt/models/glm/__init__.py
+-rw-r--r--   0        0        0     2235 2022-07-17 15:34:56.361351 doubt-4.4.1/src/doubt/models/glm/quantile_loss.py
+-rw-r--r--   0        0        0     9220 2023-03-20 18:57:45.276816 doubt-4.4.1/src/doubt/models/glm/quantile_regressor.py
+-rw-r--r--   0        0        0      495 2022-07-17 15:34:56.361782 doubt-4.4.1/src/doubt/models/model.py
+-rw-r--r--   0        0        0      102 2022-07-17 15:34:56.361953 doubt-4.4.1/src/doubt/models/tree/__init__.py
+-rw-r--r--   0        0        0    13354 2023-03-20 18:32:48.084709 doubt-4.4.1/src/doubt/models/tree/forest.py
+-rw-r--r--   0        0        0    10540 2023-03-20 18:33:10.883879 doubt-4.4.1/src/doubt/models/tree/tree.py
+-rw-r--r--   0        0        0     3821 2022-07-17 15:34:56.362536 doubt-4.4.1/src/doubt/models/tree/utils.py
+-rw-r--r--   0        0        0     3667 1970-01-01 00:00:00.000000 doubt-4.4.1/setup.py
+-rw-r--r--   0        0        0     3515 1970-01-01 00:00:00.000000 doubt-4.4.1/PKG-INFO
```

### Comparing `doubt-4.4.0/LICENSE` & `doubt-4.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/README.md` & `doubt-4.4.1/README.md`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/pyproject.toml` & `doubt-4.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "doubt"
-version = "4.4.0"
+version = "4.4.1"
 description = "Bringing back uncertainty to machine learning."
 authors = ["Dan Saattrup Nielsen <saattrupdan@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/saattrupdan/doubt"
 
 [tool.poetry.dependencies]
```

### Comparing `doubt-4.4.0/src/doubt/datasets/__init__.py` & `doubt-4.4.1/src/doubt/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/src/doubt/datasets/airfoil.py` & `doubt-4.4.1/src/doubt/datasets/airfoil.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/src/doubt/datasets/bike_sharing_daily.py` & `doubt-4.4.1/src/doubt/datasets/bike_sharing_daily.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/src/doubt/datasets/bike_sharing_hourly.py` & `doubt-4.4.1/src/doubt/datasets/bike_sharing_hourly.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/src/doubt/datasets/blog.py` & `doubt-4.4.1/src/doubt/datasets/blog.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/src/doubt/datasets/concrete.py` & `doubt-4.4.1/src/doubt/datasets/concrete.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/src/doubt/datasets/cpu.py` & `doubt-4.4.1/src/doubt/datasets/cpu.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/src/doubt/datasets/dataset.py` & `doubt-4.4.1/src/doubt/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/src/doubt/datasets/facebook_comments.py` & `doubt-4.4.1/src/doubt/datasets/facebook_comments.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/src/doubt/datasets/facebook_metrics.py` & `doubt-4.4.1/src/doubt/datasets/facebook_metrics.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/src/doubt/datasets/fish_bioconcentration.py` & `doubt-4.4.1/src/doubt/datasets/fish_bioconcentration.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/src/doubt/datasets/fish_toxicity.py` & `doubt-4.4.1/src/doubt/datasets/fish_toxicity.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/src/doubt/datasets/forest_fire.py` & `doubt-4.4.1/src/doubt/datasets/forest_fire.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/src/doubt/datasets/gas_turbine.py` & `doubt-4.4.1/src/doubt/datasets/gas_turbine.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/src/doubt/datasets/nanotube.py` & `doubt-4.4.1/src/doubt/datasets/nanotube.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/src/doubt/datasets/new_taipei_housing.py` & `doubt-4.4.1/src/doubt/datasets/new_taipei_housing.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/src/doubt/datasets/parkinsons.py` & `doubt-4.4.1/src/doubt/datasets/parkinsons.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/src/doubt/datasets/power_plant.py` & `doubt-4.4.1/src/doubt/datasets/power_plant.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/src/doubt/datasets/protein.py` & `doubt-4.4.1/src/doubt/datasets/protein.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/src/doubt/datasets/servo.py` & `doubt-4.4.1/src/doubt/datasets/servo.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/src/doubt/datasets/solar_flare.py` & `doubt-4.4.1/src/doubt/datasets/solar_flare.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/src/doubt/datasets/space_shuttle.py` & `doubt-4.4.1/src/doubt/datasets/space_shuttle.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/src/doubt/datasets/stocks.py` & `doubt-4.4.1/src/doubt/datasets/stocks.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/src/doubt/datasets/superconductivity.py` & `doubt-4.4.1/src/doubt/datasets/superconductivity.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/src/doubt/datasets/tehran_housing.py` & `doubt-4.4.1/src/doubt/datasets/tehran_housing.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/src/doubt/datasets/yacht.py` & `doubt-4.4.1/src/doubt/datasets/yacht.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/src/doubt/models/boot/boot.py` & `doubt-4.4.1/src/doubt/models/boot/boot.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,15 +325,15 @@
     # Next, we compute the associated uncertainty data, if requested. Firstly, if
     # `return_all` is set then we return the raw bootstrapped predictions, being the
     # `C` array
     if return_all:
         if onedim:
             return preds, C[:, 0]
         else:
-            return preds, C
+            return preds, C.T
 
     # If the uncertainty has been specified and not the quantiles, then we compute
     # the quantiles from the uncertainty
     if quantiles is None and uncertainty is not None:
         quantiles = [uncertainty / 2, 1 - uncertainty / 2]
 
     # Compute the quantiles of the `C` array
```

### Comparing `doubt-4.4.0/src/doubt/models/glm/quantile_loss.py` & `doubt-4.4.1/src/doubt/models/glm/quantile_loss.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/src/doubt/models/glm/quantile_regressor.py` & `doubt-4.4.1/src/doubt/models/glm/quantile_regressor.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/src/doubt/models/tree/forest.py` & `doubt-4.4.1/src/doubt/models/tree/forest.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/src/doubt/models/tree/tree.py` & `doubt-4.4.1/src/doubt/models/tree/tree.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/src/doubt/models/tree/utils.py` & `doubt-4.4.1/src/doubt/models/tree/utils.py`

 * *Files identical despite different names*

### Comparing `doubt-4.4.0/setup.py` & `doubt-4.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
  'scikit-learn>=1.1.1,<2.0.0',
  'tables>=3.7.0,<4.0.0',
  'tqdm>=4.62.0,<5.0.0',
  'xlrd>=2.0.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'doubt',
-    'version': '4.4.0',
+    'version': '4.4.1',
     'description': 'Bringing back uncertainty to machine learning.',
     'long_description': '# Doubt\n\n*Bringing back uncertainty to machine learning.*\n\n______________________________________________________________________\n[![PyPI Status](https://badge.fury.io/py/doubt.svg)](https://pypi.org/project/doubt/)\n[![Documentation](https://img.shields.io/badge/docs-passing-green)](https://saattrupdan.github.io/doubt/doubt.html)\n[![License](https://img.shields.io/github/license/saattrupdan/doubt)](https://github.com/saattrupdan/doubt/blob/main/LICENSE)\n[![LastCommit](https://img.shields.io/github/last-commit/saattrupdan/doubt)](https://github.com/saattrupdan/doubt/commits/main)\n[![Code Coverage](https://img.shields.io/badge/Coverage-67%25-yellow.svg)](https://github.com/saattrupdan/doubt/tree/dev/tests)\n[![Conference](https://img.shields.io/badge/Conference-AAAI23-blue)](https://arxiv.org/abs/2201.11676)\n\nA Python package to include prediction intervals in the predictions of machine\nlearning models, to quantify their uncertainty.\n\n\n## Installation\n\nIf you do not already have HDF5 installed, then start by installing that. On MacOS this\ncan be done using `sudo port install hdf5` after\n[MacPorts](https://www.macports.org/install.php) have been installed. On Ubuntu you can\nget HDF5 with `sudo apt-get install python-dev python3-dev libhdf5-serial-dev`. After\nthat, you can install `doubt` with `pip`:\n\n```shell\npip install doubt\n```\n\n\n## Features\n\n- Bootstrap wrapper for all Scikit-Learn models\n    - Can also be used to calculate usual bootstrapped statistics of a dataset\n- Quantile Regression for all generalised linear models\n- Quantile Regression Forests\n- A uniform dataset API, with 24 regression datasets and counting\n\n\n## Quick Start\n\nIf you already have a model in Scikit-Learn, then you can simply\nwrap it in a `Boot` to enable predicting with prediction intervals:\n\n```python\n>>> from sklearn.linear_model import LinearRegression\n>>> from doubt import Boot\n>>> from doubt.datasets import PowerPlant\n>>>\n>>> X, y = PowerPlant().split()\n>>> clf = Boot(LinearRegression())\n>>> clf = clf.fit(X, y)\n>>> clf.predict([10, 30, 1000, 50], uncertainty=0.05)\n(481.9203102126274, array([473.43314309, 490.0313962 ]))\n```\n\nAlternatively, you can use one of the standalone models with uncertainty\noutputs. For instance, a `QuantileRegressionForest`:\n\n```python\n>>> from doubt import QuantileRegressionForest as QRF\n>>> from doubt.datasets import Concrete\n>>> import numpy as np\n>>>\n>>> X, y = Concrete().split()\n>>> clf = QRF(max_leaf_nodes=8)\n>>> clf.fit(X, y)\n>>> clf.predict(np.ones(8), uncertainty=0.25)\n(16.933590347847982, array([ 8.93456428, 26.0664534 ]))\n```\n',
     'author': 'Dan Saattrup Nielsen',
     'author_email': 'saattrupdan@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/saattrupdan/doubt',
```

### Comparing `doubt-4.4.0/PKG-INFO` & `doubt-4.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doubt
-Version: 4.4.0
+Version: 4.4.1
 Summary: Bringing back uncertainty to machine learning.
 Home-page: https://github.com/saattrupdan/doubt
 License: MIT
 Author: Dan Saattrup Nielsen
 Author-email: saattrupdan@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

