# Comparing `tmp/wordpress-scanner-1.1.tar.gz` & `tmp/wordpress-scanner-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordpress-scanner-1.1.tar", last modified: Thu Apr 13 18:28:09 2023, max compression
+gzip compressed data, was "wordpress-scanner-1.2.tar", last modified: Sun Apr 23 21:37:55 2023, max compression
```

## Comparing `wordpress-scanner-1.1.tar` & `wordpress-scanner-1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 18:28:09.136179 wordpress-scanner-1.1/
--rw-rw-rw-   0        0        0     1603 2023-04-13 18:28:09.135178 wordpress-scanner-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1122 2023-04-13 18:24:20.000000 wordpress-scanner-1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 18:28:09.136179 wordpress-scanner-1.1/setup.cfg
--rw-rw-rw-   0        0        0      715 2023-04-13 18:27:56.000000 wordpress-scanner-1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:28:09.133181 wordpress-scanner-1.1/wordpress_scanner.egg-info/
--rw-rw-rw-   0        0        0     1603 2023-04-13 18:28:08.000000 wordpress-scanner-1.1/wordpress_scanner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-04-13 18:28:09.000000 wordpress-scanner-1.1/wordpress_scanner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 18:28:08.000000 wordpress-scanner-1.1/wordpress_scanner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 18:28:08.000000 wordpress-scanner-1.1/wordpress_scanner.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 21:37:55.616880 wordpress-scanner-1.2/
+-rw-rw-rw-   0        0        0     1603 2023-04-23 21:37:55.610868 wordpress-scanner-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1122 2023-04-13 18:24:20.000000 wordpress-scanner-1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-23 21:37:55.617858 wordpress-scanner-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      715 2023-04-23 21:37:47.000000 wordpress-scanner-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 21:37:55.604856 wordpress-scanner-1.2/wordpress_scanner.egg-info/
+-rw-rw-rw-   0        0        0     1603 2023-04-23 21:37:55.000000 wordpress-scanner-1.2/wordpress_scanner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-04-23 21:37:55.000000 wordpress-scanner-1.2/wordpress_scanner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 21:37:55.000000 wordpress-scanner-1.2/wordpress_scanner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 21:37:55.000000 wordpress-scanner-1.2/wordpress_scanner.egg-info/top_level.txt
```

### Comparing `wordpress-scanner-1.1/PKG-INFO` & `wordpress-scanner-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordpress-scanner
-Version: 1.1
+Version: 1.2
 Summary: A theme, username, plugin name browser for Flask in Python
 Home-page: https://github.com/firatylmz06/wordpress-scanner
 Author: Fırat YILMAZ
 Author-email: iletisim@firatyilmaz.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wordpress-scanner-1.1/README.md` & `wordpress-scanner-1.2/README.md`

 * *Files identical despite different names*

### Comparing `wordpress-scanner-1.1/setup.py` & `wordpress-scanner-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
  
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name='wordpress-scanner',
-    version='1.1',
+    version='1.2',
     author='Fırat YILMAZ',
     author_email='iletisim@firatyilmaz.com',    
     description='A theme, username, plugin name browser for Flask in Python',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/firatylmz06/wordpress-scanner",
     packages=setuptools.find_packages(),
```

### Comparing `wordpress-scanner-1.1/wordpress_scanner.egg-info/PKG-INFO` & `wordpress-scanner-1.2/wordpress_scanner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordpress-scanner
-Version: 1.1
+Version: 1.2
 Summary: A theme, username, plugin name browser for Flask in Python
 Home-page: https://github.com/firatylmz06/wordpress-scanner
 Author: Fırat YILMAZ
 Author-email: iletisim@firatyilmaz.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

