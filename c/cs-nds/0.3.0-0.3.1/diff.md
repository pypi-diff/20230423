# Comparing `tmp/cs-nds-0.3.0.tar.gz` & `tmp/cs-nds-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs-nds-0.3.0.tar", last modified: Tue Apr 18 09:26:34 2023, max compression
+gzip compressed data, was "cs-nds-0.3.1.tar", last modified: Sun Apr 23 20:01:39 2023, max compression
```

## Comparing `cs-nds-0.3.0.tar` & `cs-nds-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 alex      (1000) wheel      (998)        0 2023-04-18 09:26:34.455708 cs-nds-0.3.0/
--rw-r--r--   0 alex      (1000) wheel      (998)    35149 2023-03-19 20:03:06.000000 cs-nds-0.3.0/LICENSE
--rw-r--r--   0 alex      (1000) wheel      (998)     1623 2023-04-18 09:26:34.452375 cs-nds-0.3.0/PKG-INFO
--rw-r--r--   0 alex      (1000) wheel      (998)      935 2023-04-18 09:21:32.000000 cs-nds-0.3.0/README.md
-drwxr-xr-x   0 alex      (1000) wheel      (998)        0 2023-04-18 09:26:34.452375 cs-nds-0.3.0/cs_nds/
--rw-r--r--   0 alex      (1000) wheel      (998)      112 2023-04-18 08:56:46.000000 cs-nds-0.3.0/cs_nds/__init__.py
--rw-r--r--   0 alex      (1000) wheel      (998)     1018 2023-04-18 09:04:08.000000 cs-nds-0.3.0/cs_nds/bintree.py
--rw-r--r--   0 alex      (1000) wheel      (998)      995 2023-04-18 09:13:54.000000 cs-nds-0.3.0/cs_nds/dynarray.py
--rw-r--r--   0 alex      (1000) wheel      (998)      346 2023-03-19 20:05:10.000000 cs-nds-0.3.0/cs_nds/queue.py
--rw-r--r--   0 alex      (1000) wheel      (998)      902 2023-04-18 09:16:48.000000 cs-nds-0.3.0/cs_nds/stack.py
-drwxr-xr-x   0 alex      (1000) wheel      (998)        0 2023-04-18 09:26:34.452375 cs-nds-0.3.0/cs_nds.egg-info/
--rw-r--r--   0 alex      (1000) wheel      (998)     1623 2023-04-18 09:26:34.000000 cs-nds-0.3.0/cs_nds.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) wheel      (998)      234 2023-04-18 09:26:34.000000 cs-nds-0.3.0/cs_nds.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) wheel      (998)        1 2023-04-18 09:26:34.000000 cs-nds-0.3.0/cs_nds.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) wheel      (998)        7 2023-04-18 09:26:34.000000 cs-nds-0.3.0/cs_nds.egg-info/top_level.txt
--rw-r--r--   0 alex      (1000) wheel      (998)       38 2023-04-18 09:26:34.455708 cs-nds-0.3.0/setup.cfg
--rw-r--r--   0 alex      (1000) wheel      (998)     1034 2023-04-18 09:18:49.000000 cs-nds-0.3.0/setup.py
+drwxr-xr-x   0 alex      (1000) wheel      (998)        0 2023-04-23 20:01:39.255313 cs-nds-0.3.1/
+-rw-r--r--   0 alex      (1000) wheel      (998)    35149 2023-03-19 20:03:06.000000 cs-nds-0.3.1/LICENSE
+-rw-r--r--   0 alex      (1000) wheel      (998)     1677 2023-04-23 20:01:39.255313 cs-nds-0.3.1/PKG-INFO
+-rw-r--r--   0 alex      (1000) wheel      (998)      989 2023-04-23 20:00:54.000000 cs-nds-0.3.1/README.md
+drwxr-xr-x   0 alex      (1000) wheel      (998)        0 2023-04-23 20:01:39.255313 cs-nds-0.3.1/cs_nds/
+-rw-r--r--   0 alex      (1000) wheel      (998)      112 2023-04-18 08:56:46.000000 cs-nds-0.3.1/cs_nds/__init__.py
+-rw-r--r--   0 alex      (1000) wheel      (998)     1077 2023-04-23 19:57:57.000000 cs-nds-0.3.1/cs_nds/bintree.py
+-rw-r--r--   0 alex      (1000) wheel      (998)      995 2023-04-18 09:13:54.000000 cs-nds-0.3.1/cs_nds/dynarray.py
+-rw-r--r--   0 alex      (1000) wheel      (998)      346 2023-03-19 20:05:10.000000 cs-nds-0.3.1/cs_nds/queue.py
+-rw-r--r--   0 alex      (1000) wheel      (998)      902 2023-04-18 09:16:48.000000 cs-nds-0.3.1/cs_nds/stack.py
+drwxr-xr-x   0 alex      (1000) wheel      (998)        0 2023-04-23 20:01:39.255313 cs-nds-0.3.1/cs_nds.egg-info/
+-rw-r--r--   0 alex      (1000) wheel      (998)     1677 2023-04-23 20:01:39.000000 cs-nds-0.3.1/cs_nds.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) wheel      (998)      234 2023-04-23 20:01:39.000000 cs-nds-0.3.1/cs_nds.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) wheel      (998)        1 2023-04-23 20:01:39.000000 cs-nds-0.3.1/cs_nds.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) wheel      (998)        7 2023-04-23 20:01:39.000000 cs-nds-0.3.1/cs_nds.egg-info/top_level.txt
+-rw-r--r--   0 alex      (1000) wheel      (998)       38 2023-04-23 20:01:39.255313 cs-nds-0.3.1/setup.cfg
+-rw-r--r--   0 alex      (1000) wheel      (998)     1034 2023-04-23 20:01:19.000000 cs-nds-0.3.1/setup.py
```

### Comparing `cs-nds-0.3.0/LICENSE` & `cs-nds-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cs-nds-0.3.0/PKG-INFO` & `cs-nds-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs-nds
-Version: 0.3.0
+Version: 0.3.1
 Summary: Often used things for Computer Science classes
 Home-page: https://github.com/alexcoder04/cs_nds
 Author: alexcoder04
 Author-email: alexcoder04@protonmail.com
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
@@ -41,14 +41,19 @@
 pip install cs-nds
 ```
 
 To use it in your code, just import it:
 
 ```python
 import cs_nds
+
+my_queue = cs_nds.Queue()
+my_queue.enqueue(3)
+
+# ...
 ```
 
 ## Data Structures
 
  - `Stack` ("Stapel" / stack)
  - `Queue` ("(Warte-)Schlange" / queue)
  - `DynArray` ("Dynamische Reihung" / dynamic array)
```

### Comparing `cs-nds-0.3.0/README.md` & `cs-nds-0.3.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -23,14 +23,19 @@
 pip install cs-nds
 ```
 
 To use it in your code, just import it:
 
 ```python
 import cs_nds
+
+my_queue = cs_nds.Queue()
+my_queue.enqueue(3)
+
+# ...
 ```
 
 ## Data Structures
 
  - `Stack` ("Stapel" / stack)
  - `Queue` ("(Warte-)Schlange" / queue)
  - `DynArray` ("Dynamische Reihung" / dynamic array)
```

### Comparing `cs-nds-0.3.0/cs_nds/bintree.py` & `cs-nds-0.3.1/cs_nds/bintree.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,17 @@
         self.__value = inhalt
         self.__left = None
         self.__right = None
 
     def hasItem(self) -> bool:
         return self.__value is not None
 
+    def getItem(self) -> any:
+        return self.__value
+
     def setItem(self, inhalt: any) -> None:
         self.__value = inhalt
 
     def deleteItem(self) -> None:
         self.__value = None
 
     def isLeaf(self) -> bool:
```

### Comparing `cs-nds-0.3.0/cs_nds/dynarray.py` & `cs-nds-0.3.1/cs_nds/dynarray.py`

 * *Files identical despite different names*

### Comparing `cs-nds-0.3.0/cs_nds/stack.py` & `cs-nds-0.3.1/cs_nds/stack.py`

 * *Files identical despite different names*

### Comparing `cs-nds-0.3.0/cs_nds.egg-info/PKG-INFO` & `cs-nds-0.3.1/cs_nds.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs-nds
-Version: 0.3.0
+Version: 0.3.1
 Summary: Often used things for Computer Science classes
 Home-page: https://github.com/alexcoder04/cs_nds
 Author: alexcoder04
 Author-email: alexcoder04@protonmail.com
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
@@ -41,14 +41,19 @@
 pip install cs-nds
 ```
 
 To use it in your code, just import it:
 
 ```python
 import cs_nds
+
+my_queue = cs_nds.Queue()
+my_queue.enqueue(3)
+
+# ...
 ```
 
 ## Data Structures
 
  - `Stack` ("Stapel" / stack)
  - `Queue` ("(Warte-)Schlange" / queue)
  - `DynArray` ("Dynamische Reihung" / dynamic array)
```

### Comparing `cs-nds-0.3.0/setup.py` & `cs-nds-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="cs-nds",
-    version="0.3.0",
+    version="0.3.1",
     description="Often used things for Computer Science classes",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/alexcoder04/cs_nds",
     author="alexcoder04",
     author_email="alexcoder04@protonmail.com",
     classifiers=[
```

