# Comparing `tmp/gpt4all-j-0.2.0.tar.gz` & `tmp/gpt4all-j-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt4all-j-0.2.0.tar", last modified: Sun Apr 23 18:16:25 2023, max compression
+gzip compressed data, was "gpt4all-j-0.2.1.tar", last modified: Sun Apr 23 18:34:34 2023, max compression
```

## Comparing `gpt4all-j-0.2.0.tar` & `gpt4all-j-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-23 18:16:25.169914 gpt4all-j-0.2.0/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     3521 2023-04-23 18:16:25.169914 gpt4all-j-0.2.0/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1931 2023-04-23 18:09:05.000000 gpt4all-j-0.2.0/README.md
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-23 18:16:25.169914 gpt4all-j-0.2.0/gpt4all_j.egg-info/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     3521 2023-04-23 18:16:25.000000 gpt4all-j-0.2.0/gpt4all_j.egg-info/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      615 2023-04-23 18:16:25.000000 gpt4all-j-0.2.0/gpt4all_j.egg-info/SOURCES.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-04-23 18:16:25.000000 gpt4all-j-0.2.0/gpt4all_j.egg-info/dependency_links.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-04-23 18:16:25.000000 gpt4all-j-0.2.0/gpt4all_j.egg-info/not-zip-safe
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       16 2023-04-23 18:16:25.000000 gpt4all-j-0.2.0/gpt4all_j.egg-info/requires.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        9 2023-04-23 18:16:25.000000 gpt4all-j-0.2.0/gpt4all_j.egg-info/top_level.txt
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-23 18:16:25.169914 gpt4all-j-0.2.0/gpt4allj/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       55 2023-04-17 19:06:48.000000 gpt4all-j-0.2.0/gpt4allj/__init__.py
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-23 18:16:25.159914 gpt4all-j-0.2.0/gpt4allj/lib/
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-23 18:16:25.169914 gpt4all-j-0.2.0/gpt4allj/lib/avx/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   141824 2023-04-23 16:38:33.000000 gpt4all-j-0.2.0/gpt4allj/lib/avx/ggml.dll
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   154624 2023-04-23 16:38:33.000000 gpt4all-j-0.2.0/gpt4allj/lib/avx/gptj.dll
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   433850 2023-04-23 16:38:33.000000 gpt4all-j-0.2.0/gpt4allj/lib/avx/libggml.dylib
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   174048 2023-04-23 16:38:33.000000 gpt4all-j-0.2.0/gpt4allj/lib/avx/libggml.so
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   346954 2023-04-23 16:38:33.000000 gpt4all-j-0.2.0/gpt4allj/lib/avx/libgptj.dylib
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   264224 2023-04-23 16:38:33.000000 gpt4all-j-0.2.0/gpt4allj/lib/avx/libgptj.so
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-23 18:16:25.169914 gpt4all-j-0.2.0/gpt4allj/lib/avx2/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   131072 2023-04-23 16:38:33.000000 gpt4all-j-0.2.0/gpt4allj/lib/avx2/ggml.dll
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   154624 2023-04-23 16:38:33.000000 gpt4all-j-0.2.0/gpt4allj/lib/avx2/gptj.dll
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   433850 2023-04-23 16:38:33.000000 gpt4all-j-0.2.0/gpt4allj/lib/avx2/libggml.dylib
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   169848 2023-04-23 16:38:33.000000 gpt4all-j-0.2.0/gpt4allj/lib/avx2/libggml.so
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   346954 2023-04-23 16:38:33.000000 gpt4all-j-0.2.0/gpt4allj/lib/avx2/libgptj.dylib
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   264224 2023-04-23 16:38:33.000000 gpt4all-j-0.2.0/gpt4allj/lib/avx2/libgptj.so
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1766 2023-04-23 16:18:35.000000 gpt4all-j-0.2.0/gpt4allj/lib.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1816 2023-04-23 16:21:53.000000 gpt4all-j-0.2.0/gpt4allj/model.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-04-23 18:16:25.169914 gpt4all-j-0.2.0/setup.cfg
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1396 2023-04-23 18:09:53.000000 gpt4all-j-0.2.0/setup.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-23 18:34:34.499916 gpt4all-j-0.2.1/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     3530 2023-04-23 18:34:34.499916 gpt4all-j-0.2.1/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1932 2023-04-23 18:17:44.000000 gpt4all-j-0.2.1/README.md
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-23 18:34:34.489916 gpt4all-j-0.2.1/gpt4all_j.egg-info/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     3530 2023-04-23 18:34:34.000000 gpt4all-j-0.2.1/gpt4all_j.egg-info/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      615 2023-04-23 18:34:34.000000 gpt4all-j-0.2.1/gpt4all_j.egg-info/SOURCES.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-04-23 18:34:34.000000 gpt4all-j-0.2.1/gpt4all_j.egg-info/dependency_links.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-04-23 18:34:34.000000 gpt4all-j-0.2.1/gpt4all_j.egg-info/not-zip-safe
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       16 2023-04-23 18:34:34.000000 gpt4all-j-0.2.1/gpt4all_j.egg-info/requires.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        9 2023-04-23 18:34:34.000000 gpt4all-j-0.2.1/gpt4all_j.egg-info/top_level.txt
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-23 18:34:34.489916 gpt4all-j-0.2.1/gpt4allj/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       55 2023-04-17 19:06:48.000000 gpt4all-j-0.2.1/gpt4allj/__init__.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-23 18:34:34.489916 gpt4all-j-0.2.1/gpt4allj/lib/
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-23 18:34:34.499916 gpt4all-j-0.2.1/gpt4allj/lib/avx/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   141824 2023-04-23 16:38:33.000000 gpt4all-j-0.2.1/gpt4allj/lib/avx/ggml.dll
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   154624 2023-04-23 16:38:33.000000 gpt4all-j-0.2.1/gpt4allj/lib/avx/gptj.dll
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   433850 2023-04-23 16:38:33.000000 gpt4all-j-0.2.1/gpt4allj/lib/avx/libggml.dylib
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   174048 2023-04-23 16:38:33.000000 gpt4all-j-0.2.1/gpt4allj/lib/avx/libggml.so
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   346954 2023-04-23 16:38:33.000000 gpt4all-j-0.2.1/gpt4allj/lib/avx/libgptj.dylib
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   264224 2023-04-23 16:38:33.000000 gpt4all-j-0.2.1/gpt4allj/lib/avx/libgptj.so
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-23 18:34:34.499916 gpt4all-j-0.2.1/gpt4allj/lib/avx2/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   131072 2023-04-23 16:38:33.000000 gpt4all-j-0.2.1/gpt4allj/lib/avx2/ggml.dll
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   154624 2023-04-23 16:38:33.000000 gpt4all-j-0.2.1/gpt4allj/lib/avx2/gptj.dll
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   433850 2023-04-23 16:38:33.000000 gpt4all-j-0.2.1/gpt4allj/lib/avx2/libggml.dylib
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   169848 2023-04-23 16:38:33.000000 gpt4all-j-0.2.1/gpt4allj/lib/avx2/libggml.so
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   346954 2023-04-23 16:38:33.000000 gpt4all-j-0.2.1/gpt4allj/lib/avx2/libgptj.dylib
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   264224 2023-04-23 16:38:33.000000 gpt4all-j-0.2.1/gpt4allj/lib/avx2/libgptj.so
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1766 2023-04-23 16:18:35.000000 gpt4all-j-0.2.1/gpt4allj/lib.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1816 2023-04-23 16:21:53.000000 gpt4all-j-0.2.1/gpt4allj/model.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-04-23 18:34:34.499916 gpt4all-j-0.2.1/setup.cfg
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1396 2023-04-23 18:18:47.000000 gpt4all-j-0.2.1/setup.py
```

### Comparing `gpt4all-j-0.2.0/PKG-INFO` & `gpt4all-j-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt4all-j
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python bindings for the C++ port of GPT4All-J model.
 Home-page: https://github.com/marella/gpt4all-j
 Author: Ravindra Marella
 Author-email: mv.ravindra007@gmail.com
 License: MIT
 Description: # [GPT4All-J](https://github.com/marella/gpt4all-j) [![tests](https://github.com/marella/gpt4all-j/actions/workflows/tests.yml/badge.svg)](https://github.com/marella/gpt4all-j/actions/workflows/tests.yml)
         
@@ -74,14 +74,15 @@
         
         model = Model('/path/to/ggml-gpt4all-j.bin', lib=lib)
         ```
         
         ## License
         
         [MIT](https://github.com/marella/gpt4all-j/blob/main/LICENSE)
+        
         [gptj.cpp]: https://github.com/marella/gptj.cpp
         
 Keywords: gpt4all-j gpt4all gpt-j ai llm cpp
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `gpt4all-j-0.2.0/README.md` & `gpt4all-j-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -66,8 +66,9 @@
 
 model = Model('/path/to/ggml-gpt4all-j.bin', lib=lib)
 ```
 
 ## License
 
 [MIT](https://github.com/marella/gpt4all-j/blob/main/LICENSE)
+
 [gptj.cpp]: https://github.com/marella/gptj.cpp
```

### Comparing `gpt4all-j-0.2.0/gpt4all_j.egg-info/PKG-INFO` & `gpt4all-j-0.2.1/gpt4all_j.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt4all-j
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python bindings for the C++ port of GPT4All-J model.
 Home-page: https://github.com/marella/gpt4all-j
 Author: Ravindra Marella
 Author-email: mv.ravindra007@gmail.com
 License: MIT
 Description: # [GPT4All-J](https://github.com/marella/gpt4all-j) [![tests](https://github.com/marella/gpt4all-j/actions/workflows/tests.yml/badge.svg)](https://github.com/marella/gpt4all-j/actions/workflows/tests.yml)
         
@@ -74,14 +74,15 @@
         
         model = Model('/path/to/ggml-gpt4all-j.bin', lib=lib)
         ```
         
         ## License
         
         [MIT](https://github.com/marella/gpt4all-j/blob/main/LICENSE)
+        
         [gptj.cpp]: https://github.com/marella/gptj.cpp
         
 Keywords: gpt4all-j gpt4all gpt-j ai llm cpp
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `gpt4all-j-0.2.0/gpt4all_j.egg-info/SOURCES.txt` & `gpt4all-j-0.2.1/gpt4all_j.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.0/gpt4allj/lib/avx/ggml.dll` & `gpt4all-j-0.2.1/gpt4allj/lib/avx/ggml.dll`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.0/gpt4allj/lib/avx/gptj.dll` & `gpt4all-j-0.2.1/gpt4allj/lib/avx/gptj.dll`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.0/gpt4allj/lib/avx/libggml.dylib` & `gpt4all-j-0.2.1/gpt4allj/lib/avx/libggml.dylib`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.0/gpt4allj/lib/avx/libggml.so` & `gpt4all-j-0.2.1/gpt4allj/lib/avx/libggml.so`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.0/gpt4allj/lib/avx/libgptj.dylib` & `gpt4all-j-0.2.1/gpt4allj/lib/avx/libgptj.dylib`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.0/gpt4allj/lib/avx/libgptj.so` & `gpt4all-j-0.2.1/gpt4allj/lib/avx/libgptj.so`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.0/gpt4allj/lib/avx2/ggml.dll` & `gpt4all-j-0.2.1/gpt4allj/lib/avx2/ggml.dll`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.0/gpt4allj/lib/avx2/gptj.dll` & `gpt4all-j-0.2.1/gpt4allj/lib/avx2/gptj.dll`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.0/gpt4allj/lib/avx2/libggml.dylib` & `gpt4all-j-0.2.1/gpt4allj/lib/avx2/libggml.dylib`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.0/gpt4allj/lib/avx2/libggml.so` & `gpt4all-j-0.2.1/gpt4allj/lib/avx2/libggml.so`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.0/gpt4allj/lib/avx2/libgptj.dylib` & `gpt4all-j-0.2.1/gpt4allj/lib/avx2/libgptj.dylib`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.0/gpt4allj/lib/avx2/libgptj.so` & `gpt4all-j-0.2.1/gpt4allj/lib/avx2/libgptj.so`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.0/gpt4allj/lib.py` & `gpt4all-j-0.2.1/gpt4allj/lib.py`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.0/gpt4allj/model.py` & `gpt4all-j-0.2.1/gpt4allj/model.py`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.0/setup.py` & `gpt4all-j-0.2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md') as f:
     long_description = f.read()
 
 name = 'gpt4all-j'
 
 setup(
     name=name,
-    version='0.2.0',
+    version='0.2.1',
     description='Python bindings for the C++ port of GPT4All-J model.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ravindra Marella',
     author_email='mv.ravindra007@gmail.com',
     url='https://github.com/marella/{}'.format(name),
     license='MIT',
```

