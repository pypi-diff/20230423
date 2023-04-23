# Comparing `tmp/cnki_html2json-0.1.1.tar.gz` & `tmp/cnki_html2json-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnki_html2json-0.1.1.tar", last modified: Sat Apr 22 17:29:22 2023, max compression
+gzip compressed data, was "cnki_html2json-0.1.2.tar", last modified: Sun Apr 23 02:06:27 2023, max compression
```

## Comparing `cnki_html2json-0.1.1.tar` & `cnki_html2json-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:29:22.477869 cnki_html2json-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-22 17:29:11.000000 cnki_html2json-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-04-22 17:29:22.477869 cnki_html2json-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-04-22 17:29:11.000000 cnki_html2json-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:29:22.473869 cnki_html2json-0.1.1/cnki_html2json/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-22 17:29:11.000000 cnki_html2json-0.1.1/cnki_html2json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-22 17:29:11.000000 cnki_html2json-0.1.1/cnki_html2json/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-04-22 17:29:11.000000 cnki_html2json-0.1.1/cnki_html2json/crawl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-04-22 17:29:11.000000 cnki_html2json-0.1.1/cnki_html2json/html2json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-22 17:29:11.000000 cnki_html2json-0.1.1/cnki_html2json/parse_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-22 17:29:11.000000 cnki_html2json-0.1.1/cnki_html2json/recognize_slider_coordinate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:29:22.473869 cnki_html2json-0.1.1/cnki_html2json.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-04-22 17:29:22.000000 cnki_html2json-0.1.1/cnki_html2json.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-22 17:29:22.000000 cnki_html2json-0.1.1/cnki_html2json.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 17:29:22.000000 cnki_html2json-0.1.1/cnki_html2json.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-22 17:29:22.000000 cnki_html2json-0.1.1/cnki_html2json.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-22 17:29:22.000000 cnki_html2json-0.1.1/cnki_html2json.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-22 17:29:22.000000 cnki_html2json-0.1.1/cnki_html2json.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 17:29:22.477869 cnki_html2json-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-22 17:29:11.000000 cnki_html2json-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:29:22.477869 cnki_html2json-0.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-22 17:29:11.000000 cnki_html2json-0.1.1/test/test_html2json.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-22 17:29:11.000000 cnki_html2json-0.1.1/test/test_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:06:27.490551 cnki_html2json-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-23 02:06:16.000000 cnki_html2json-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-04-23 02:06:27.490551 cnki_html2json-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-04-23 02:06:16.000000 cnki_html2json-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:06:27.490551 cnki_html2json-0.1.2/cnki_html2json/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-23 02:06:16.000000 cnki_html2json-0.1.2/cnki_html2json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-23 02:06:16.000000 cnki_html2json-0.1.2/cnki_html2json/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-04-23 02:06:16.000000 cnki_html2json-0.1.2/cnki_html2json/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-04-23 02:06:16.000000 cnki_html2json-0.1.2/cnki_html2json/html2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-23 02:06:16.000000 cnki_html2json-0.1.2/cnki_html2json/parse_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-23 02:06:16.000000 cnki_html2json-0.1.2/cnki_html2json/recognize_slider_coordinate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:06:27.490551 cnki_html2json-0.1.2/cnki_html2json.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-04-23 02:06:27.000000 cnki_html2json-0.1.2/cnki_html2json.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-23 02:06:27.000000 cnki_html2json-0.1.2/cnki_html2json.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 02:06:27.000000 cnki_html2json-0.1.2/cnki_html2json.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-23 02:06:27.000000 cnki_html2json-0.1.2/cnki_html2json.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-23 02:06:27.000000 cnki_html2json-0.1.2/cnki_html2json.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-23 02:06:27.000000 cnki_html2json-0.1.2/cnki_html2json.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 02:06:27.490551 cnki_html2json-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-23 02:06:16.000000 cnki_html2json-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:06:27.490551 cnki_html2json-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-23 02:06:16.000000 cnki_html2json-0.1.2/tests/test_html2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-23 02:06:16.000000 cnki_html2json-0.1.2/tests/test_metadata.py
```

### Comparing `cnki_html2json-0.1.1/LICENSE` & `cnki_html2json-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.1/PKG-INFO` & `cnki_html2json-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: cnki_html2json
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package to convert cnki html to json
 Home-page: https://github.com/doublessay/cnki-html2json
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: cnki,text-structure,crawler
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 从知网HTML格式的文献中提取结构化文本
 
 本仓库是一个从知网CNKI的HTML格式的 <b>期刊论文</b> 中提取结构化文本，然后导出 <b>JSON</b> 文件的工具，方便对中文期刊论文进行更细维度的分析。
```

### Comparing `cnki_html2json-0.1.1/README.md` & `cnki_html2json-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.1/cnki_html2json/cli.py` & `cnki_html2json-0.1.2/cnki_html2json/cli.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.1/cnki_html2json/crawl.py` & `cnki_html2json-0.1.2/cnki_html2json/crawl.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.1/cnki_html2json/html2json.py` & `cnki_html2json-0.1.2/cnki_html2json/html2json.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.1/cnki_html2json/parse_metadata.py` & `cnki_html2json-0.1.2/cnki_html2json/parse_metadata.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.1/cnki_html2json/recognize_slider_coordinate.py` & `cnki_html2json-0.1.2/cnki_html2json/recognize_slider_coordinate.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.1/cnki_html2json.egg-info/PKG-INFO` & `cnki_html2json-0.1.2/cnki_html2json.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: cnki-html2json
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package to convert cnki html to json
 Home-page: https://github.com/doublessay/cnki-html2json
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: cnki,text-structure,crawler
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 从知网HTML格式的文献中提取结构化文本
 
 本仓库是一个从知网CNKI的HTML格式的 <b>期刊论文</b> 中提取结构化文本，然后导出 <b>JSON</b> 文件的工具，方便对中文期刊论文进行更细维度的分析。
```

### Comparing `cnki_html2json-0.1.1/setup.py` & `cnki_html2json-0.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,40 @@
-from setuptools import setup,find_packages
+from setuptools import setup
 
 setup(
     name="cnki_html2json",
     author = "WangK2",
     author_email = "kw221225@gmail.com",
-    version="0.1.1",
+    version="0.1.2",
     description="A package to convert cnki html to json",
     long_description = open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords = ["cnki","text-structure","crawler"],
     license="MIT",
     url="https://github.com/doublessay/cnki-html2json",
-    packages=find_packages(exclude=['test']),
-    exclude_package_data={'':['test/*']},
+    packages=["cnki_html2json"],
     python_requires=">=3.8.0",
     install_requires=[
         "selenium",
         "lxml",
         "opencv-python",
         "numpy",
         "loguru"],
     
     classifiers=[
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     entry_points={
         "console_scripts": [
             "cnki-crawler = cnki_html2json.cli:main",
         ]
     },
```

### Comparing `cnki_html2json-0.1.1/test/test_html2json.py` & `cnki_html2json-0.1.2/tests/test_html2json.py`

 * *Files identical despite different names*

