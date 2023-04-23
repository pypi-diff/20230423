# Comparing `tmp/pursuitlib-0.2.1.tar.gz` & `tmp/pursuitlib-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pursuitlib-0.2.1.tar", last modified: Sun Mar 13 18:35:55 2022, max compression
+gzip compressed data, was "pursuitlib-0.3.0.tar", last modified: Sun Apr 23 21:39:55 2023, max compression
```

## Comparing `pursuitlib-0.2.1.tar` & `pursuitlib-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-03-13 18:35:55.144832 pursuitlib-0.2.1/
--rw-rw-rw-   0        0        0      533 2022-03-13 18:35:55.143844 pursuitlib-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      110 2022-03-13 18:10:36.000000 pursuitlib-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2022-03-13 18:35:55.116831 pursuitlib-0.2.1/pursuitlib/
--rw-rw-rw-   0        0        0        0 2022-03-13 18:10:36.000000 pursuitlib-0.2.1/pursuitlib/__init__.py
--rw-rw-rw-   0        0        0      651 2022-03-13 18:10:36.000000 pursuitlib-0.2.1/pursuitlib/color.py
--rw-rw-rw-   0        0        0      493 2022-03-13 18:10:36.000000 pursuitlib-0.2.1/pursuitlib/parsing.py
--rw-rw-rw-   0        0        0      781 2022-03-13 18:30:12.000000 pursuitlib-0.2.1/pursuitlib/utils.py
-drwxrwxrwx   0        0        0        0 2022-03-13 18:35:55.141838 pursuitlib-0.2.1/pursuitlib.egg-info/
--rw-rw-rw-   0        0        0      533 2022-03-13 18:35:54.000000 pursuitlib-0.2.1/pursuitlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2022-03-13 18:35:55.000000 pursuitlib-0.2.1/pursuitlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-13 18:35:54.000000 pursuitlib-0.2.1/pursuitlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2022-03-13 18:35:55.000000 pursuitlib-0.2.1/pursuitlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      177 2022-03-13 18:10:36.000000 pursuitlib-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-03-13 18:35:55.145846 pursuitlib-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      691 2022-03-13 18:30:26.000000 pursuitlib-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 21:39:55.748036 pursuitlib-0.3.0/
+-rw-rw-rw-   0        0        0      510 2023-04-23 21:39:55.747036 pursuitlib-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      110 2022-12-04 22:52:50.000000 pursuitlib-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 21:39:55.725034 pursuitlib-0.3.0/pursuitlib/
+-rw-rw-rw-   0        0        0        0 2022-12-04 22:52:50.000000 pursuitlib-0.3.0/pursuitlib/__init__.py
+-rw-rw-rw-   0        0        0      651 2022-12-04 22:52:50.000000 pursuitlib-0.3.0/pursuitlib/color.py
+-rw-rw-rw-   0        0        0     1043 2023-04-23 18:50:32.000000 pursuitlib-0.3.0/pursuitlib/decorators.py
+-rw-rw-rw-   0        0        0      314 2023-04-15 22:57:18.000000 pursuitlib-0.3.0/pursuitlib/indexedenum.py
+-rw-rw-rw-   0        0        0     1411 2023-04-14 17:01:53.000000 pursuitlib-0.3.0/pursuitlib/iterators.py
+-rw-rw-rw-   0        0        0      962 2023-04-10 18:15:09.000000 pursuitlib-0.3.0/pursuitlib/parsing.py
+-rw-rw-rw-   0        0        0      781 2023-04-10 18:11:46.000000 pursuitlib-0.3.0/pursuitlib/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-23 21:39:55.744036 pursuitlib-0.3.0/pursuitlib.egg-info/
+-rw-rw-rw-   0        0        0      510 2023-04-23 21:39:55.000000 pursuitlib-0.3.0/pursuitlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-04-23 21:39:55.000000 pursuitlib-0.3.0/pursuitlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 21:39:55.000000 pursuitlib-0.3.0/pursuitlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-23 21:39:55.000000 pursuitlib-0.3.0/pursuitlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      177 2022-12-04 22:52:50.000000 pursuitlib-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-23 21:39:55.749035 pursuitlib-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      691 2023-04-23 21:16:54.000000 pursuitlib-0.3.0/setup.py
```

### Comparing `pursuitlib-0.2.1/pursuitlib/color.py` & `pursuitlib-0.3.0/pursuitlib/color.py`

 * *Files identical despite different names*

### Comparing `pursuitlib-0.2.1/pursuitlib/utils.py` & `pursuitlib-0.3.0/pursuitlib/utils.py`

 * *Files identical despite different names*

### Comparing `pursuitlib-0.2.1/setup.py` & `pursuitlib-0.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup
 from pathlib import Path
 
 directory = Path(__file__).parent
 
 setup(
-    name='pursuitlib',
-    version='0.2.1',
-    packages=['pursuitlib'],
+    name="pursuitlib",
+    version="0.3.0",
+    packages=["pursuitlib"],
     entry_points={},
-    author='Pursuit',
-    author_email='fr.pursuit@gmail.com',
-    description='Provides utility functions',
+    author="Pursuit",
+    author_email="fr.pursuit@gmail.com",
+    description="Provides utility functions",
     long_description=(directory / "README.md").read_text(encoding="utf-8"),
-    long_description_content_type='text/markdown',
-    url='https://gitlab.com/frPursuit/pursuitlib-python',
-    license='All rights reserved',
+    long_description_content_type="text/markdown",
+    url="https://gitlab.com/frPursuit/pursuitlib-python",
+    license="All rights reserved",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.7"
+    python_requires=">=3.8"
 )
```

