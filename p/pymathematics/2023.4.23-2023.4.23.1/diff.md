# Comparing `tmp/pymathematics-2023.4.23.tar.gz` & `tmp/pymathematics-2023.4.23.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymathematics-2023.4.23.tar", last modified: Sun Apr 23 05:56:44 2023, max compression
+gzip compressed data, was "pymathematics-2023.4.23.1.tar", last modified: Sun Apr 23 06:56:34 2023, max compression
```

## Comparing `pymathematics-2023.4.23.tar` & `pymathematics-2023.4.23.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-23 05:56:44.229373 pymathematics-2023.4.23/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     1088 2023-04-16 06:03:02.000000 pymathematics-2023.4.23/LICENSE
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-23 05:56:44.218374 pymathematics-2023.4.23/PKG-INFO
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      123 2023-04-23 05:53:29.000000 pymathematics-2023.4.23/README.md
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-23 05:56:43.909348 pymathematics-2023.4.23/pymathematics/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)    17355 2023-04-23 02:56:55.000000 pymathematics-2023.4.23/pymathematics/__init__.py
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      111 2023-04-22 15:29:04.000000 pymathematics-2023.4.23/pymathematics/info.py
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-23 05:56:44.155743 pymathematics-2023.4.23/pymathematics.egg-info/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-23 05:56:40.000000 pymathematics-2023.4.23/pymathematics.egg-info/PKG-INFO
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      222 2023-04-23 05:56:40.000000 pymathematics-2023.4.23/pymathematics.egg-info/SOURCES.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        1 2023-04-23 05:56:40.000000 pymathematics-2023.4.23/pymathematics.egg-info/dependency_links.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       14 2023-04-23 05:56:40.000000 pymathematics-2023.4.23/pymathematics.egg-info/top_level.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       38 2023-04-23 05:56:44.233370 pymathematics-2023.4.23/setup.cfg
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      689 2023-04-23 05:53:24.000000 pymathematics-2023.4.23/setup.py
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-23 06:56:34.095297 pymathematics-2023.4.23.1/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     1088 2023-04-16 06:03:02.000000 pymathematics-2023.4.23.1/LICENSE
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      509 2023-04-23 06:56:34.087298 pymathematics-2023.4.23.1/PKG-INFO
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      125 2023-04-23 06:52:17.000000 pymathematics-2023.4.23.1/README.md
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-23 06:56:33.800295 pymathematics-2023.4.23.1/pymathematics/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)    18612 2023-04-23 06:50:52.000000 pymathematics-2023.4.23.1/pymathematics/__init__.py
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      113 2023-04-23 06:51:57.000000 pymathematics-2023.4.23.1/pymathematics/info.py
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-23 06:56:34.028296 pymathematics-2023.4.23.1/pymathematics.egg-info/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      509 2023-04-23 06:56:31.000000 pymathematics-2023.4.23.1/pymathematics.egg-info/PKG-INFO
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      222 2023-04-23 06:56:31.000000 pymathematics-2023.4.23.1/pymathematics.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        1 2023-04-23 06:56:31.000000 pymathematics-2023.4.23.1/pymathematics.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       14 2023-04-23 06:56:31.000000 pymathematics-2023.4.23.1/pymathematics.egg-info/top_level.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       38 2023-04-23 06:56:34.097298 pymathematics-2023.4.23.1/setup.cfg
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      691 2023-04-23 06:52:12.000000 pymathematics-2023.4.23.1/setup.py
```

### Comparing `pymathematics-2023.4.23/LICENSE` & `pymathematics-2023.4.23.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymathematics-2023.4.23/pymathematics/__init__.py` & `pymathematics-2023.4.23.1/pymathematics/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,37 @@
             raise ValueError("vector should have 3 directions")
         return vector.dot_product(vector1,vector2)/vector.magnitude(vector2)
 
     def angle_of_projection(vector1:list,vector2:list) -> float:
         return f"arccos({vector.dot_product(vector1,vector2)}/{(vector.magnitude(vector1)*vector.magnitude(vector2))})"
 
 class matrix:
+    def ismatrix(matrix_):
+        if not isinstance(matrix_, list):
+            return False
+        if not all(isinstance(row, list) for row in matrix_):
+            return False
+        row_lengths = [len(row) for row in matrix_]
+        if not all(length == row_lengths[0] for length in row_lengths):
+            return False
+        return True
+    
+    def shape(matrix_):
+        if matrix.ismatrix(matrix_) == False:
+            raise ValueError("elements of each rows aren't the same")
+        return len(matrix_),len(matrix_[0])
+    
+    def size(matrix_):
+        if matrix.ismatrix(matrix_) == False:
+            raise ValueError("elements of each rows aren't the same")
+        return len(matrix_)*len(matrix_[0])
+
     def determinant(matrix_):
+        if matrix.ismatrix(matrix_) == False:
+            raise ValueError("elements of each rows aren't the same")
         if len(matrix_) == 1:
             return matrix_[0][0]
         elif len(matrix_) == 2:
             return matrix_[0][0]*matrix_[1][1]-matrix_[0][1]*matrix_[1][0]
         det = 0
         for x in range(len(matrix_)):
             minor = []
@@ -55,14 +77,16 @@
                     if z != x:
                         row.append(matrix_[y][z])
                 minor.append(row)
             det += (-1)**x*matrix_[0][x]*matrix.determinant(minor)
         return det
     
     def inverse(matrix_):
+        if matrix.ismatrix(matrix_) == False:
+            raise ValueError("elements of each rows aren't the same")
         identity = [[0 if x != y else 1 for y in range(len(matrix_))] for x in range(len(matrix_))]
         for x in range(len(matrix_)):
             pivot = matrix_[x][x]
             for y in range(len(matrix_)):
                 matrix_[x][y] /= pivot
                 identity[x][y] /= pivot
             for y in range(len(matrix_)):
@@ -70,23 +94,27 @@
                     factor = matrix_[y][x]
                     for k in range(len(matrix_)):
                         matrix_[y][k] -= factor * matrix_[x][k]
                         identity[y][k] -= factor * identity[x][k]
         return identity
     
     def transpose(matrix_):
+        if matrix.ismatrix(matrix_) == False:
+            raise ValueError("elements of each rows aren't the same")
         rows = len(matrix_)
         cols = len(matrix_[0])
         res = [[0 for y in range(rows)]for x in range(cols)]
         for x in range(rows):
             for y in range(cols):
                 res[y][x] = matrix_[x][y]   
         return res
     
     def product(matrix1,matrix2):
+        if matrix.ismatrix(matrix1) == False or matrix.ismatrix(matrix2) == False:
+            raise ValueError("elements of each rows aren't the same")
         rows1 = len(matrix1)
         cols1 = len(matrix1[0])
         rows2 = len(matrix2)
         cols2 = len(matrix2[0])
         if cols1 != rows2:
             raise ValueError("number of columns of a first matrix should be equal to the rows of the second matrix")
         result = [[0 for y in range(cols2)] for x in range(rows1)]
```

### Comparing `pymathematics-2023.4.23/setup.py` & `pymathematics-2023.4.23.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 
 setup(
     name = "pymathematics",
-    version = "2023.4.23",
+    version = "2023.4.23.1",
     description = "package for mathematics",
     long_description = "for more info, check the github repository",
     author = "Sahil Rajwar",
     maintainer = "its_Sahil",
     author_email = "justsahilrajwar2004@gmail.com",
     packages = ["pymathematics"],
     license = "MIT",
```

