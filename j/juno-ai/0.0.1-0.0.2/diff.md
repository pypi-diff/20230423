# Comparing `tmp/juno-ai-0.0.1.tar.gz` & `tmp/juno-ai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/juno-ai-0.0.1.tar", last modified: Sun Apr 23 01:46:10 2023, max compression
+gzip compressed data, was "dist/juno-ai-0.0.2.tar", last modified: Sun Apr 23 01:53:04 2023, max compression
```

## Comparing `juno-ai-0.0.1.tar` & `juno-ai-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-04-23 01:46:10.000000 juno-ai-0.0.1/
--rw-r--r--   0 alexirobbins   (501) staff       (20)      923 2023-04-23 01:46:10.000000 juno-ai-0.0.1/PKG-INFO
-drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-04-23 01:46:10.000000 juno-ai-0.0.1/juno_ai.egg-info/
--rw-r--r--   0 alexirobbins   (501) staff       (20)      923 2023-04-23 01:46:10.000000 juno-ai-0.0.1/juno_ai.egg-info/PKG-INFO
--rw-r--r--   0 alexirobbins   (501) staff       (20)      345 2023-04-23 01:46:10.000000 juno-ai-0.0.1/juno_ai.egg-info/SOURCES.txt
--rw-r--r--   0 alexirobbins   (501) staff       (20)       34 2023-04-23 01:46:10.000000 juno-ai-0.0.1/juno_ai.egg-info/requires.txt
--rw-r--r--   0 alexirobbins   (501) staff       (20)        5 2023-04-23 01:46:10.000000 juno-ai-0.0.1/juno_ai.egg-info/top_level.txt
--rw-r--r--   0 alexirobbins   (501) staff       (20)        1 2023-04-23 01:46:10.000000 juno-ai-0.0.1/juno_ai.egg-info/dependency_links.txt
--rw-r--r--   0 alexirobbins   (501) staff       (20)     1156 2023-04-23 01:46:00.000000 juno-ai-0.0.1/setup.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)       38 2023-04-23 01:46:10.000000 juno-ai-0.0.1/setup.cfg
-drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-04-23 01:46:10.000000 juno-ai-0.0.1/juno/
--rw-r--r--   0 alexirobbins   (501) staff       (20)     1359 2023-04-23 00:04:48.000000 juno-ai-0.0.1/juno/magic.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)     2381 2023-04-16 21:49:54.000000 juno-ai-0.0.1/juno/serialize_context.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)     1253 2023-04-16 22:35:57.000000 juno-ai-0.0.1/juno/client_setup.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)      473 2023-04-15 21:33:31.000000 juno-ai-0.0.1/juno/version.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)       58 2023-04-09 05:43:26.000000 juno-ai-0.0.1/juno/__init__.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)      873 2023-03-31 21:04:15.000000 juno-ai-0.0.1/juno/output_parser.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)    16128 2023-04-23 01:07:57.000000 juno-ai-0.0.1/juno/event_javascript.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)     1229 2023-04-22 23:55:05.000000 juno-ai-0.0.1/juno/juno.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)     8507 2023-04-23 00:13:02.000000 juno-ai-0.0.1/juno/prompting_javascript.py
+drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-04-23 01:53:04.000000 juno-ai-0.0.2/
+-rw-r--r--   0 alexirobbins   (501) staff       (20)      712 2023-04-23 01:53:04.000000 juno-ai-0.0.2/PKG-INFO
+drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-04-23 01:53:04.000000 juno-ai-0.0.2/juno_ai.egg-info/
+-rw-r--r--   0 alexirobbins   (501) staff       (20)      712 2023-04-23 01:53:03.000000 juno-ai-0.0.2/juno_ai.egg-info/PKG-INFO
+-rw-r--r--   0 alexirobbins   (501) staff       (20)      345 2023-04-23 01:53:03.000000 juno-ai-0.0.2/juno_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 alexirobbins   (501) staff       (20)       34 2023-04-23 01:53:03.000000 juno-ai-0.0.2/juno_ai.egg-info/requires.txt
+-rw-r--r--   0 alexirobbins   (501) staff       (20)        5 2023-04-23 01:53:03.000000 juno-ai-0.0.2/juno_ai.egg-info/top_level.txt
+-rw-r--r--   0 alexirobbins   (501) staff       (20)        1 2023-04-23 01:53:03.000000 juno-ai-0.0.2/juno_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     1219 2023-04-23 01:52:53.000000 juno-ai-0.0.2/setup.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)       38 2023-04-23 01:53:04.000000 juno-ai-0.0.2/setup.cfg
+drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-04-23 01:53:04.000000 juno-ai-0.0.2/juno/
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     1359 2023-04-23 00:04:48.000000 juno-ai-0.0.2/juno/magic.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     2381 2023-04-16 21:49:54.000000 juno-ai-0.0.2/juno/serialize_context.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     1253 2023-04-16 22:35:57.000000 juno-ai-0.0.2/juno/client_setup.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)      473 2023-04-23 01:52:59.000000 juno-ai-0.0.2/juno/version.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)       58 2023-04-09 05:43:26.000000 juno-ai-0.0.2/juno/__init__.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)      873 2023-03-31 21:04:15.000000 juno-ai-0.0.2/juno/output_parser.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)    16128 2023-04-23 01:07:57.000000 juno-ai-0.0.2/juno/event_javascript.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     1229 2023-04-22 23:55:05.000000 juno-ai-0.0.2/juno/juno.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     8507 2023-04-23 00:13:02.000000 juno-ai-0.0.2/juno/prompting_javascript.py
```

### Comparing `juno-ai-0.0.1/PKG-INFO` & `juno-ai-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,16 @@
 Metadata-Version: 1.1
 Name: juno-ai
-Version: 0.0.1
+Version: 0.0.2
 Summary: UNKNOWN
-Home-page: UNKNOWN
+Home-page: https://github.com/alexi/juno
 Author: juno
 Author-email: hellojunoai@gmail.com
 License: UNKNOWN
-Description: # juno
-        
-        ## Get Started
-        
-        ```bash
-        pip install -e .
-        ```
-        
-        In jupyter:
-        
-        ```python
-        %load_ext juno
-        ```
-        
-        new cell:
-        ```python
-        %chat [prompt]
-        ```
+Description: Juno AI Assistant for Jupyter Notebook
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: IPython
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Programming Language :: Python :: 3
```

### Comparing `juno-ai-0.0.1/juno_ai.egg-info/PKG-INFO` & `juno-ai-0.0.2/juno_ai.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,16 @@
 Metadata-Version: 1.1
 Name: juno-ai
-Version: 0.0.1
+Version: 0.0.2
 Summary: UNKNOWN
-Home-page: UNKNOWN
+Home-page: https://github.com/alexi/juno
 Author: juno
 Author-email: hellojunoai@gmail.com
 License: UNKNOWN
-Description: # juno
-        
-        ## Get Started
-        
-        ```bash
-        pip install -e .
-        ```
-        
-        In jupyter:
-        
-        ```python
-        %load_ext juno
-        ```
-        
-        new cell:
-        ```python
-        %chat [prompt]
-        ```
+Description: Juno AI Assistant for Jupyter Notebook
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: IPython
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Programming Language :: Python :: 3
```

### Comparing `juno-ai-0.0.1/setup.py` & `juno-ai-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 # exec(open(read('juno/version.py')).read())
 print('packages:', [package for package in find_packages()
                 if package.startswith('juno')])
 setup(
     name='juno-ai', 
     # version=__version__, 
-    version='0.0.1',
+    version='0.0.2',
     packages=[package for package in find_packages()
                 if package.startswith('juno')], 
-    long_description=read('README.md'),
+    long_description='Juno AI Assistant for Jupyter Notebook',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Framework :: IPython',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'Topic :: Multimedia :: Graphics',
         'Programming Language :: Python :: 3',
@@ -29,8 +29,9 @@
     install_requires=[
         'IPython',
         'traitlets',
         'notebook>=5.7.6',
     ],
     author='juno',
     author_email='hellojunoai@gmail.com',
+    url="https://github.com/alexi/juno"
 )
```

### Comparing `juno-ai-0.0.1/juno/magic.py` & `juno-ai-0.0.2/juno/magic.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.1/juno/serialize_context.py` & `juno-ai-0.0.2/juno/serialize_context.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.1/juno/client_setup.py` & `juno-ai-0.0.2/juno/client_setup.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.1/juno/output_parser.py` & `juno-ai-0.0.2/juno/output_parser.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.1/juno/event_javascript.py` & `juno-ai-0.0.2/juno/event_javascript.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.1/juno/juno.py` & `juno-ai-0.0.2/juno/juno.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.1/juno/prompting_javascript.py` & `juno-ai-0.0.2/juno/prompting_javascript.py`

 * *Files identical despite different names*

