# Comparing `tmp/zfista-0.0.1.tar.gz` & `tmp/zfista-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zfista-0.0.1.tar", last modified: Tue May 10 12:51:55 2022, max compression
+gzip compressed data, was "zfista-0.0.2.tar", last modified: Sun Apr 23 15:06:07 2023, max compression
```

## Comparing `zfista-0.0.1.tar` & `zfista-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,25 @@
-drwxr-xr-x   0 zalgo      (501) staff       (20)        0 2022-05-10 12:51:55.338927 zfista-0.0.1/
--rw-r--r--   0 zalgo      (501) staff       (20)     1070 2022-05-10 06:41:25.000000 zfista-0.0.1/LICENSE
--rw-r--r--   0 zalgo      (501) staff       (20)       17 2022-05-10 08:07:00.000000 zfista-0.0.1/MANIFEST.in
--rw-r--r--   0 zalgo      (501) staff       (20)     1220 2022-05-10 12:51:55.338347 zfista-0.0.1/PKG-INFO
--rw-r--r--   0 zalgo      (501) staff       (20)      846 2022-05-10 08:41:38.000000 zfista-0.0.1/README.md
--rw-r--r--   0 zalgo      (501) staff       (20)       38 2022-05-10 12:51:55.339241 zfista-0.0.1/setup.cfg
--rw-r--r--   0 zalgo      (501) staff       (20)      987 2022-05-10 08:45:43.000000 zfista-0.0.1/setup.py
-drwxr-xr-x   0 zalgo      (501) staff       (20)        0 2022-05-10 12:51:55.332323 zfista-0.0.1/tests/
--rw-r--r--   0 zalgo      (501) staff       (20)        0 2022-05-10 02:24:04.000000 zfista-0.0.1/tests/__init__.py
--rw-r--r--   0 zalgo      (501) staff       (20)     5365 2022-05-10 08:44:34.000000 zfista-0.0.1/tests/test_proximal_gradient.py
-drwxr-xr-x   0 zalgo      (501) staff       (20)        0 2022-05-10 12:51:55.334130 zfista-0.0.1/zfista/
--rw-r--r--   0 zalgo      (501) staff       (20)      121 2022-05-10 08:42:43.000000 zfista-0.0.1/zfista/__init__.py
--rw-r--r--   0 zalgo      (501) staff       (20)     9781 2022-05-10 08:27:36.000000 zfista-0.0.1/zfista/proximal_gradient.py
-drwxr-xr-x   0 zalgo      (501) staff       (20)        0 2022-05-10 12:51:55.337421 zfista-0.0.1/zfista.egg-info/
--rw-r--r--   0 zalgo      (501) staff       (20)     1220 2022-05-10 12:51:55.000000 zfista-0.0.1/zfista.egg-info/PKG-INFO
--rw-r--r--   0 zalgo      (501) staff       (20)      284 2022-05-10 12:51:55.000000 zfista-0.0.1/zfista.egg-info/SOURCES.txt
--rw-r--r--   0 zalgo      (501) staff       (20)        1 2022-05-10 12:51:55.000000 zfista-0.0.1/zfista.egg-info/dependency_links.txt
--rw-r--r--   0 zalgo      (501) staff       (20)      102 2022-05-10 12:51:55.000000 zfista-0.0.1/zfista.egg-info/requires.txt
--rw-r--r--   0 zalgo      (501) staff       (20)       13 2022-05-10 12:51:55.000000 zfista-0.0.1/zfista.egg-info/top_level.txt
+drwxr-xr-x   0 zalgo      (501) staff       (20)        0 2023-04-23 15:06:07.149808 zfista-0.0.2/
+-rw-r--r--   0 zalgo      (501) staff       (20)     1070 2023-04-08 12:23:58.000000 zfista-0.0.2/LICENSE
+-rw-r--r--   0 zalgo      (501) staff       (20)     2485 2023-04-23 15:06:07.150016 zfista-0.0.2/PKG-INFO
+-rw-r--r--   0 zalgo      (501) staff       (20)     2072 2023-04-23 11:27:09.000000 zfista-0.0.2/README.md
+drwxr-xr-x   0 zalgo      (501) staff       (20)        0 2023-04-23 15:06:07.137624 zfista-0.0.2/benchmarks/
+-rw-r--r--   0 zalgo      (501) staff       (20)        0 2023-04-23 10:16:42.000000 zfista-0.0.2/benchmarks/__init__.py
+-rw-r--r--   0 zalgo      (501) staff       (20)    17025 2023-04-23 11:27:09.000000 zfista-0.0.2/benchmarks/benchmark.py
+-rw-r--r--   0 zalgo      (501) staff       (20)      193 2023-04-23 10:16:42.000000 zfista-0.0.2/pyproject.toml
+-rw-r--r--   0 zalgo      (501) staff       (20)      626 2023-04-23 15:06:07.151097 zfista-0.0.2/setup.cfg
+drwxr-xr-x   0 zalgo      (501) staff       (20)        0 2023-04-23 15:06:07.141325 zfista-0.0.2/tests/
+-rw-r--r--   0 zalgo      (501) staff       (20)        0 2023-04-08 12:23:59.000000 zfista-0.0.2/tests/__init__.py
+-rw-r--r--   0 zalgo      (501) staff       (20)     3628 2023-04-23 10:16:42.000000 zfista-0.0.2/tests/test_metrics.py
+-rw-r--r--   0 zalgo      (501) staff       (20)     4131 2023-04-23 10:16:42.000000 zfista-0.0.2/tests/test_problems.py
+-rw-r--r--   0 zalgo      (501) staff       (20)     8776 2023-04-23 10:16:42.000000 zfista-0.0.2/tests/test_proximal_gradient.py
+drwxr-xr-x   0 zalgo      (501) staff       (20)        0 2023-04-23 15:06:07.146163 zfista-0.0.2/zfista/
+-rw-r--r--   0 zalgo      (501) staff       (20)      100 2023-04-09 06:54:31.000000 zfista-0.0.2/zfista/__init__.py
+-rw-r--r--   0 zalgo      (501) staff       (20)     5905 2023-04-23 10:16:42.000000 zfista-0.0.2/zfista/metrics.py
+-rw-r--r--   0 zalgo      (501) staff       (20)    18539 2023-04-23 10:16:42.000000 zfista-0.0.2/zfista/problems.py
+-rw-r--r--   0 zalgo      (501) staff       (20)    14166 2023-04-23 11:27:09.000000 zfista-0.0.2/zfista/proximal_gradient.py
+drwxr-xr-x   0 zalgo      (501) staff       (20)        0 2023-04-23 15:06:07.149376 zfista-0.0.2/zfista.egg-info/
+-rw-r--r--   0 zalgo      (501) staff       (20)     2485 2023-04-23 15:06:07.000000 zfista-0.0.2/zfista.egg-info/PKG-INFO
+-rw-r--r--   0 zalgo      (501) staff       (20)      417 2023-04-23 15:06:07.000000 zfista-0.0.2/zfista.egg-info/SOURCES.txt
+-rw-r--r--   0 zalgo      (501) staff       (20)        1 2023-04-23 15:06:07.000000 zfista-0.0.2/zfista.egg-info/dependency_links.txt
+-rw-r--r--   0 zalgo      (501) staff       (20)      115 2023-04-23 15:06:07.000000 zfista-0.0.2/zfista.egg-info/requires.txt
+-rw-r--r--   0 zalgo      (501) staff       (20)       24 2023-04-23 15:06:07.000000 zfista-0.0.2/zfista.egg-info/top_level.txt
```

### Comparing `zfista-0.0.1/LICENSE` & `zfista-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zfista-0.0.1/tests/test_proximal_gradient.py` & `zfista-0.0.2/tests/test_proximal_gradient.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 import unittest
+from typing import Tuple
 
+import jax
 import numpy as np
+from jaxopt.prox import prox_lasso
 from numpy.testing import assert_array_almost_equal
 from sklearn.base import RegressorMixin
 from sklearn.linear_model._base import LinearModel
 
 from zfista import minimize_proximal_gradient
 
+jax.config.update("jax_enable_x64", True)
 
-def _soft_threshold(x, thresh):
-    return np.where(np.abs(x) <= thresh, 0, x - thresh * np.sign(x))
 
-
-def build_dataset(n_samples=50, n_features=200, n_informative_features=10, n_targets=1):
+def build_dataset(
+    n_samples: int = 50,
+    n_features: int = 200,
+    n_informative_features: int = 10,
+    n_targets: int = 1,
+) -> Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]:
     """
     build an ill-posed linear regression problem with many noisy features and
     comparatively few samples
     See https://github.com/scikit-learn/scikit-learn/blob/main/sklearn/linear_model/tests/test_coordinate_descent.py
     """
     random_state = np.random.RandomState(0)
     if n_targets > 1:
@@ -28,106 +34,179 @@
     y = np.dot(X, w)
     X_test = random_state.randn(n_samples, n_features)
     y_test = np.dot(X_test, w)
     return X, y, X_test, y_test
 
 
 class TestProximalGradient(unittest.TestCase):
-    def test_minimize_proximal_gradient_lasso_zero(self):
+    def test_minimize_proximal_gradient_lasso_zero(self) -> None:
         A = np.array([[0], [0], [0]])
         b = np.array([0, 0, 0])
         x0 = np.random.random(1)
-        l1_ratio = .1
+        l1_ratio = 0.1
 
-        def f(x):
+        def f(x: np.ndarray) -> np.floating:
             return np.linalg.norm(A @ x - b) ** 2 / 6
 
-        def g(x):
+        def g(x: np.ndarray) -> np.floating:
             return l1_ratio * np.linalg.norm(x, ord=1)
 
-        def jac_f(x):
+        def jac_f(x: np.ndarray) -> np.ndarray:
             return A.T @ (A @ x - b) / 3
 
-        def prox_wsum_g(weight, x):
-            return _soft_threshold(x, l1_ratio * weight)
+        def prox_wsum_g(weight: np.ndarray, x: np.ndarray) -> np.ndarray:
+            return prox_lasso(x, l1_ratio * weight)
 
         res = minimize_proximal_gradient(f, g, jac_f, prox_wsum_g, x0)
-        res_nesterov = minimize_proximal_gradient(f, g, jac_f, prox_wsum_g, x0, nesterov=True)
+        res_nesterov = minimize_proximal_gradient(
+            f, g, jac_f, prox_wsum_g, x0, nesterov=True
+        )
         assert_array_almost_equal(res.x, [0], decimal=3)
         assert_array_almost_equal(res_nesterov.x, [0], decimal=3)
 
-    def test_minimize_proximal_gradient_lasso_toy(self):
+    def test_minimize_proximal_gradient_lasso_toy(self) -> None:
         """
         min (1 / 2) ||Ax - b||^2 + l1_ratio * ||x||_1
         See https://github.com/scikit-learn/scikit-learn/blob/main/sklearn/linear_model/tests/test_coordinate_descent.py
         """
         A = np.array([[-1], [0], [1]])
         b = np.array([-1, 0, 1])
         x0 = np.random.random(1)
-        l1_ratios = [1e-8, .1, .5, 1]
+        l1_ratios = [1e-8, 0.1, 0.5, 1]
         for l1_ratio in l1_ratios:
-            def f(x):
+
+            def f(x: np.ndarray) -> np.floating:
                 return np.linalg.norm(A @ x - b) ** 2 / 6
 
-            def g(x):
+            def g(x: np.ndarray) -> np.floating:
                 return l1_ratio * np.linalg.norm(x, ord=1)
 
-            def jac_f(x):
+            def jac_f(x: np.ndarray) -> np.ndarray:
                 return A.T @ (A @ x - b) / 3
 
-            def prox_wsum_g(weight, x):
-                return _soft_threshold(x, l1_ratio * weight)
+            def prox_wsum_g(weight: np.ndarray, x: np.ndarray) -> np.ndarray:
+                return prox_lasso(x, l1_ratio * weight)
 
             res = minimize_proximal_gradient(f, g, jac_f, prox_wsum_g, x0)
-            res_nesterov = minimize_proximal_gradient(f, g, jac_f, prox_wsum_g, x0, nesterov=True)
+            res_nesterov = minimize_proximal_gradient(
+                f, g, jac_f, prox_wsum_g, x0, nesterov=True
+            )
             if l1_ratio == 1e-8:
                 assert_array_almost_equal(res.x, [1], decimal=3)
                 assert_array_almost_equal(res_nesterov.x, [1], decimal=3)
-            if l1_ratio == .1:
-                assert_array_almost_equal(res.x, [.85], decimal=3)
-                assert_array_almost_equal(res_nesterov.x, [.85], decimal=3)
-            if l1_ratio == .5:
-                assert_array_almost_equal(res.x, [.25], decimal=3)
-                assert_array_almost_equal(res_nesterov.x, [.25], decimal=3)
+            if l1_ratio == 0.1:
+                assert_array_almost_equal(res.x, [0.85], decimal=3)
+                assert_array_almost_equal(res_nesterov.x, [0.85], decimal=3)
+            if l1_ratio == 0.5:
+                assert_array_almost_equal(res.x, [0.25], decimal=3)
+                assert_array_almost_equal(res_nesterov.x, [0.25], decimal=3)
             if l1_ratio == 1:
                 assert_array_almost_equal(res.x, [0], decimal=3)
                 assert_array_almost_equal(res_nesterov.x, [0], decimal=3)
 
-    def test_minimize_proximal_gradient_multiobjective_lasso_toy(self):
+    def test_minimize_proximal_gradient_biobjective_lasso_toy(self) -> None:
         """
         min ((1 / 2) ||Ax - b||^2 + l1_ratio * ||x||_1, (1 / 2) ||Ax - b||^2 + l1_ratio * ||x||_1)
         See https://github.com/scikit-learn/scikit-learn/blob/main/sklearn/linear_model/tests/test_coordinate_descent.py
         """
         A = np.array([[-1], [0], [1]])
         b = np.array([-1, 0, 1])
         x0 = np.random.random(1)
-        l1_ratios = [1e-8, .1, .5, 1]
+        l1_ratios = [1e-8, 0.1, 0.5, 1]
         for l1_ratio in l1_ratios:
-            def f(x):
+
+            def f(x: np.ndarray) -> np.ndarray:
                 val = np.linalg.norm(A @ x - b) ** 2 / 6
                 return np.array([val, val])
 
-            def g(x):
+            def g(x: np.ndarray) -> np.ndarray:
                 val = l1_ratio * np.linalg.norm(x, ord=1)
                 return np.array([val, val])
 
-            def jac_f(x):
+            def jac_f(x: np.ndarray) -> np.ndarray:
                 grad_fi = A.T @ (A @ x - b) / 3
                 return np.vstack([grad_fi, grad_fi])
 
-            def prox_wsum_g(weight, x):
-                return _soft_threshold(x, l1_ratio * weight.sum())
+            def prox_wsum_g(weight: np.ndarray, x: np.ndarray) -> np.ndarray:
+                return prox_lasso(x, l1_ratio * weight.sum())
+
+            res = minimize_proximal_gradient(f, g, jac_f, prox_wsum_g, x0)
+            res_nesterov = minimize_proximal_gradient(
+                f, g, jac_f, prox_wsum_g, x0, nesterov=True
+            )
+            if l1_ratio == 1e-8:
+                assert_array_almost_equal(res.x, [1], decimal=3)
+                assert_array_almost_equal(res_nesterov.x, [1], decimal=3)
+            if l1_ratio == 0.1:
+                assert_array_almost_equal(res.x, [0.85], decimal=3)
+                assert_array_almost_equal(res_nesterov.x, [0.85], decimal=3)
+            if l1_ratio == 0.5:
+                assert_array_almost_equal(res.x, [0.25], decimal=3)
+                assert_array_almost_equal(res_nesterov.x, [0.25], decimal=3)
+            if l1_ratio == 1:
+                assert_array_almost_equal(res.x, [0], decimal=3)
+                assert_array_almost_equal(res_nesterov.x, [0], decimal=3)
+
+    def test_minimize_proximal_gradient_triobjective_lasso_toy(self) -> None:
+        """
+        min ((1 / 2) ||Ax - b||^2 + l1_ratio * ||x||_1, (1 / 2) ||Ax - b||^2 + l1_ratio * ||x||_1, (1 / 2) ||Ax - b||^2 + l1_ratio * ||x||_1)
+        See https://github.com/scikit-learn/scikit-learn/blob/main/sklearn/linear_model/tests/test_coordinate_descent.py
+        """
+        A = np.array([[-1], [0], [1]])
+        b = np.array([-1, 0, 1])
+        x0 = np.random.random(1)
+        l1_ratios = [1e-8, 0.1, 0.5, 1]
+        for l1_ratio in l1_ratios:
+
+            def f(x: np.ndarray) -> np.ndarray:
+                val = np.linalg.norm(A @ x - b) ** 2 / 6
+                return np.array([val, val, val])
+
+            def g(x: np.ndarray) -> np.ndarray:
+                val = l1_ratio * np.linalg.norm(x, ord=1)
+                return np.array([val, val, val])
+
+            def jac_f(x: np.ndarray) -> np.ndarray:
+                grad_fi = A.T @ (A @ x - b) / 3
+                return np.vstack([grad_fi, grad_fi, grad_fi])
+
+            def prox_wsum_g(weight: np.ndarray, x: np.ndarray) -> np.ndarray:
+                return prox_lasso(x, l1_ratio * weight.sum())
 
             res = minimize_proximal_gradient(f, g, jac_f, prox_wsum_g, x0)
-            res_nesterov = minimize_proximal_gradient(f, g, jac_f, prox_wsum_g, x0, nesterov=True)
+            res_nesterov = minimize_proximal_gradient(
+                f, g, jac_f, prox_wsum_g, x0, nesterov=True
+            )
             if l1_ratio == 1e-8:
                 assert_array_almost_equal(res.x, [1], decimal=3)
                 assert_array_almost_equal(res_nesterov.x, [1], decimal=3)
-            if l1_ratio == .1:
-                assert_array_almost_equal(res.x, [.85], decimal=3)
-                assert_array_almost_equal(res_nesterov.x, [.85], decimal=3)
-            if l1_ratio == .5:
-                assert_array_almost_equal(res.x, [.25], decimal=3)
-                assert_array_almost_equal(res_nesterov.x, [.25], decimal=3)
+            if l1_ratio == 0.1:
+                assert_array_almost_equal(res.x, [0.85], decimal=3)
+                assert_array_almost_equal(res_nesterov.x, [0.85], decimal=3)
+            if l1_ratio == 0.5:
+                assert_array_almost_equal(res.x, [0.25], decimal=3)
+                assert_array_almost_equal(res_nesterov.x, [0.25], decimal=3)
             if l1_ratio == 1:
                 assert_array_almost_equal(res.x, [0], decimal=3)
                 assert_array_almost_equal(res_nesterov.x, [0], decimal=3)
+
+    def test_minimize_proximal_gradient_return_all(self) -> None:
+        A = np.array([[0], [0], [0]])
+        b = np.array([0, 0, 0])
+        x0 = np.random.random(1)
+        l1_ratio = 0.1
+
+        def f(x: np.ndarray) -> np.floating:
+            return np.linalg.norm(A @ x - b) ** 2 / 6
+
+        def g(x: np.ndarray) -> np.floating:
+            return l1_ratio * np.linalg.norm(x, ord=1)
+
+        def jac_f(x: np.ndarray) -> np.ndarray:
+            return A.T @ (A @ x - b) / 3
+
+        def prox_wsum_g(weight: np.ndarray, x: np.ndarray) -> np.ndarray:
+            return prox_lasso(x, l1_ratio * weight)
+
+        res = minimize_proximal_gradient(f, g, jac_f, prox_wsum_g, x0, return_all=True)
+        self.assertIn("allvecs", res)
+        self.assertIn("allerrs", res)
```

