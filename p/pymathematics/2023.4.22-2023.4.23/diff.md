# Comparing `tmp/pymathematics-2023.4.22.tar.gz` & `tmp/pymathematics-2023.4.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymathematics-2023.4.22.tar", last modified: Sat Apr 22 07:24:41 2023, max compression
+gzip compressed data, was "pymathematics-2023.4.23.tar", last modified: Sun Apr 23 05:56:44 2023, max compression
```

## Comparing `pymathematics-2023.4.22.tar` & `pymathematics-2023.4.23.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-22 07:24:41.275465 pymathematics-2023.4.22/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     1088 2023-04-16 06:03:02.000000 pymathematics-2023.4.22/LICENSE
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-22 07:24:41.261462 pymathematics-2023.4.22/PKG-INFO
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      123 2023-04-22 05:45:25.000000 pymathematics-2023.4.22/README.md
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-22 07:24:40.891632 pymathematics-2023.4.22/pymathematics/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)    16853 2023-04-22 05:47:49.000000 pymathematics-2023.4.22/pymathematics/__init__.py
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      111 2023-04-22 05:44:53.000000 pymathematics-2023.4.22/pymathematics/info.py
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-22 07:24:41.186885 pymathematics-2023.4.22/pymathematics.egg-info/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-22 07:24:35.000000 pymathematics-2023.4.22/pymathematics.egg-info/PKG-INFO
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      222 2023-04-22 07:24:36.000000 pymathematics-2023.4.22/pymathematics.egg-info/SOURCES.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        1 2023-04-22 07:24:35.000000 pymathematics-2023.4.22/pymathematics.egg-info/dependency_links.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       14 2023-04-22 07:24:35.000000 pymathematics-2023.4.22/pymathematics.egg-info/top_level.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       38 2023-04-22 07:24:41.278461 pymathematics-2023.4.22/setup.cfg
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      689 2023-04-22 05:45:13.000000 pymathematics-2023.4.22/setup.py
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-23 05:56:44.229373 pymathematics-2023.4.23/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     1088 2023-04-16 06:03:02.000000 pymathematics-2023.4.23/LICENSE
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-23 05:56:44.218374 pymathematics-2023.4.23/PKG-INFO
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      123 2023-04-23 05:53:29.000000 pymathematics-2023.4.23/README.md
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-23 05:56:43.909348 pymathematics-2023.4.23/pymathematics/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)    17355 2023-04-23 02:56:55.000000 pymathematics-2023.4.23/pymathematics/__init__.py
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      111 2023-04-22 15:29:04.000000 pymathematics-2023.4.23/pymathematics/info.py
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-23 05:56:44.155743 pymathematics-2023.4.23/pymathematics.egg-info/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-23 05:56:40.000000 pymathematics-2023.4.23/pymathematics.egg-info/PKG-INFO
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      222 2023-04-23 05:56:40.000000 pymathematics-2023.4.23/pymathematics.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        1 2023-04-23 05:56:40.000000 pymathematics-2023.4.23/pymathematics.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       14 2023-04-23 05:56:40.000000 pymathematics-2023.4.23/pymathematics.egg-info/top_level.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       38 2023-04-23 05:56:44.233370 pymathematics-2023.4.23/setup.cfg
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      689 2023-04-23 05:53:24.000000 pymathematics-2023.4.23/setup.py
```

### Comparing `pymathematics-2023.4.22/LICENSE` & `pymathematics-2023.4.23/LICENSE`

 * *Files identical despite different names*

### Comparing `pymathematics-2023.4.22/pymathematics/__init__.py` & `pymathematics-2023.4.23/pymathematics/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,39 @@
     author = author
     version = version
     homepage = homepage
 
 class constants:
     pi = 3.1415926535897932384626433832795
     e = 2.7182818284590452353602874713527
+    inf = infinity = float("inf")
+    nan = NaN = float("nan")
 
 class vector:
     def cross_product(vector1:list,vector2:list) -> int|float:
+        if len(vector1) != 3 or len(vector2) != 3:
+            raise ValueError("vector should have 3 directions")
         return [vector1[1]*vector2[2]-vector2[1]*vector1[2],-(vector1[0]*vector2[2]-vector2[0]*vector1[2]),vector1[0]*vector2[1]-vector2[0]*vector1[1]]
 
     def dot_product(vector1:list,vector2:list) -> int|float:
+        if len(vector1) != 3 or len(vector2) != 3:
+            raise ValueError("vector should have 3 directions")
         return vector1[0]*vector2[0]+vector1[1]*vector2[1]+vector1[2]*vector2[2]
 
     def magnitude(vector) -> int|float:
+        if len(vector) != 3:
+            raise ValueError("vector should have 3 directions")
         return sqrt(vector[0]**2+vector[1]**2+vector[2]**2)
 
     def projection(vector1:list,vector2:list) -> int|float:
         """
         `projection of vector1 to vector2`
         """
+        if len(vector1) != 3 or len(vector2) != 3:
+            raise ValueError("vector should have 3 directions")
         return vector.dot_product(vector1,vector2)/vector.magnitude(vector2)
 
     def angle_of_projection(vector1:list,vector2:list) -> float:
         return f"arccos({vector.dot_product(vector1,vector2)}/{(vector.magnitude(vector1)*vector.magnitude(vector2))})"
 
 class matrix:
     def determinant(matrix_):
@@ -100,15 +110,15 @@
         A = sets.toset(A)
         B = sets.toset(B)
         for x in B:
             if x not in A:
                 A.append(x)
         return quick_sort(A)
 
-    def intercept(A:list,B:list) -> list:
+    def intersect(A:list,B:list) -> list:
         res = []
         A = sets.toset(A)
         B = sets.toset(B)
         for i in B:
             if i in A:
                 res.append(i)
         if len(res) == 0:
@@ -186,15 +196,15 @@
     if number < 0:
         return "undefined"
     elif number == 0:
         return 0
     flag = number/2
     while absolute(flag*flag - number) > 0.00001:
         flag = (flag + number/flag)/2
-    return round(flag,5)
+    return flag
 
 def quadratic_roots(coefficients:list) -> list:
     if len(coefficients) != 3:
         raise ValueError("there should be only 3 coefficients!")
     D = coefficients[0]**2-4*coefficients[0]*coefficients[2]
     if D < 0:
         x1 = f"{-coefficients[1]} + {sqrt(absolute(D))}i"
```

### Comparing `pymathematics-2023.4.22/setup.py` & `pymathematics-2023.4.23/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 
 setup(
     name = "pymathematics",
-    version = "2023.4.22",
+    version = "2023.4.23",
     description = "package for mathematics",
     long_description = "for more info, check the github repository",
     author = "Sahil Rajwar",
     maintainer = "its_Sahil",
     author_email = "justsahilrajwar2004@gmail.com",
     packages = ["pymathematics"],
     license = "MIT",
```

