# Comparing `tmp/precession-2.0.0.dev0.tar.gz` & `tmp/precession-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "precession-2.0.0.dev0.tar", last modified: Mon Apr 10 12:57:13 2023, max compression
+gzip compressed data, was "precession-2.0.1.tar", last modified: Sun Apr 23 18:52:59 2023, max compression
```

## Comparing `precession-2.0.0.dev0.tar` & `precession-2.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dgerosa    (501) staff       (20)        0 2023-04-10 12:57:13.897329 precession-2.0.0.dev0/
--rw-r--r--   0 dgerosa    (501) staff       (20)     1071 2022-02-03 16:32:40.000000 precession-2.0.0.dev0/LICENSE
--rw-r--r--   0 dgerosa    (501) staff       (20)       24 2023-04-08 16:44:47.000000 precession-2.0.0.dev0/MANIFEST.in
--rw-r--r--   0 dgerosa    (501) staff       (20)      469 2023-04-10 12:57:13.896834 precession-2.0.0.dev0/PKG-INFO
--rw-r--r--   0 dgerosa    (501) staff       (20)     2755 2023-04-10 07:58:58.000000 precession-2.0.0.dev0/README.md
-drwxr-xr-x   0 dgerosa    (501) staff       (20)        0 2023-04-10 12:57:13.893781 precession-2.0.0.dev0/precession/
--rw-r--r--   0 dgerosa    (501) staff       (20)       54 2023-04-08 16:09:00.000000 precession-2.0.0.dev0/precession/__init__.py
--rw-r--r--   0 dgerosa    (501) staff       (20)      463 2023-04-10 12:56:42.000000 precession-2.0.0.dev0/precession/__version__.py
--rw-r--r--   0 dgerosa    (501) staff       (20)   226011 2023-04-08 16:08:25.000000 precession-2.0.0.dev0/precession/precession.py
-drwxr-xr-x   0 dgerosa    (501) staff       (20)        0 2023-04-10 12:57:13.896097 precession-2.0.0.dev0/precession.egg-info/
--rw-r--r--   0 dgerosa    (501) staff       (20)      469 2023-04-10 12:57:13.000000 precession-2.0.0.dev0/precession.egg-info/PKG-INFO
--rw-r--r--   0 dgerosa    (501) staff       (20)      331 2023-04-10 12:57:13.000000 precession-2.0.0.dev0/precession.egg-info/SOURCES.txt
--rw-r--r--   0 dgerosa    (501) staff       (20)        1 2023-04-10 12:57:13.000000 precession-2.0.0.dev0/precession.egg-info/dependency_links.txt
--rw-r--r--   0 dgerosa    (501) staff       (20)        1 2023-04-08 16:11:27.000000 precession-2.0.0.dev0/precession.egg-info/not-zip-safe
--rw-r--r--   0 dgerosa    (501) staff       (20)       19 2023-04-10 12:57:13.000000 precession-2.0.0.dev0/precession.egg-info/requires.txt
--rw-r--r--   0 dgerosa    (501) staff       (20)       11 2023-04-10 12:57:13.000000 precession-2.0.0.dev0/precession.egg-info/top_level.txt
--rw-r--r--   0 dgerosa    (501) staff       (20)       18 2023-04-10 07:39:31.000000 precession-2.0.0.dev0/requirements.txt
--rw-r--r--   0 dgerosa    (501) staff       (20)       38 2023-04-10 12:57:13.897439 precession-2.0.0.dev0/setup.cfg
--rw-r--r--   0 dgerosa    (501) staff       (20)      961 2023-04-10 07:58:24.000000 precession-2.0.0.dev0/setup.py
+drwxr-xr-x   0 dgerosa    (501) staff       (20)        0 2023-04-23 18:52:59.606385 precession-2.0.1/
+-rw-r--r--   0 dgerosa    (501) staff       (20)     1071 2022-02-03 16:32:40.000000 precession-2.0.1/LICENSE
+-rw-r--r--   0 dgerosa    (501) staff       (20)       24 2023-04-08 16:44:47.000000 precession-2.0.1/MANIFEST.in
+-rw-r--r--   0 dgerosa    (501) staff       (20)      464 2023-04-23 18:52:59.605887 precession-2.0.1/PKG-INFO
+-rw-r--r--   0 dgerosa    (501) staff       (20)     2755 2023-04-10 07:58:58.000000 precession-2.0.1/README.md
+drwxr-xr-x   0 dgerosa    (501) staff       (20)        0 2023-04-23 18:52:59.600202 precession-2.0.1/precession/
+-rw-r--r--   0 dgerosa    (501) staff       (20)       54 2023-04-08 16:09:00.000000 precession-2.0.1/precession/__init__.py
+-rw-r--r--   0 dgerosa    (501) staff       (20)      458 2023-04-23 18:52:19.000000 precession-2.0.1/precession/__version__.py
+-rw-r--r--   0 dgerosa    (501) staff       (20)   226012 2023-04-23 18:52:21.000000 precession-2.0.1/precession/precession.py
+drwxr-xr-x   0 dgerosa    (501) staff       (20)        0 2023-04-23 18:52:59.604443 precession-2.0.1/precession.egg-info/
+-rw-r--r--   0 dgerosa    (501) staff       (20)      464 2023-04-23 18:52:59.000000 precession-2.0.1/precession.egg-info/PKG-INFO
+-rw-r--r--   0 dgerosa    (501) staff       (20)      331 2023-04-23 18:52:59.000000 precession-2.0.1/precession.egg-info/SOURCES.txt
+-rw-r--r--   0 dgerosa    (501) staff       (20)        1 2023-04-23 18:52:59.000000 precession-2.0.1/precession.egg-info/dependency_links.txt
+-rw-r--r--   0 dgerosa    (501) staff       (20)        1 2023-04-08 16:11:27.000000 precession-2.0.1/precession.egg-info/not-zip-safe
+-rw-r--r--   0 dgerosa    (501) staff       (20)       19 2023-04-23 18:52:59.000000 precession-2.0.1/precession.egg-info/requires.txt
+-rw-r--r--   0 dgerosa    (501) staff       (20)       11 2023-04-23 18:52:59.000000 precession-2.0.1/precession.egg-info/top_level.txt
+-rw-r--r--   0 dgerosa    (501) staff       (20)       18 2023-04-10 07:39:31.000000 precession-2.0.1/requirements.txt
+-rw-r--r--   0 dgerosa    (501) staff       (20)       38 2023-04-23 18:52:59.606560 precession-2.0.1/setup.cfg
+-rw-r--r--   0 dgerosa    (501) staff       (20)      984 2023-04-10 13:12:57.000000 precession-2.0.1/setup.py
```

### Comparing `precession-2.0.0.dev0/LICENSE` & `precession-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `precession-2.0.0.dev0/README.md` & `precession-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `precession-2.0.0.dev0/precession/precession.py` & `precession-2.0.1/precession/precession.py`

 * *Files 0% similar despite different names*

```diff
@@ -1138,15 +1138,15 @@
     
     Examples
     --------
     ``theta12 = precession.eval_theta12(theta1=theta1,theta2=theta2,deltaphi=deltaphi)``
     ``theta12 = precession.eval_theta12(deltachi=deltachi,kappa=kappa,chieff=chieff,q=q,chi1=chi1,chi2=chi2)``
     """
 
-    costheta12 = eval_costheta1(theta1=theta1, theta2=theta2, deltaphi=deltaphi, deltachi=deltachi, kappa=kappa, chieff=chieff, q=q, chi1=chi1, chi2=chi2)
+    costheta12 = eval_costheta12(theta1=theta1, theta2=theta2, deltaphi=deltaphi, deltachi=deltachi, kappa=kappa, chieff=chieff, q=q, chi1=chi1, chi2=chi2)
     theta12 = np.arccos(costheta12)
 
     return theta12
 
 
 def eval_cosdeltaphi(deltachi, kappa, r, chieff, q, chi1, chi2):
     """
```

### Comparing `precession-2.0.0.dev0/setup.py` & `precession-2.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-#python setup.py sdist
-#twine upload --repository pypitest dist/*
-
+# python setup.py sdist
+# twine upload --repository pypitest dist/*
+# twine upload dist/*
 
 import os
 import setuptools
 
 about = {}
 here = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(here, 'precession', '__version__.py'), 'r') as _:
```

