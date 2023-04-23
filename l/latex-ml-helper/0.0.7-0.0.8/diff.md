# Comparing `tmp/latex_ml_helper-0.0.7.tar.gz` & `tmp/latex_ml_helper-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latex_ml_helper-0.0.7.tar", last modified: Sun Apr 23 20:13:59 2023, max compression
+gzip compressed data, was "latex_ml_helper-0.0.8.tar", last modified: Sun Apr 23 20:32:25 2023, max compression
```

## Comparing `latex_ml_helper-0.0.7.tar` & `latex_ml_helper-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 20:13:59.665432 latex_ml_helper-0.0.7/
--rw-rw-rw-   0        0        0      657 2023-04-23 20:13:59.665432 latex_ml_helper-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-23 20:13:59.660433 latex_ml_helper-0.0.7/latex_ml_helper.egg-info/
--rw-rw-rw-   0        0        0      657 2023-04-23 20:13:59.000000 latex_ml_helper-0.0.7/latex_ml_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-04-23 20:13:59.000000 latex_ml_helper-0.0.7/latex_ml_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 20:13:59.000000 latex_ml_helper-0.0.7/latex_ml_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-23 20:13:59.000000 latex_ml_helper-0.0.7/latex_ml_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-23 20:13:59.000000 latex_ml_helper-0.0.7/latex_ml_helper.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-23 20:13:59.664432 latex_ml_helper-0.0.7/libraries/
--rw-rw-rw-   0        0        0      464 2023-04-23 20:03:19.000000 latex_ml_helper-0.0.7/libraries/__init__.py
--rw-rw-rw-   0        0        0      168 2023-04-16 17:40:17.000000 latex_ml_helper-0.0.7/libraries/copy.py
--rw-rw-rw-   0        0        0     4507 2023-04-17 09:54:52.000000 latex_ml_helper-0.0.7/libraries/definitions.py
--rw-rw-rw-   0        0        0     1689 2023-04-23 20:13:16.000000 latex_ml_helper-0.0.7/libraries/otup.py
--rw-rw-rw-   0        0        0     8350 2023-04-17 10:56:51.000000 latex_ml_helper-0.0.7/libraries/snippets.py
--rw-rw-rw-   0        0        0       42 2023-04-23 20:13:59.665432 latex_ml_helper-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      917 2023-04-23 20:13:53.000000 latex_ml_helper-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 20:32:25.078779 latex_ml_helper-0.0.8/
+-rw-rw-rw-   0        0        0      657 2023-04-23 20:32:25.077779 latex_ml_helper-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-23 20:32:25.073779 latex_ml_helper-0.0.8/latex_ml_helper.egg-info/
+-rw-rw-rw-   0        0        0      657 2023-04-23 20:32:25.000000 latex_ml_helper-0.0.8/latex_ml_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-04-23 20:32:25.000000 latex_ml_helper-0.0.8/latex_ml_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 20:32:25.000000 latex_ml_helper-0.0.8/latex_ml_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-23 20:32:25.000000 latex_ml_helper-0.0.8/latex_ml_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-23 20:32:25.000000 latex_ml_helper-0.0.8/latex_ml_helper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 20:32:25.077779 latex_ml_helper-0.0.8/libraries/
+-rw-rw-rw-   0        0        0      490 2023-04-23 20:31:50.000000 latex_ml_helper-0.0.8/libraries/__init__.py
+-rw-rw-rw-   0        0        0      168 2023-04-16 17:40:17.000000 latex_ml_helper-0.0.8/libraries/copy.py
+-rw-rw-rw-   0        0        0     4507 2023-04-17 09:54:52.000000 latex_ml_helper-0.0.8/libraries/definitions.py
+-rw-rw-rw-   0        0        0     2360 2023-04-23 20:31:04.000000 latex_ml_helper-0.0.8/libraries/otup.py
+-rw-rw-rw-   0        0        0     8350 2023-04-17 10:56:51.000000 latex_ml_helper-0.0.8/libraries/snippets.py
+-rw-rw-rw-   0        0        0       42 2023-04-23 20:32:25.078779 latex_ml_helper-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      917 2023-04-23 20:32:03.000000 latex_ml_helper-0.0.8/setup.py
```

### Comparing `latex_ml_helper-0.0.7/PKG-INFO` & `latex_ml_helper-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latex_ml_helper
-Version: 0.0.7
+Version: 0.0.8
 Summary: Package for getting latex equations for machine learning models
 Home-page: UNKNOWN
 Author: Ramal Salha
 Author-email: <ramal.salha@gmail.com>
 License: UNKNOWN
 Keywords: python,video,stream,video stream,camera stream,sockets
 Platform: UNKNOWN
```

### Comparing `latex_ml_helper-0.0.7/latex_ml_helper.egg-info/PKG-INFO` & `latex_ml_helper-0.0.8/latex_ml_helper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latex-ml-helper
-Version: 0.0.7
+Version: 0.0.8
 Summary: Package for getting latex equations for machine learning models
 Home-page: UNKNOWN
 Author: Ramal Salha
 Author-email: <ramal.salha@gmail.com>
 License: UNKNOWN
 Keywords: python,video,stream,video stream,camera stream,sockets
 Platform: UNKNOWN
```

### Comparing `latex_ml_helper-0.0.7/libraries/definitions.py` & `latex_ml_helper-0.0.8/libraries/definitions.py`

 * *Files identical despite different names*

### Comparing `latex_ml_helper-0.0.7/libraries/otup.py` & `latex_ml_helper-0.0.8/libraries/otup.py`

 * *Files 27% similar despite different names*

```diff
@@ -72,19 +72,56 @@
     text = """
 s = symbols("s")
 G = C * (s * eye(A.shape[0]) - A) ** (-1) * B
 simplify(G)
 """
     return text
 
+def e_At():
+    text = """
+t = symbols('t')
+At = t * A
+At.exp()  # e^tA
+"""
+    return text
+
+def solution():
+    text = """
+x = symbols('x')
+expr = (x + 2) * (x - 3)
+
+
+sol = solve(expr)
+
+sol[1], sol[0]
+"""
+
+    return text
+
+def lyapunov():
+    text = """
+P = Matrix(lyap(Transpose(A),eye(4)))
+# Postoji pozitivno definitna, simetrična P...
+print(P.eigenvals())
+P  
+# -> Sustav je stabilan jer postoji takva P simetrična, pozitivno definitna.
+
+# ... takva da je: A'*P+P*A=-I.  (Provjera)
+Transpose(A)*P+P*A # <- mora bit jedinicna matrica
+"""
+    return text
+
 def help_otup():
     text = """
 Imports() <- import libraries
 graphic_solution() <- graphic solution u = [1, 2]
 graphic_solution2() <- graphic solution u = 0.5
 C_m() <- controllability matrix
 jordan_form_solution() <- jordan form
 tf() <- transfer function
 tf2() <- transfer function custom
+e_At() <- e^At
+solution() <- rjesavanje jednadzbi
+lyapunov() <- lyapunov
 """
 
     return text
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `latex_ml_helper-0.0.7/libraries/snippets.py` & `latex_ml_helper-0.0.8/libraries/snippets.py`

 * *Files identical despite different names*

### Comparing `latex_ml_helper-0.0.7/setup.py` & `latex_ml_helper-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'Package for getting latex equations for machine learning models'
 
 # Setting up
 setup(
     name="latex_ml_helper",
     version=VERSION,
     author="Ramal Salha",
```

