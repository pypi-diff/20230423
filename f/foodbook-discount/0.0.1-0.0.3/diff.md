# Comparing `tmp/foodbook_discount-0.0.1.tar.gz` & `tmp/foodbook_discount-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foodbook_discount-0.0.1.tar", last modified: Sun Apr 23 17:01:07 2023, max compression
+gzip compressed data, was "foodbook_discount-0.0.3.tar", last modified: Sun Apr 23 17:34:10 2023, max compression
```

## Comparing `foodbook_discount-0.0.1.tar` & `foodbook_discount-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 17:01:07.275257 foodbook_discount-0.0.1/
--rw-rw-rw-   0        0        0       82 2023-04-23 16:34:24.000000 foodbook_discount-0.0.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1071 2023-04-23 16:36:46.000000 foodbook_discount-0.0.1/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2023-04-23 16:35:04.000000 foodbook_discount-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      693 2023-04-23 17:01:07.274260 foodbook_discount-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       79 2023-04-23 16:32:47.000000 foodbook_discount-0.0.1/README.txt
--rw-rw-rw-   0        0        0      333 2023-04-23 16:31:32.000000 foodbook_discount-0.0.1/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 17:01:07.273262 foodbook_discount-0.0.1/foodbook_discount.egg-info/
--rw-rw-rw-   0        0        0      693 2023-04-23 17:01:07.000000 foodbook_discount-0.0.1/foodbook_discount.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-04-23 17:01:07.000000 foodbook_discount-0.0.1/foodbook_discount.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 17:01:07.000000 foodbook_discount-0.0.1/foodbook_discount.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 17:01:07.000000 foodbook_discount-0.0.1/foodbook_discount.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 17:01:07.275257 foodbook_discount-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      751 2023-04-23 16:59:09.000000 foodbook_discount-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 17:34:10.406321 foodbook_discount-0.0.3/
+-rw-rw-rw-   0        0        0       82 2023-04-23 16:34:24.000000 foodbook_discount-0.0.3/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1071 2023-04-23 16:36:46.000000 foodbook_discount-0.0.3/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-23 16:35:04.000000 foodbook_discount-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      693 2023-04-23 17:34:10.406321 foodbook_discount-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       79 2023-04-23 16:32:47.000000 foodbook_discount-0.0.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 17:34:10.401470 foodbook_discount-0.0.3/discount/
+-rw-rw-rw-   0        0        0      333 2023-04-23 16:31:32.000000 foodbook_discount-0.0.3/discount/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 17:34:10.405300 foodbook_discount-0.0.3/foodbook_discount.egg-info/
+-rw-rw-rw-   0        0        0      693 2023-04-23 17:34:10.000000 foodbook_discount-0.0.3/foodbook_discount.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-04-23 17:34:10.000000 foodbook_discount-0.0.3/foodbook_discount.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 17:34:10.000000 foodbook_discount-0.0.3/foodbook_discount.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 17:34:10.000000 foodbook_discount-0.0.3/foodbook_discount.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 17:34:10.406321 foodbook_discount-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      761 2023-04-23 17:33:54.000000 foodbook_discount-0.0.3/setup.py
```

### Comparing `foodbook_discount-0.0.1/LICENCE.txt` & `foodbook_discount-0.0.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `foodbook_discount-0.0.1/PKG-INFO` & `foodbook_discount-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foodbook_discount
-Version: 0.0.1
+Version: 0.0.3
 Summary: Package created for using discount function
 Home-page: 
 Author: Akash Sane
 Author-email: x21220956@student.ncirl.ie
 License: MIT
 Keywords: discount
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `foodbook_discount-0.0.1/foodbook_discount.egg-info/PKG-INFO` & `foodbook_discount-0.0.3/foodbook_discount.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foodbook-discount
-Version: 0.0.1
+Version: 0.0.3
 Summary: Package created for using discount function
 Home-page: 
 Author: Akash Sane
 Author-email: x21220956@student.ncirl.ie
 License: MIT
 Keywords: discount
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `foodbook_discount-0.0.1/setup.py` & `foodbook_discount-0.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,19 +7,19 @@
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3' 
 ]
 
 setup(
 
     name='foodbook_discount',
-    version='0.0.1',
+    version='0.0.3',
     description='Package created for using discount function',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='Akash Sane',
     author_email='x21220956@student.ncirl.ie',
     license='MIT',
     classifiers=classifiers,
     keywords='discount',
-    packages=find_packages(),
+    packages=find_packages('discount'),
     install_requires=['']
 )
```

