# Comparing `tmp/oa-0.0.7.tar.gz` & `tmp/oa-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oa-0.0.7.tar", last modified: Sun Apr 23 00:00:01 2023, max compression
+gzip compressed data, was "oa-0.0.8.tar", last modified: Sun Apr 23 00:02:07 2023, max compression
```

## Comparing `oa-0.0.7.tar` & `oa-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 thorwhalen   (501) staff       (20)        0 2023-04-23 00:00:01.378959 oa-0.0.7/
--rw-r--r--   0 thorwhalen   (501) staff       (20)    11357 2023-03-06 13:22:17.000000 oa-0.0.7/LICENSE
--rw-r--r--   0 thorwhalen   (501) staff       (20)    11684 2023-04-23 00:00:01.379127 oa-0.0.7/PKG-INFO
--rw-r--r--   0 thorwhalen   (501) staff       (20)    11441 2023-04-22 23:58:59.000000 oa-0.0.7/README.md
-drwxr-xr-x   0 thorwhalen   (501) staff       (20)        0 2023-04-23 00:00:01.247339 oa-0.0.7/oa/
--rw-r--r--   0 thorwhalen   (501) staff       (20)      182 2023-04-22 20:50:59.000000 oa-0.0.7/oa/__init__.py
--rw-r--r--   0 thorwhalen   (501) staff       (20)     2566 2023-04-22 23:17:50.000000 oa-0.0.7/oa/base.py
-drwxr-xr-x   0 thorwhalen   (501) staff       (20)        0 2023-04-23 00:00:01.375564 oa-0.0.7/oa/examples/
--rw-r--r--   0 thorwhalen   (501) staff       (20)        0 2023-03-31 14:33:35.000000 oa-0.0.7/oa/examples/__init__.py
--rw-r--r--   0 thorwhalen   (501) staff       (20)     4427 2023-04-22 23:15:19.000000 oa-0.0.7/oa/examples/illustrate_stories.py
--rw-r--r--   0 thorwhalen   (501) staff       (20)    11564 2023-04-22 23:05:43.000000 oa-0.0.7/oa/openai_specs.py
-drwxr-xr-x   0 thorwhalen   (501) staff       (20)        0 2023-04-23 00:00:01.377301 oa-0.0.7/oa/scrap/
--rw-r--r--   0 thorwhalen   (501) staff       (20)        1 2023-04-22 11:54:07.000000 oa-0.0.7/oa/scrap/__init__.py
--rw-r--r--   0 thorwhalen   (501) staff       (20)     2153 2023-04-22 14:36:27.000000 oa-0.0.7/oa/util.py
-drwxr-xr-x   0 thorwhalen   (501) staff       (20)        0 2023-04-23 00:00:01.351253 oa-0.0.7/oa.egg-info/
--rw-r--r--   0 thorwhalen   (501) staff       (20)    11684 2023-04-22 23:59:59.000000 oa-0.0.7/oa.egg-info/PKG-INFO
--rw-r--r--   0 thorwhalen   (501) staff       (20)      325 2023-04-23 00:00:00.000000 oa-0.0.7/oa.egg-info/SOURCES.txt
--rw-r--r--   0 thorwhalen   (501) staff       (20)        1 2023-04-22 23:59:59.000000 oa-0.0.7/oa.egg-info/dependency_links.txt
--rw-r--r--   0 thorwhalen   (501) staff       (20)        1 2023-04-22 23:59:59.000000 oa-0.0.7/oa.egg-info/not-zip-safe
--rw-r--r--   0 thorwhalen   (501) staff       (20)       14 2023-04-22 23:59:59.000000 oa-0.0.7/oa.egg-info/requires.txt
--rw-r--r--   0 thorwhalen   (501) staff       (20)        3 2023-04-22 23:59:59.000000 oa-0.0.7/oa.egg-info/top_level.txt
--rw-r--r--   0 thorwhalen   (501) staff       (20)      505 2023-04-23 00:00:01.382104 oa-0.0.7/setup.cfg
--rw-r--r--   0 thorwhalen   (501) staff       (20)       91 2023-03-06 13:22:17.000000 oa-0.0.7/setup.py
+drwxr-xr-x   0 thorwhalen   (501) staff       (20)        0 2023-04-23 00:02:07.083784 oa-0.0.8/
+-rw-r--r--   0 thorwhalen   (501) staff       (20)    11357 2023-03-06 13:22:17.000000 oa-0.0.8/LICENSE
+-rw-r--r--   0 thorwhalen   (501) staff       (20)    11726 2023-04-23 00:02:07.083923 oa-0.0.8/PKG-INFO
+-rw-r--r--   0 thorwhalen   (501) staff       (20)    11483 2023-04-23 00:01:40.000000 oa-0.0.8/README.md
+drwxr-xr-x   0 thorwhalen   (501) staff       (20)        0 2023-04-23 00:02:07.068768 oa-0.0.8/oa/
+-rw-r--r--   0 thorwhalen   (501) staff       (20)      182 2023-04-22 20:50:59.000000 oa-0.0.8/oa/__init__.py
+-rw-r--r--   0 thorwhalen   (501) staff       (20)     2566 2023-04-22 23:17:50.000000 oa-0.0.8/oa/base.py
+drwxr-xr-x   0 thorwhalen   (501) staff       (20)        0 2023-04-23 00:02:07.081445 oa-0.0.8/oa/examples/
+-rw-r--r--   0 thorwhalen   (501) staff       (20)        0 2023-03-31 14:33:35.000000 oa-0.0.8/oa/examples/__init__.py
+-rw-r--r--   0 thorwhalen   (501) staff       (20)     4427 2023-04-22 23:15:19.000000 oa-0.0.8/oa/examples/illustrate_stories.py
+-rw-r--r--   0 thorwhalen   (501) staff       (20)    11564 2023-04-22 23:05:43.000000 oa-0.0.8/oa/openai_specs.py
+drwxr-xr-x   0 thorwhalen   (501) staff       (20)        0 2023-04-23 00:02:07.082815 oa-0.0.8/oa/scrap/
+-rw-r--r--   0 thorwhalen   (501) staff       (20)        1 2023-04-22 11:54:07.000000 oa-0.0.8/oa/scrap/__init__.py
+-rw-r--r--   0 thorwhalen   (501) staff       (20)     2153 2023-04-22 14:36:27.000000 oa-0.0.8/oa/util.py
+drwxr-xr-x   0 thorwhalen   (501) staff       (20)        0 2023-04-23 00:02:07.079170 oa-0.0.8/oa.egg-info/
+-rw-r--r--   0 thorwhalen   (501) staff       (20)    11726 2023-04-23 00:02:06.000000 oa-0.0.8/oa.egg-info/PKG-INFO
+-rw-r--r--   0 thorwhalen   (501) staff       (20)      325 2023-04-23 00:02:06.000000 oa-0.0.8/oa.egg-info/SOURCES.txt
+-rw-r--r--   0 thorwhalen   (501) staff       (20)        1 2023-04-23 00:02:06.000000 oa-0.0.8/oa.egg-info/dependency_links.txt
+-rw-r--r--   0 thorwhalen   (501) staff       (20)        1 2023-04-23 00:02:06.000000 oa-0.0.8/oa.egg-info/not-zip-safe
+-rw-r--r--   0 thorwhalen   (501) staff       (20)       14 2023-04-23 00:02:06.000000 oa-0.0.8/oa.egg-info/requires.txt
+-rw-r--r--   0 thorwhalen   (501) staff       (20)        3 2023-04-23 00:02:06.000000 oa-0.0.8/oa.egg-info/top_level.txt
+-rw-r--r--   0 thorwhalen   (501) staff       (20)      505 2023-04-23 00:02:07.085172 oa-0.0.8/setup.cfg
+-rw-r--r--   0 thorwhalen   (501) staff       (20)       91 2023-03-06 13:22:17.000000 oa-0.0.8/setup.py
```

### Comparing `oa-0.0.7/LICENSE` & `oa-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `oa-0.0.7/PKG-INFO` & `oa-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oa
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python interface to OpenAi
 Home-page: https://github.com/thorwhalen/oa
 Author: Thor Whalen
 License: apache-2.0
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -82,15 +82,15 @@
 
 
 
 <img src="https://oaidalleapiprodscus.blob.core.windows.net/private/org-AY3lr3H3xB9yPQ0HGR498f9M/user-7ZNCDYLWzP0GT48V6DCiTFWt/img-pNE6fCWGN3eJGj7ycFwZREhi.png?st=2023-04-22T22%3A17%3A03Z&se=2023-04-23T00%3A17%3A03Z&sp=r&sv=2021-08-06&sr=b&rscd=inline&rsct=image/png&skoid=6aaadede-4fb3-4698-a8f6-684d7786b067&sktid=a48cca56-e6da-484e-a814-9c849652bcb3&skt=2023-04-22T21%3A08%3A14Z&ske=2023-04-23T21%3A08%3A14Z&sks=b&skv=2021-08-06&sig=5j6LPVO992R95dllAAjbmOXzS0MORD06Fo8unwtGNl0%3D"/>
 
 
 
-## Raw form
+## Raw form - When you need to be closer to the metal
 
 The `raw` object is a thin layer on top of the `openai` package, which is itself a thin layer over the web requests. 
 
 What was unsatisfactory with the `openai` package is (1) finding the right function, (2) the signature of the function once you found it, and (3) the documentation of the function. 
 What raw contains is pointers to the main functionalities (not all available -- yet), with nice signatures and documentation, extracted from the web service openAPI specs themselves. 
 
 For example, to ask chatGPT something, the openai function is `openai.ChatCompletion.create`, or to get simple completions, the function is `openai.Completion.create` whose help is:
```

### Comparing `oa-0.0.7/README.md` & `oa-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 
 
 <img src="https://oaidalleapiprodscus.blob.core.windows.net/private/org-AY3lr3H3xB9yPQ0HGR498f9M/user-7ZNCDYLWzP0GT48V6DCiTFWt/img-pNE6fCWGN3eJGj7ycFwZREhi.png?st=2023-04-22T22%3A17%3A03Z&se=2023-04-23T00%3A17%3A03Z&sp=r&sv=2021-08-06&sr=b&rscd=inline&rsct=image/png&skoid=6aaadede-4fb3-4698-a8f6-684d7786b067&sktid=a48cca56-e6da-484e-a814-9c849652bcb3&skt=2023-04-22T21%3A08%3A14Z&ske=2023-04-23T21%3A08%3A14Z&sks=b&skv=2021-08-06&sig=5j6LPVO992R95dllAAjbmOXzS0MORD06Fo8unwtGNl0%3D"/>
 
 
 
-## Raw form
+## Raw form - When you need to be closer to the metal
 
 The `raw` object is a thin layer on top of the `openai` package, which is itself a thin layer over the web requests. 
 
 What was unsatisfactory with the `openai` package is (1) finding the right function, (2) the signature of the function once you found it, and (3) the documentation of the function. 
 What raw contains is pointers to the main functionalities (not all available -- yet), with nice signatures and documentation, extracted from the web service openAPI specs themselves. 
 
 For example, to ask chatGPT something, the openai function is `openai.ChatCompletion.create`, or to get simple completions, the function is `openai.Completion.create` whose help is:
```

### Comparing `oa-0.0.7/oa/base.py` & `oa-0.0.8/oa/base.py`

 * *Files identical despite different names*

### Comparing `oa-0.0.7/oa/examples/illustrate_stories.py` & `oa-0.0.8/oa/examples/illustrate_stories.py`

 * *Files identical despite different names*

### Comparing `oa-0.0.7/oa/openai_specs.py` & `oa-0.0.8/oa/openai_specs.py`

 * *Files identical despite different names*

### Comparing `oa-0.0.7/oa/util.py` & `oa-0.0.8/oa/util.py`

 * *Files identical despite different names*

### Comparing `oa-0.0.7/oa.egg-info/PKG-INFO` & `oa-0.0.8/oa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oa
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python interface to OpenAi
 Home-page: https://github.com/thorwhalen/oa
 Author: Thor Whalen
 License: apache-2.0
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -82,15 +82,15 @@
 
 
 
 <img src="https://oaidalleapiprodscus.blob.core.windows.net/private/org-AY3lr3H3xB9yPQ0HGR498f9M/user-7ZNCDYLWzP0GT48V6DCiTFWt/img-pNE6fCWGN3eJGj7ycFwZREhi.png?st=2023-04-22T22%3A17%3A03Z&se=2023-04-23T00%3A17%3A03Z&sp=r&sv=2021-08-06&sr=b&rscd=inline&rsct=image/png&skoid=6aaadede-4fb3-4698-a8f6-684d7786b067&sktid=a48cca56-e6da-484e-a814-9c849652bcb3&skt=2023-04-22T21%3A08%3A14Z&ske=2023-04-23T21%3A08%3A14Z&sks=b&skv=2021-08-06&sig=5j6LPVO992R95dllAAjbmOXzS0MORD06Fo8unwtGNl0%3D"/>
 
 
 
-## Raw form
+## Raw form - When you need to be closer to the metal
 
 The `raw` object is a thin layer on top of the `openai` package, which is itself a thin layer over the web requests. 
 
 What was unsatisfactory with the `openai` package is (1) finding the right function, (2) the signature of the function once you found it, and (3) the documentation of the function. 
 What raw contains is pointers to the main functionalities (not all available -- yet), with nice signatures and documentation, extracted from the web service openAPI specs themselves. 
 
 For example, to ask chatGPT something, the openai function is `openai.ChatCompletion.create`, or to get simple completions, the function is `openai.Completion.create` whose help is:
```

