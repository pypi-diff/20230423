# Comparing `tmp/agnm-1.0.0.tar.gz` & `tmp/agnm-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agnm-1.0.0.tar", last modified: Sun Apr 23 18:52:26 2023, max compression
+gzip compressed data, was "agnm-1.0.1.tar", last modified: Sun Apr 23 18:54:23 2023, max compression
```

## Comparing `agnm-1.0.0.tar` & `agnm-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 18:52:26.064020 agnm-1.0.0/
--rw-rw-rw-   0        0        0     1080 2023-04-17 16:38:53.000000 agnm-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     2064 2023-04-23 18:52:26.060938 agnm-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1664 2023-04-23 18:50:26.000000 agnm-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 18:52:26.043937 agnm-1.0.0/agnm/
--rw-rw-rw-   0        0        0        0 2023-04-23 18:51:59.000000 agnm-1.0.0/agnm/__init__.py
--rw-rw-rw-   0        0        0     2603 2023-04-23 18:51:59.000000 agnm-1.0.0/agnm/motion.py
-drwxrwxrwx   0        0        0        0 2023-04-23 18:52:26.057946 agnm-1.0.0/agnm.egg-info/
--rw-rw-rw-   0        0        0     2064 2023-04-23 18:52:26.000000 agnm-1.0.0/agnm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-04-23 18:52:26.000000 agnm-1.0.0/agnm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 18:52:26.000000 agnm-1.0.0/agnm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-23 18:52:26.000000 agnm-1.0.0/agnm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      472 2023-04-23 18:51:03.000000 agnm-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-23 18:52:26.064020 agnm-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-23 18:54:23.083951 agnm-1.0.1/
+-rw-rw-rw-   0        0        0     1080 2023-04-17 16:38:53.000000 agnm-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     2062 2023-04-23 18:54:23.081920 agnm-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1662 2023-04-23 18:53:52.000000 agnm-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 18:54:23.067635 agnm-1.0.1/agnm/
+-rw-rw-rw-   0        0        0        0 2023-04-23 18:51:59.000000 agnm-1.0.1/agnm/__init__.py
+-rw-rw-rw-   0        0        0     2603 2023-04-23 18:51:59.000000 agnm-1.0.1/agnm/motion.py
+drwxrwxrwx   0        0        0        0 2023-04-23 18:54:23.079957 agnm-1.0.1/agnm.egg-info/
+-rw-rw-rw-   0        0        0     2062 2023-04-23 18:54:23.000000 agnm-1.0.1/agnm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2023-04-23 18:54:23.000000 agnm-1.0.1/agnm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 18:54:23.000000 agnm-1.0.1/agnm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-23 18:54:23.000000 agnm-1.0.1/agnm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      472 2023-04-23 18:53:52.000000 agnm-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-23 18:54:23.084922 agnm-1.0.1/setup.cfg
```

### Comparing `agnm-1.0.0/LICENSE.txt` & `agnm-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `agnm-1.0.0/PKG-INFO` & `agnm-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: agnm
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package for physics motion calculations
 Author-email: Agnė Moleikaitytė <agnmol@ktu.lt>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Physics equations of motion solver
 This is a package for physics motion calculations.
 
 # Installation
-```pip install agnmol```
+```pip install agnm```
 
 # Usage
 ### Displacement
 Displacement is calculated using formula: 
 ```math
 x = (vi-vf)/2*t 
 ```
```

### Comparing `agnm-1.0.0/README.md` & `agnm-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Physics equations of motion solver
 This is a package for physics motion calculations.
 
 # Installation
-```pip install agnmol```
+```pip install agnm```
 
 # Usage
 ### Displacement
 Displacement is calculated using formula: 
 ```math
 x = (vi-vf)/2*t 
 ```
```

### Comparing `agnm-1.0.0/agnm/motion.py` & `agnm-1.0.1/agnm/motion.py`

 * *Files identical despite different names*

### Comparing `agnm-1.0.0/agnm.egg-info/PKG-INFO` & `agnm-1.0.1/agnm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: agnm
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package for physics motion calculations
 Author-email: Agnė Moleikaitytė <agnmol@ktu.lt>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Physics equations of motion solver
 This is a package for physics motion calculations.
 
 # Installation
-```pip install agnmol```
+```pip install agnm```
 
 # Usage
 ### Displacement
 Displacement is calculated using formula: 
 ```math
 x = (vi-vf)/2*t 
 ```
```

