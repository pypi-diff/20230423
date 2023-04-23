# Comparing `tmp/discounts-0.0.6.tar.gz` & `tmp/discounts-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discounts-0.0.6.tar", last modified: Sun Apr 23 18:43:08 2023, max compression
+gzip compressed data, was "discounts-0.0.7.tar", last modified: Sun Apr 23 18:51:10 2023, max compression
```

## Comparing `discounts-0.0.6.tar` & `discounts-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 18:43:08.875116 discounts-0.0.6/
--rw-rw-rw-   0        0        0       82 2023-04-23 16:34:24.000000 discounts-0.0.6/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1071 2023-04-23 16:36:46.000000 discounts-0.0.6/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2023-04-23 16:35:04.000000 discounts-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      685 2023-04-23 18:43:08.874122 discounts-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       79 2023-04-23 16:32:47.000000 discounts-0.0.6/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-23 18:43:08.852242 discounts-0.0.6/discounts/
--rw-rw-rw-   0        0        0      339 2023-04-23 18:41:56.000000 discounts-0.0.6/discounts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 18:43:08.873118 discounts-0.0.6/discounts.egg-info/
--rw-rw-rw-   0        0        0      685 2023-04-23 18:43:08.000000 discounts-0.0.6/discounts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-04-23 18:43:08.000000 discounts-0.0.6/discounts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 18:43:08.000000 discounts-0.0.6/discounts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-23 18:43:08.000000 discounts-0.0.6/discounts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 18:43:08.875116 discounts-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      743 2023-04-23 18:39:34.000000 discounts-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 18:51:10.076436 discounts-0.0.7/
+-rw-rw-rw-   0        0        0       82 2023-04-23 16:34:24.000000 discounts-0.0.7/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1071 2023-04-23 16:36:46.000000 discounts-0.0.7/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-23 16:35:04.000000 discounts-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      685 2023-04-23 18:51:10.075436 discounts-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       79 2023-04-23 16:32:47.000000 discounts-0.0.7/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 18:51:10.061477 discounts-0.0.7/discounts/
+-rw-rw-rw-   0        0        0      338 2023-04-23 18:50:30.000000 discounts-0.0.7/discounts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 18:51:10.074439 discounts-0.0.7/discounts.egg-info/
+-rw-rw-rw-   0        0        0      685 2023-04-23 18:51:09.000000 discounts-0.0.7/discounts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-04-23 18:51:09.000000 discounts-0.0.7/discounts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 18:51:09.000000 discounts-0.0.7/discounts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-23 18:51:09.000000 discounts-0.0.7/discounts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 18:51:10.076436 discounts-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      743 2023-04-23 18:50:43.000000 discounts-0.0.7/setup.py
```

### Comparing `discounts-0.0.6/LICENCE.txt` & `discounts-0.0.7/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `discounts-0.0.6/PKG-INFO` & `discounts-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discounts
-Version: 0.0.6
+Version: 0.0.7
 Summary: Package created for using discount function
 Home-page: 
 Author: Akash Sane
 Author-email: x21220956@student.ncirl.ie
 License: MIT
 Keywords: discount
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discounts-0.0.6/discounts.egg-info/PKG-INFO` & `discounts-0.0.7/discounts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discounts
-Version: 0.0.6
+Version: 0.0.7
 Summary: Package created for using discount function
 Home-page: 
 Author: Akash Sane
 Author-email: x21220956@student.ncirl.ie
 License: MIT
 Keywords: discount
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discounts-0.0.6/setup.py` & `discounts-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3' 
 ]
 
 setup(
 
     name='discounts',
-    version='0.0.6',
+    version='0.0.7',
     description='Package created for using discount function',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='Akash Sane',
     author_email='x21220956@student.ncirl.ie',
     license='MIT',
     classifiers=classifiers,
```

