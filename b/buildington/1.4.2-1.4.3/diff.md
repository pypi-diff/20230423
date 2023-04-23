# Comparing `tmp/buildington-1.4.2.tar.gz` & `tmp/buildington-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildington-1.4.2.tar", last modified: Sun Apr 23 10:40:24 2023, max compression
+gzip compressed data, was "buildington-1.4.3.tar", last modified: Sun Apr 23 10:52:06 2023, max compression
```

## Comparing `buildington-1.4.2.tar` & `buildington-1.4.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 10:40:24.649411 buildington-1.4.2/
--rw-rw-rw-   0        0        0     1831 2023-04-23 10:40:24.649411 buildington-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     1305 2023-04-23 10:40:05.000000 buildington-1.4.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-23 10:40:24.618162 buildington-1.4.2/buildington/
--rw-rw-rw-   0        0        0     3594 2023-04-23 09:05:44.000000 buildington-1.4.2/buildington/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 10:40:24.649411 buildington-1.4.2/buildington.egg-info/
--rw-rw-rw-   0        0        0     1831 2023-04-23 10:40:24.000000 buildington-1.4.2/buildington.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-04-23 10:40:24.000000 buildington-1.4.2/buildington.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 10:40:24.000000 buildington-1.4.2/buildington.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-23 10:40:24.000000 buildington-1.4.2/buildington.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-23 10:40:24.000000 buildington-1.4.2/buildington.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 10:40:24.649411 buildington-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0      650 2023-04-23 10:40:12.000000 buildington-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:52:06.473681 buildington-1.4.3/
+-rw-rw-rw-   0        0        0     2259 2023-04-23 10:52:06.473681 buildington-1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1733 2023-04-23 10:51:50.000000 buildington-1.4.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 10:52:06.426808 buildington-1.4.3/buildington/
+-rw-rw-rw-   0        0        0     3594 2023-04-23 09:05:44.000000 buildington-1.4.3/buildington/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:52:06.473681 buildington-1.4.3/buildington.egg-info/
+-rw-rw-rw-   0        0        0     2259 2023-04-23 10:52:06.000000 buildington-1.4.3/buildington.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-04-23 10:52:06.000000 buildington-1.4.3/buildington.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 10:52:06.000000 buildington-1.4.3/buildington.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-23 10:52:06.000000 buildington-1.4.3/buildington.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-23 10:52:06.000000 buildington-1.4.3/buildington.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 10:52:06.473681 buildington-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      650 2023-04-23 10:51:54.000000 buildington-1.4.3/setup.py
```

### Comparing `buildington-1.4.2/PKG-INFO` & `buildington-1.4.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 Metadata-Version: 2.1
 Name: buildington
-Version: 1.4.2
+Version: 1.4.3
 Summary: Building websites like React, and hosting 'em like Flask!
 Author: RixTheTyrunt
 Author-email: rixthetyrunt@gmail.com
 Classifier: Environment :: Console
 Classifier: Framework :: Flask
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Server
 Description-Content-Type: text/plain
 
-Coding crap:
+++--------------------------------------++
+++--------------------------------------++
+|| |)     . |   + .          +          ||
+|| |+ | | | | +-+ | +-+ +-+ -+- +-+ +-+ ||
+|| |) +-+ | | +-+ | | | +-+  +  +-+ | | ||
+||                        |             ||
+||                       -+             ||
+||                      By RixTheTyrunt ||
+++--------------------------------------++
+++--------------------------------------++
+
 You can use the [buildington.page] decorator and/or the [buildington.addFile] method to add a route to your website. Here's an example of both:
 +------------------------------------------------------------------------------+
 | Python                                                                       |
 +------------------------------------------------------------------------------+
 | import buildington                                                           |
 |                                                                              |
 | buildington.addFile("README.txt")                                            |
```

### Comparing `buildington-1.4.2/buildington/__init__.py` & `buildington-1.4.3/buildington/__init__.py`

 * *Files identical despite different names*

### Comparing `buildington-1.4.2/buildington.egg-info/PKG-INFO` & `buildington-1.4.3/buildington.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 Metadata-Version: 2.1
 Name: buildington
-Version: 1.4.2
+Version: 1.4.3
 Summary: Building websites like React, and hosting 'em like Flask!
 Author: RixTheTyrunt
 Author-email: rixthetyrunt@gmail.com
 Classifier: Environment :: Console
 Classifier: Framework :: Flask
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Server
 Description-Content-Type: text/plain
 
-Coding crap:
+++--------------------------------------++
+++--------------------------------------++
+|| |)     . |   + .          +          ||
+|| |+ | | | | +-+ | +-+ +-+ -+- +-+ +-+ ||
+|| |) +-+ | | +-+ | | | +-+  +  +-+ | | ||
+||                        |             ||
+||                       -+             ||
+||                      By RixTheTyrunt ||
+++--------------------------------------++
+++--------------------------------------++
+
 You can use the [buildington.page] decorator and/or the [buildington.addFile] method to add a route to your website. Here's an example of both:
 +------------------------------------------------------------------------------+
 | Python                                                                       |
 +------------------------------------------------------------------------------+
 | import buildington                                                           |
 |                                                                              |
 | buildington.addFile("README.txt")                                            |
```

### Comparing `buildington-1.4.2/setup.py` & `buildington-1.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
 	name="buildington",
-	version="1.4.2",
+	version="1.4.3",
 	author="RixTheTyrunt",
 	author_email="rixthetyrunt@gmail.com",
 	description="Building websites like React, and hosting 'em like Flask!",
 	packages=["buildington"],
 	classifiers=[
 		"Environment :: Console",
 		"Framework :: Flask",
```

