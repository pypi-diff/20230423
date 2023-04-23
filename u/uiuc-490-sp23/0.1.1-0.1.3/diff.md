# Comparing `tmp/uiuc_490_sp23-0.1.1.tar.gz` & `tmp/uiuc_490_sp23-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uiuc_490_sp23-0.1.1.tar", max compression
+gzip compressed data, was "uiuc_490_sp23-0.1.3.tar", max compression
```

## Comparing `uiuc_490_sp23-0.1.1.tar` & `uiuc_490_sp23-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,22 @@
--rw-r--r--   0        0        0    35149 2023-02-07 14:54:54.901894 uiuc_490_sp23-0.1.1/LICENSE
--rw-r--r--   0        0        0      761 2023-02-17 17:34:46.456713 uiuc_490_sp23-0.1.1/README.md
--rw-r--r--   0        0        0     1147 2023-02-17 18:05:24.067062 uiuc_490_sp23-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      245 2023-02-09 14:47:23.917357 uiuc_490_sp23-0.1.1/uiuc_490_sp23/Exceptions/__init__.py
--rw-r--r--   0        0        0     1893 2023-02-09 15:00:00.445643 uiuc_490_sp23-0.1.1/uiuc_490_sp23/LineSearch/__init__.py
--rw-r--r--   0        0        0      932 2023-02-09 15:02:14.697250 uiuc_490_sp23-0.1.1/uiuc_490_sp23/Optimizers/__init__.py
--rw-r--r--   0        0        0     2380 2023-02-17 15:16:37.386203 uiuc_490_sp23-0.1.1/uiuc_490_sp23/Problem/__init__.py
--rw-r--r--   0        0        0        0 2023-02-09 14:55:29.374372 uiuc_490_sp23-0.1.1/uiuc_490_sp23/__init__.py
--rw-r--r--   0        0        0      274 2023-02-17 17:34:03.079512 uiuc_490_sp23-0.1.1/uiuc_490_sp23/__main__.py
--rw-r--r--   0        0        0   128193 2023-02-07 14:54:54.901894 uiuc_490_sp23-0.1.1/uiuc_490_sp23/assignment1/Lab1_sp2023.pdf
--rw-r--r--   0        0        0        0 2023-02-09 15:05:12.046084 uiuc_490_sp23-0.1.1/uiuc_490_sp23/assignment1/__init__.py
--rwxr-xr-x   0        0        0     3897 2023-02-17 17:20:42.381330 uiuc_490_sp23-0.1.1/uiuc_490_sp23/assignment1/__main__.py
--rw-r--r--   0        0        0     1768 1970-01-01 00:00:00.000000 uiuc_490_sp23-0.1.1/setup.py
--rw-r--r--   0        0        0     1829 1970-01-01 00:00:00.000000 uiuc_490_sp23-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-02-20 13:45:18.959618 uiuc_490_sp23-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1512 2023-04-23 19:24:16.477844 uiuc_490_sp23-0.1.3/README.md
+-rw-r--r--   0        0        0     1268 2023-04-23 19:14:47.967915 uiuc_490_sp23-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1421 2023-04-17 23:16:11.816377 uiuc_490_sp23-0.1.3/uiuc_490_sp23/Constraints/__init__.py
+-rw-r--r--   0        0        0      245 2023-02-20 13:45:18.963614 uiuc_490_sp23-0.1.3/uiuc_490_sp23/Exceptions/__init__.py
+-rw-r--r--   0        0        0     1893 2023-04-17 23:16:08.475996 uiuc_490_sp23-0.1.3/uiuc_490_sp23/LineSearch/__init__.py
+-rw-r--r--   0        0        0     1048 2023-04-17 23:16:11.820377 uiuc_490_sp23-0.1.3/uiuc_490_sp23/Optimizers/__init__.py
+-rw-r--r--   0        0        0     4665 2023-04-23 19:13:14.093197 uiuc_490_sp23-0.1.3/uiuc_490_sp23/Problem/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-20 13:45:18.963614 uiuc_490_sp23-0.1.3/uiuc_490_sp23/__init__.py
+-rw-r--r--   0        0        0      341 2023-04-22 20:50:56.404666 uiuc_490_sp23-0.1.3/uiuc_490_sp23/__main__.py
+-rw-r--r--   0        0        0   128193 2023-02-20 13:45:18.967611 uiuc_490_sp23-0.1.3/uiuc_490_sp23/assignment1/Lab1_sp2023.pdf
+-rw-r--r--   0        0        0        0 2023-02-20 13:45:18.967611 uiuc_490_sp23-0.1.3/uiuc_490_sp23/assignment1/__init__.py
+-rwxr-xr-x   0        0        0     4133 2023-04-23 19:10:35.984349 uiuc_490_sp23-0.1.3/uiuc_490_sp23/assignment1/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-22 20:37:33.301931 uiuc_490_sp23-0.1.3/uiuc_490_sp23/assignment2/__init__.py
+-rw-r--r--   0        0        0     1140 2023-04-23 19:08:59.791032 uiuc_490_sp23-0.1.3/uiuc_490_sp23/assignment2/__main__.py
+-rw-r--r--   0        0        0     1193 2023-03-22 22:14:55.796323 uiuc_490_sp23-0.1.3/uiuc_490_sp23/assignment2/asgn_source.py
+-rwxr-xr-x   0        0        0     3601 2023-04-22 20:40:28.895119 uiuc_490_sp23-0.1.3/uiuc_490_sp23/assignment2/newtons.py
+-rwxr-xr-x   0        0        0     3442 2023-04-22 21:05:25.112734 uiuc_490_sp23-0.1.3/uiuc_490_sp23/assignment2/projected_gd.py
+-rw-r--r--   0        0        0        0 2023-04-17 23:16:11.820377 uiuc_490_sp23-0.1.3/uiuc_490_sp23/assignment3/__init__.py
+-rw-r--r--   0        0        0     4926 2023-04-23 19:12:01.778467 uiuc_490_sp23-0.1.3/uiuc_490_sp23/assignment3/__main__.py
+-rw-r--r--   0        0        0     2794 1970-01-01 00:00:00.000000 uiuc_490_sp23-0.1.3/setup.py
+-rw-r--r--   0        0        0     2663 1970-01-01 00:00:00.000000 uiuc_490_sp23-0.1.3/PKG-INFO
```

### Comparing `uiuc_490_sp23-0.1.1/LICENSE` & `uiuc_490_sp23-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `uiuc_490_sp23-0.1.1/pyproject.toml` & `uiuc_490_sp23-0.1.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uiuc-490-sp23"
-version = "0.1.1"
+version = "0.1.3"
 license = "GPL-3.0-or-later"
 description = "Programming assignments for UIUC's ECE490: Introduction to Optimization course during Spring 2023"
 authors = ["Eric Silk <eric.silk@ericsilk.com>"]
 readme = "README.md"
 homepage = "https://github.com/eric-silk/ECE490"
 repository = "https://github.com/eric-silk/ECE490"
 keywords = ["optimization"]
@@ -19,20 +19,24 @@
 ]
 packages = [{include = "uiuc_490_sp23"}]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/eric-silk/ECE490/issues"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = ">=3.10,<3.12"
 numpy = "^1.24.2"
+matplotlib = "^3.7.1"
+scipy = "^1.10.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 pylint = "^2.16.1"
 
 [tool.poetry.scripts]
 assignment1 = "assignment1:__main__"
+assignment2 = "assignment2:__main__"
+assignment3 = "assignment3:__main__"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `uiuc_490_sp23-0.1.1/uiuc_490_sp23/LineSearch/__init__.py` & `uiuc_490_sp23-0.1.3/uiuc_490_sp23/LineSearch/__init__.py`

 * *Files identical despite different names*

### Comparing `uiuc_490_sp23-0.1.1/uiuc_490_sp23/Optimizers/__init__.py` & `uiuc_490_sp23-0.1.3/uiuc_490_sp23/Optimizers/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 
 
 class Optimizer(ABC):
     @abstractmethod
     def step(self, x: np.ndarray, debug: bool = False) -> np.ndarray:
         pass
 
+    def __call__(self, x: np.ndarray, debug: bool = False) -> np.ndarray:
+        return self.step(x, debug=debug)
+
 
 class GradientDescent(Optimizer):
     def __init__(self, f: Problem, line_search: LineSearch) -> None:
         self.f = f
         self.line_search = line_search
 
     def step(self, x: np.ndarray, debug: bool = False) -> np.ndarray:
```

### Comparing `uiuc_490_sp23-0.1.1/uiuc_490_sp23/assignment1/Lab1_sp2023.pdf` & `uiuc_490_sp23-0.1.3/uiuc_490_sp23/assignment1/Lab1_sp2023.pdf`

 * *Files identical despite different names*

### Comparing `uiuc_490_sp23-0.1.1/uiuc_490_sp23/assignment1/__main__.py` & `uiuc_490_sp23-0.1.3/uiuc_490_sp23/assignment1/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,41 +33,43 @@
             break
     else:
         t1 = time.time()
         print(f"Failed to converge in {max_iter} iterations! Ran for {t1-t0} seconds.")
 
     print(f"x*:\n{xk}\nf(x*): {f(xk)[0]}, ||∇f(x*)||: {norm}")
 
+
 def _directly_calculate_minimizer(f: QuadraticForm) -> None:
     """
     Given a Quadratic Form problem, directly solve for the minimum.
     args:
         f: A QuadraticForm Problem object.
     """
     Q = f.get_Q()
     b = f.get_b()
     # The quadratic form is normally listed as (1/2)(x^T Q x) - bx + c with a minimizer at Qx=b
     # However, our problem is of the form x^T Q x + bx + c, so we need to solve 2Qx = -b
-    x_star = np.linalg.lstsq(2*Q,-b,rcond=None)[0]
+    x_star = np.linalg.lstsq(2 * Q, -b, rcond=None)[0]
     grad_norm = np.linalg.norm(f.gradient(x_star))
 
     print(f"x*:\n{x_star}\nf(x*): {f(x_star)[0]}, ||∇f(x*)||: {grad_norm}")
 
-def _calculate_optimal_alpha(f: QuadraticForm, scaling: float=0.99) -> float:
+
+def _calculate_optimal_alpha(f: QuadraticForm, scaling: float = 0.99) -> float:
     """
     Given a QuadraticForm problem, determine the optimal stepsize alpha.
     args:
         f: a QuadraticForm problem
         scaling: We need alpha < 2/L, so calculate 2/L and scale it by this value (default=0.99)
     """
-    Q = 2*f.get_Q()
+    Q = 2 * f.get_Q()
     s = np.linalg.svd(Q, compute_uv=False)
     L = np.max(s).item()
     # Make it just slightly less than 2/L
-    alpha = (2/L)*0.99
+    alpha = (2 / L) * 0.99
     print("alpha:", alpha)
     return alpha
 
 
 def assignment1(seed: int, epsilon: float, n: int, max_iter: int) -> None:
     np.set_printoptions(linewidth=1000)
     np.random.seed(seed)
@@ -79,28 +81,38 @@
         f,
         Backtracking(f, 1.0, 0.1, 0.5),
     )
 
     x0 = np.random.random(n)
 
     print(f"ε: {epsilon}")
-    print("="*80)
+    print("=" * 80)
     _do_optimization(f, gradient_descent_fixed_alpha, x0, epsilon, max_iter=max_iter)
-    print("="*80)
+    print("=" * 80)
     _do_optimization(f, gradient_descent_armijo, x0, epsilon, max_iter=max_iter)
-    print("="*80)
+    print("=" * 80)
     _directly_calculate_minimizer(f)
 
 
 if __name__ == "__main__":
     import argparse
 
-    parser = argparse.ArgumentParser()
+    parser = argparse.ArgumentParser(
+        prog="assignment1",
+        description=(
+            "A basic Gradient Descent implementation to "
+            "solve a randomly generated quadratic problem"
+        ),
+    )
     parser.add_argument(
-        "-s", "--seed", type=int, default=1234, help="The seed to use for randomization (default=1234)"
+        "-s",
+        "--seed",
+        type=int,
+        default=1234,
+        help="The seed to use for randomization (default=1234)",
     )
     parser.add_argument(
         "-e",
         "--epsilon",
         type=float,
         default=1e-6,
         help="Optimization convergence tolerance (float, >=0, default=1e-6)",
```

