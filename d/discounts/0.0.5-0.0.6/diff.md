# Comparing `tmp/discounts-0.0.5.tar.gz` & `tmp/discounts-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discounts-0.0.5.tar", last modified: Sun Apr 23 18:34:32 2023, max compression
+gzip compressed data, was "discounts-0.0.6.tar", last modified: Sun Apr 23 18:43:08 2023, max compression
```

## Comparing `discounts-0.0.5.tar` & `discounts-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 18:34:32.165326 discounts-0.0.5/
--rw-rw-rw-   0        0        0       82 2023-04-23 16:34:24.000000 discounts-0.0.5/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1071 2023-04-23 16:36:46.000000 discounts-0.0.5/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2023-04-23 16:35:04.000000 discounts-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      685 2023-04-23 18:34:32.164334 discounts-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       79 2023-04-23 16:32:47.000000 discounts-0.0.5/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-23 18:34:32.161337 discounts-0.0.5/discounts.egg-info/
--rw-rw-rw-   0        0        0      685 2023-04-23 18:34:31.000000 discounts-0.0.5/discounts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-04-23 18:34:32.000000 discounts-0.0.5/discounts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 18:34:31.000000 discounts-0.0.5/discounts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-23 18:34:32.000000 discounts-0.0.5/discounts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-23 18:34:32.162342 discounts-0.0.5/foodbook_discount/
--rw-rw-rw-   0        0        0      359 2023-04-23 18:14:59.000000 discounts-0.0.5/foodbook_discount/__init__.py
--rw-rw-rw-   0        0        0       42 2023-04-23 18:34:32.165326 discounts-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      743 2023-04-23 18:34:04.000000 discounts-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 18:43:08.875116 discounts-0.0.6/
+-rw-rw-rw-   0        0        0       82 2023-04-23 16:34:24.000000 discounts-0.0.6/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1071 2023-04-23 16:36:46.000000 discounts-0.0.6/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-23 16:35:04.000000 discounts-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      685 2023-04-23 18:43:08.874122 discounts-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       79 2023-04-23 16:32:47.000000 discounts-0.0.6/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 18:43:08.852242 discounts-0.0.6/discounts/
+-rw-rw-rw-   0        0        0      339 2023-04-23 18:41:56.000000 discounts-0.0.6/discounts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 18:43:08.873118 discounts-0.0.6/discounts.egg-info/
+-rw-rw-rw-   0        0        0      685 2023-04-23 18:43:08.000000 discounts-0.0.6/discounts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-04-23 18:43:08.000000 discounts-0.0.6/discounts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 18:43:08.000000 discounts-0.0.6/discounts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-23 18:43:08.000000 discounts-0.0.6/discounts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 18:43:08.875116 discounts-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      743 2023-04-23 18:39:34.000000 discounts-0.0.6/setup.py
```

### Comparing `discounts-0.0.5/LICENCE.txt` & `discounts-0.0.6/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `discounts-0.0.5/PKG-INFO` & `discounts-0.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discounts
-Version: 0.0.5
+Version: 0.0.6
 Summary: Package created for using discount function
 Home-page: 
 Author: Akash Sane
 Author-email: x21220956@student.ncirl.ie
 License: MIT
 Keywords: discount
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discounts-0.0.5/discounts.egg-info/PKG-INFO` & `discounts-0.0.6/discounts.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discounts
-Version: 0.0.5
+Version: 0.0.6
 Summary: Package created for using discount function
 Home-page: 
 Author: Akash Sane
 Author-email: x21220956@student.ncirl.ie
 License: MIT
 Keywords: discount
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discounts-0.0.5/setup.py` & `discounts-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3' 
 ]
 
 setup(
 
     name='discounts',
-    version='0.0.5',
+    version='0.0.6',
     description='Package created for using discount function',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='Akash Sane',
     author_email='x21220956@student.ncirl.ie',
     license='MIT',
     classifiers=classifiers,
```

