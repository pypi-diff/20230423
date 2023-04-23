# Comparing `tmp/sentiment_stock_plot-0.0.1.tar.gz` & `tmp/sentiment_stock_plot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentiment_stock_plot-0.0.1.tar", last modified: Sun Apr 23 06:20:24 2023, max compression
+gzip compressed data, was "sentiment_stock_plot-0.0.2.tar", last modified: Sun Apr 23 07:53:10 2023, max compression
```

## Comparing `sentiment_stock_plot-0.0.1.tar` & `sentiment_stock_plot-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 lukeabbatessa   (501) staff       (20)        0 2023-04-23 06:20:24.632327 sentiment_stock_plot-0.0.1/
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)       77 2023-04-23 06:09:45.000000 sentiment_stock_plot-0.0.1/CHANGELOG.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)     1061 2023-04-23 04:31:59.000000 sentiment_stock_plot-0.0.1/LICENCE.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)       25 2023-04-23 04:31:56.000000 sentiment_stock_plot-0.0.1/MANIFEST.in
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)      723 2023-04-23 06:20:24.631984 sentiment_stock_plot-0.0.1/PKG-INFO
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)      124 2023-04-23 06:09:37.000000 sentiment_stock_plot-0.0.1/README.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)     7064 2023-04-23 04:31:47.000000 sentiment_stock_plot-0.0.1/__init__.py
-drwxr-xr-x   0 lukeabbatessa   (501) staff       (20)        0 2023-04-23 06:20:24.631453 sentiment_stock_plot-0.0.1/sentiment_stock_plot.egg-info/
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)      723 2023-04-23 06:20:24.000000 sentiment_stock_plot-0.0.1/sentiment_stock_plot.egg-info/PKG-INFO
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)      288 2023-04-23 06:20:24.000000 sentiment_stock_plot-0.0.1/sentiment_stock_plot.egg-info/SOURCES.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)        1 2023-04-23 06:20:24.000000 sentiment_stock_plot-0.0.1/sentiment_stock_plot.egg-info/dependency_links.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)       51 2023-04-23 06:20:24.000000 sentiment_stock_plot-0.0.1/sentiment_stock_plot.egg-info/requires.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)        1 2023-04-23 06:20:24.000000 sentiment_stock_plot-0.0.1/sentiment_stock_plot.egg-info/top_level.txt
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)       38 2023-04-23 06:20:24.632526 sentiment_stock_plot-0.0.1/setup.cfg
--rw-r--r--   0 lukeabbatessa   (501) staff       (20)      841 2023-04-23 06:16:07.000000 sentiment_stock_plot-0.0.1/setup.py
+drwxr-xr-x   0 lukeabbatessa   (501) staff       (20)        0 2023-04-23 07:53:10.467899 sentiment_stock_plot-0.0.2/
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)       78 2023-04-23 07:27:06.000000 sentiment_stock_plot-0.0.2/CHANGELOG.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)     1061 2023-04-23 04:31:59.000000 sentiment_stock_plot-0.0.2/LICENCE.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)       25 2023-04-23 04:31:56.000000 sentiment_stock_plot-0.0.2/MANIFEST.in
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)      724 2023-04-23 07:53:10.467444 sentiment_stock_plot-0.0.2/PKG-INFO
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)      124 2023-04-23 06:09:37.000000 sentiment_stock_plot-0.0.2/README.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)     7064 2023-04-23 04:31:47.000000 sentiment_stock_plot-0.0.2/__init__.py
+drwxr-xr-x   0 lukeabbatessa   (501) staff       (20)        0 2023-04-23 07:53:10.466725 sentiment_stock_plot-0.0.2/sentiment_stock_plot.egg-info/
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)      724 2023-04-23 07:53:10.000000 sentiment_stock_plot-0.0.2/sentiment_stock_plot.egg-info/PKG-INFO
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)      288 2023-04-23 07:53:10.000000 sentiment_stock_plot-0.0.2/sentiment_stock_plot.egg-info/SOURCES.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)        1 2023-04-23 07:53:10.000000 sentiment_stock_plot-0.0.2/sentiment_stock_plot.egg-info/dependency_links.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)       51 2023-04-23 07:53:10.000000 sentiment_stock_plot-0.0.2/sentiment_stock_plot.egg-info/requires.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)        1 2023-04-23 07:53:10.000000 sentiment_stock_plot-0.0.2/sentiment_stock_plot.egg-info/top_level.txt
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)       38 2023-04-23 07:53:10.468106 sentiment_stock_plot-0.0.2/setup.cfg
+-rw-r--r--   0 lukeabbatessa   (501) staff       (20)      841 2023-04-23 07:51:48.000000 sentiment_stock_plot-0.0.2/setup.py
```

### Comparing `sentiment_stock_plot-0.0.1/LICENCE.txt` & `sentiment_stock_plot-0.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `sentiment_stock_plot-0.0.1/PKG-INFO` & `sentiment_stock_plot-0.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentiment_stock_plot
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is a library that provides a foundation for a sentiment stock plot
 Home-page: 
 Author: Luke Abbatessa
 Author-email: labbatessa14@gmail.com
 License: MIT
 Keywords: sentiment stock
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,10 +15,10 @@
 License-File: LICENCE.txt
 
 This is a library that provides a foundation for creating an average sentiment score vs. stock price percentage change plot.
 
 Change Log
 ==========
 
-0.0.1 (04/23/2023)
+0.0.2 (04/23/2023)
 -------------------
-- First Release
+- Second Release
```

### Comparing `sentiment_stock_plot-0.0.1/__init__.py` & `sentiment_stock_plot-0.0.2/__init__.py`

 * *Files identical despite different names*

### Comparing `sentiment_stock_plot-0.0.1/sentiment_stock_plot.egg-info/PKG-INFO` & `sentiment_stock_plot-0.0.2/sentiment_stock_plot.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentiment-stock-plot
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is a library that provides a foundation for a sentiment stock plot
 Home-page: 
 Author: Luke Abbatessa
 Author-email: labbatessa14@gmail.com
 License: MIT
 Keywords: sentiment stock
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,10 +15,10 @@
 License-File: LICENCE.txt
 
 This is a library that provides a foundation for creating an average sentiment score vs. stock price percentage change plot.
 
 Change Log
 ==========
 
-0.0.1 (04/23/2023)
+0.0.2 (04/23/2023)
 -------------------
-- First Release
+- Second Release
```

### Comparing `sentiment_stock_plot-0.0.1/setup.py` & `sentiment_stock_plot-0.0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,22 +6,22 @@
     'Operating System :: MacOS',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='sentiment_stock_plot',
-    version='0.0.1',
+    version='0.0.2',
     description='This is a library that provides a foundation for a sentiment stock plot',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='Luke Abbatessa',
     author_email='labbatessa14@gmail.com',
     license='MIT',
     classifiers=classifiers,
     keywords='sentiment stock',
     packages=find_packages(),
-    install_requires=['pandas>=1.4.3',
+    install_requires=['pandas>=1.3.5',
                       'plotly>=5.10.0',
-                      'dash-data-prep>=0.0.1'
+                      'dash-data-prep>=0.0.2'
     ],
 )
```

