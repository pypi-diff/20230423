# Comparing `tmp/featurizerai-1.4.0.tar.gz` & `tmp/featurizerai-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurizerai-1.4.0.tar", last modified: Sat Apr 22 17:01:16 2023, max compression
+gzip compressed data, was "featurizerai-1.4.3.tar", last modified: Sat Apr 22 22:42:41 2023, max compression
```

## Comparing `featurizerai-1.4.0.tar` & `featurizerai-1.4.3.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:01:16.333853 featurizerai-1.4.0/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.4.0/LICENSE
--rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.4.0/MANIFEST.in
--rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-22 17:01:16.333922 featurizerai-1.4.0/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.4.0/pyproject.toml
--rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-22 17:01:16.334134 featurizerai-1.4.0/setup.cfg
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1385 2023-04-22 16:59:53.000000 featurizerai-1.4.0/setup.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:01:16.331590 featurizerai-1.4.0/src/
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:01:16.332639 featurizerai-1.4.0/src/featurizerai/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-08 16:21:11.000000 featurizerai-1.4.0/src/featurizerai/__init__.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:01:16.333579 featurizerai-1.4.0/src/featurizerai/features/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     5672 2023-04-22 17:01:08.000000 featurizerai-1.4.0/src/featurizerai/features/FeatureStore.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-03-30 14:52:30.000000 featurizerai-1.4.0/src/featurizerai/features/__init__.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:01:16.333263 featurizerai-1.4.0/src/featurizerai.egg-info/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      856 2023-04-22 17:01:16.000000 featurizerai-1.4.0/src/featurizerai.egg-info/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)      425 2023-04-22 17:01:16.000000 featurizerai-1.4.0/src/featurizerai.egg-info/SOURCES.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-22 17:01:16.000000 featurizerai-1.4.0/src/featurizerai.egg-info/dependency_links.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-22 17:01:16.000000 featurizerai-1.4.0/src/featurizerai.egg-info/requires.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       13 2023-04-22 17:01:16.000000 featurizerai-1.4.0/src/featurizerai.egg-info/top_level.txt
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:01:16.333741 featurizerai-1.4.0/tests/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      810 2023-04-22 16:32:43.000000 featurizerai-1.4.0/tests/test_module1.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 22:42:41.518757 featurizerai-1.4.3/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.4.3/LICENSE
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.4.3/MANIFEST.in
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-22 22:42:41.518821 featurizerai-1.4.3/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.4.3/pyproject.toml
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-22 22:42:41.519193 featurizerai-1.4.3/setup.cfg
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1378 2023-04-22 22:41:27.000000 featurizerai-1.4.3/setup.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 22:42:41.516549 featurizerai-1.4.3/src/
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 22:42:41.518009 featurizerai-1.4.3/src/features/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:23:59.000000 featurizerai-1.4.3/src/features/__init__.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     3010 2023-04-22 21:36:06.000000 featurizerai-1.4.3/src/features/create_stream.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     4533 2023-04-22 22:30:15.000000 featurizerai-1.4.3/src/features/materialize.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      941 2023-04-22 21:36:37.000000 featurizerai-1.4.3/src/features/test_create_stream.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      822 2023-04-22 22:30:00.000000 featurizerai-1.4.3/src/features/test_materialize.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-22 22:42:41.518650 featurizerai-1.4.3/src/featurizerai.egg-info/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-22 22:42:41.000000 featurizerai-1.4.3/src/featurizerai.egg-info/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      403 2023-04-22 22:42:41.000000 featurizerai-1.4.3/src/featurizerai.egg-info/SOURCES.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-22 22:42:41.000000 featurizerai-1.4.3/src/featurizerai.egg-info/dependency_links.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-22 22:42:41.000000 featurizerai-1.4.3/src/featurizerai.egg-info/requires.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        9 2023-04-22 22:42:41.000000 featurizerai-1.4.3/src/featurizerai.egg-info/top_level.txt
```

### Comparing `featurizerai-1.4.0/LICENSE` & `featurizerai-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `featurizerai-1.4.0/PKG-INFO` & `featurizerai-1.4.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.4.0
+Version: 1.4.3
 Summary: Python library for Featurizer AI
-Home-page: https://github.com/burakgloba/featurizerai
+Home-page: https://github.com/burakglobal/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
```

### Comparing `featurizerai-1.4.0/setup.py` & `featurizerai-1.4.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 
 setuptools.setup(
     name='featurizerai',
     author='Burak',
-    version='1.4.0',
+    version='1.4.3',
     author_email='burakgblobal@gmail.com',
     description='Python library for Featurizer AI',
     keywords='featurizer, package',
-    url='https://github.com/burakgloba/featurizerai',
+    url='https://github.com/burakglobal/featurizerai',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     classifiers=[
         # see https://pypi.org/classifiers/
         'Development Status :: 5 - Production/Stable',
 
         'Intended Audience :: Developers',
@@ -30,12 +30,12 @@
     # install_requires=['Pillow'],
     extras_require={
         'dev': ['check-manifest'],
         # 'test': ['coverage'],
     },
     # entry_points={
     #     'console_scripts': [  # This can provide executable scripts
-    #         'run=featurizerai:main',
-    # You can execute `run` in bash to run `main()` in src/featurizerai/__init__.py
+    #         'run=features:main',
+    # You can execute `run` in bash to run `main()` in src/features/__init__.py
     #     ],
     # },
 )
```

### Comparing `featurizerai-1.4.0/src/featurizerai.egg-info/PKG-INFO` & `featurizerai-1.4.3/src/featurizerai.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.4.0
+Version: 1.4.3
 Summary: Python library for Featurizer AI
-Home-page: https://github.com/burakgloba/featurizerai
+Home-page: https://github.com/burakglobal/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
```

