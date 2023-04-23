# Comparing `tmp/hpc-utils-0.1.0.tar.gz` & `tmp/hpc-utils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpc-utils-0.1.0.tar", last modified: Sun Apr  9 12:21:31 2023, max compression
+gzip compressed data, was "hpc-utils-0.1.1.tar", last modified: Sun Apr 23 02:39:03 2023, max compression
```

## Comparing `hpc-utils-0.1.0.tar` & `hpc-utils-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 12:21:31.566861 hpc-utils-0.1.0/
--rw-rw-rw-   0        0        0      173 2022-03-20 16:23:15.000000 hpc-utils-0.1.0/AUTHORS.rst
--rw-rw-rw-   0        0        0    35591 2022-03-20 16:22:07.000000 hpc-utils-0.1.0/LICENSE.md
--rw-rw-rw-   0        0        0     6122 2023-04-09 12:21:31.566861 hpc-utils-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5093 2023-03-30 17:38:58.000000 hpc-utils-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 12:21:31.553849 hpc-utils-0.1.0/hpc/
--rw-rw-rw-   0        0        0     1041 2023-03-30 19:46:38.000000 hpc-utils-0.1.0/hpc/__init__.py
--rw-rw-rw-   0        0        0     5063 2023-03-31 23:01:20.000000 hpc-utils-0.1.0/hpc/filter.py
-drwxrwxrwx   0        0        0        0 2023-04-09 12:21:31.563478 hpc-utils-0.1.0/hpc_utils.egg-info/
--rw-rw-rw-   0        0        0     6122 2023-04-09 12:21:31.000000 hpc-utils-0.1.0/hpc_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-04-09 12:21:31.000000 hpc-utils-0.1.0/hpc_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 12:21:31.000000 hpc-utils-0.1.0/hpc_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-09 12:21:31.000000 hpc-utils-0.1.0/hpc_utils.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       26 2023-04-09 12:21:31.000000 hpc-utils-0.1.0/hpc_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-09 12:21:31.000000 hpc-utils-0.1.0/hpc_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 12:21:31.566861 hpc-utils-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1656 2023-04-09 12:20:59.000000 hpc-utils-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-09 12:21:31.564484 hpc-utils-0.1.0/tests/
--rw-rw-rw-   0        0        0     7151 2023-04-09 12:07:45.000000 hpc-utils-0.1.0/tests/test_array.py
+drwxrwxrwx   0        0        0        0 2023-04-23 02:39:03.548638 hpc-utils-0.1.1/
+-rw-rw-rw-   0        0        0      173 2022-03-20 16:23:15.000000 hpc-utils-0.1.1/AUTHORS.rst
+-rw-rw-rw-   0        0        0    35591 2022-03-20 16:22:07.000000 hpc-utils-0.1.1/LICENSE.md
+-rw-rw-rw-   0        0        0     5886 2023-04-23 02:39:03.547637 hpc-utils-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4784 2023-04-23 02:28:26.000000 hpc-utils-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 02:39:03.535595 hpc-utils-0.1.1/hpc/
+-rw-rw-rw-   0        0        0     1041 2023-03-30 19:46:38.000000 hpc-utils-0.1.1/hpc/__init__.py
+-rw-rw-rw-   0        0        0     5374 2023-04-23 02:05:20.000000 hpc-utils-0.1.1/hpc/indexing.py
+drwxrwxrwx   0        0        0        0 2023-04-23 02:39:03.543636 hpc-utils-0.1.1/hpc_utils.egg-info/
+-rw-rw-rw-   0        0        0     5886 2023-04-23 02:39:03.000000 hpc-utils-0.1.1/hpc_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2023-04-23 02:39:03.000000 hpc-utils-0.1.1/hpc_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 02:39:03.000000 hpc-utils-0.1.1/hpc_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-23 02:39:03.000000 hpc-utils-0.1.1/hpc_utils.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       26 2023-04-23 02:39:03.000000 hpc-utils-0.1.1/hpc_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-23 02:39:03.000000 hpc-utils-0.1.1/hpc_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 02:39:03.548638 hpc-utils-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1638 2023-04-23 02:25:59.000000 hpc-utils-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 02:39:03.544636 hpc-utils-0.1.1/tests/
+-rw-rw-rw-   0        0        0     7886 2023-04-23 01:07:34.000000 hpc-utils-0.1.1/tests/test_array.py
```

### Comparing `hpc-utils-0.1.0/LICENSE.md` & `hpc-utils-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hpc-utils-0.1.0/hpc/__init__.py` & `hpc-utils-0.1.1/hpc/__init__.py`

 * *Files identical despite different names*

### Comparing `hpc-utils-0.1.0/hpc/filter.py` & `hpc-utils-0.1.1/hpc/indexing.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     i, j = get_indices(mask, mask_val)
     # get the coresponding values to the indeces from the array
     vals = arr[i, j] if arr.ndim == 2 else arr[:, i, j]
     return vals
 
 
-def get_indices2(arr: np.ndarray, mask: List) -> List[Tuple[int, int]]:
+def get_indices2(arr: np.ndarray, mask: List = None) -> List[Tuple[int, int]]:
     """Get Indeces
 
         - get the indeces of array cells after filtering the values based on two mask values
 
     Parameters
     ----------
     arr: [np.ndarray]
@@ -92,32 +92,40 @@
         rows = arr.shape[0]
         cols = arr.shape[1]
         ind = [(i, j) for i in range(rows) for j in range(cols)]
 
     return ind
 
 
-def get_pixels2(arr: np.ndarray, mask: List) -> List:
+def get_pixels2(arr: np.ndarray, mask: List = None) -> np.ndarray:
     """Get pixels from a raster (with optional mask).
 
     Parameters
     ----------
     arr : [np.ndarray]
         Array of raster data in the form [y][x].
     mask : [np.ndarray]
         Array (2D) of zeroes to mask data.(from the rastarizing the vector)
 
     Returns
     -------
     np.ndarray
         Array of non-masked data.
     """
-    ind = get_indices2(arr, mask)
-    fn = lambda x: arr[x[0], x[1]]
-    values = list(map(fn, ind))
+    if arr.ndim == 2:
+        ind = get_indices2(arr, mask)
+        fn = lambda x: arr[x[0], x[1]]
+        values = np.fromiter(map(fn, ind), dtype=arr.dtype)
+    else:
+        ind = get_indices2(arr[0, :, :], mask)
+        fn = lambda x: arr[:, x[0], x[1]]
+        values = list(map(fn, ind))
+        values = np.array(values, dtype=arr.dtype)
+        values = values.transpose()
+
     return values
 
 
 def locate_values(values: np.ndarray, grid_x: np.ndarray, grid_y: np.ndarray):
     """Locate values in an array
 
         locate a value in array, each point has to values (resembling the x & y coordinates), the values array
@@ -155,14 +163,15 @@
     -------
     array:
         array with a shape (any, 2), for the row, column indices in the array.
         array([[ 5,  4],
                [ 2,  9],
                [ 5,  9]])
     """
+
     def find(point_i):
         x_ind = np.abs(point_i[0] - grid_x).argmin()
         y_ind = np.abs(point_i[1] - grid_y).argmin()
         return x_ind, y_ind
 
     indices = np.array(list(map(find, values)))
```

### Comparing `hpc-utils-0.1.0/setup.py` & `hpc-utils-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,23 +7,23 @@
     history = history_file.read()
 
 requirements = [line.strip() for line in open("requirements.txt").readlines()]
 requirements_dev = [line.strip() for line in open("requirements-dev.txt").readlines()]
 
 setup(
     name="hpc-utils",
-    version="0.1.0",
+    version="0.1.1",
     description="numpy utility package",
     author="Mostafa Farrag",
     author_email="moah.farag@gmail.come",
-    url="https://github.com/MAfarrag/numpy-utils",
+    url="https://github.com/MAfarrag/hpc",
     keywords=["numpy", "computation"],
     long_description=readme + "\n\n" + history,
-    repository="https://github.com/MAfarrag/numpy-utils",
-    documentation="https://numpy-utils.readthedocs.io/",
+    repository="https://github.com/MAfarrag/hpc",
+    documentation="https://hpc-utils.readthedocs.io/",
     long_description_content_type="text/markdown",
     license="GNU General Public License v3",
     zip_safe=False,
     packages=find_packages(include=["hpc", "hpc.*"]),
     test_suite="tests",
     tests_require=requirements_dev,
     install_requires=requirements,
```

