# Comparing `tmp/histcite-python-0.1.1.tar.gz` & `tmp/histcite-python-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "histcite-python-0.1.1.tar", last modified: Sat Apr 22 17:01:09 2023, max compression
+gzip compressed data, was "histcite-python-0.1.2.tar", last modified: Sun Apr 23 01:47:24 2023, max compression
```

## Comparing `histcite-python-0.1.1.tar` & `histcite-python-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:01:09.871692 histcite-python-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-22 17:00:55.000000 histcite-python-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-04-22 17:01:09.871692 histcite-python-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-04-22 17:00:55.000000 histcite-python-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:01:09.867692 histcite-python-0.1.1/histcite/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-22 17:00:55.000000 histcite-python-0.1.1/histcite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-22 17:00:55.000000 histcite-python-0.1.1/histcite/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-22 17:00:55.000000 histcite-python-0.1.1/histcite/compute_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-04-22 17:00:55.000000 histcite-python-0.1.1/histcite/network_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-22 17:00:55.000000 histcite-python-0.1.1/histcite/parse_citation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-04-22 17:00:55.000000 histcite-python-0.1.1/histcite/process_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:01:09.871692 histcite-python-0.1.1/histcite_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-04-22 17:01:09.000000 histcite-python-0.1.1/histcite_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-22 17:01:09.000000 histcite-python-0.1.1/histcite_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 17:01:09.000000 histcite-python-0.1.1/histcite_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-22 17:01:09.000000 histcite-python-0.1.1/histcite_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-22 17:01:09.000000 histcite-python-0.1.1/histcite_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-22 17:01:09.000000 histcite-python-0.1.1/histcite_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 17:01:09.871692 histcite-python-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-22 17:00:55.000000 histcite-python-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:01:09.871692 histcite-python-0.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:00:55.000000 histcite-python-0.1.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-22 17:00:55.000000 histcite-python-0.1.1/test/test_compute_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-22 17:00:55.000000 histcite-python-0.1.1/test/test_network_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-22 17:00:55.000000 histcite-python-0.1.1/test/test_parse_citation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 01:47:24.339620 histcite-python-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-23 01:47:09.000000 histcite-python-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-04-23 01:47:24.339620 histcite-python-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-04-23 01:47:09.000000 histcite-python-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 01:47:24.339620 histcite-python-0.1.2/histcite/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-23 01:47:09.000000 histcite-python-0.1.2/histcite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-23 01:47:09.000000 histcite-python-0.1.2/histcite/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-23 01:47:09.000000 histcite-python-0.1.2/histcite/compute_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-04-23 01:47:09.000000 histcite-python-0.1.2/histcite/network_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-23 01:47:09.000000 histcite-python-0.1.2/histcite/parse_citation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-04-23 01:47:09.000000 histcite-python-0.1.2/histcite/process_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 01:47:24.339620 histcite-python-0.1.2/histcite_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-04-23 01:47:24.000000 histcite-python-0.1.2/histcite_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-23 01:47:24.000000 histcite-python-0.1.2/histcite_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 01:47:24.000000 histcite-python-0.1.2/histcite_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-23 01:47:24.000000 histcite-python-0.1.2/histcite_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-23 01:47:24.000000 histcite-python-0.1.2/histcite_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 01:47:24.000000 histcite-python-0.1.2/histcite_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 01:47:24.339620 histcite-python-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-23 01:47:09.000000 histcite-python-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 01:47:24.339620 histcite-python-0.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-23 01:47:09.000000 histcite-python-0.1.2/test/test_compute_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-23 01:47:09.000000 histcite-python-0.1.2/test/test_network_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-23 01:47:09.000000 histcite-python-0.1.2/test/test_parse_citation.py
```

### Comparing `histcite-python-0.1.1/LICENSE` & `histcite-python-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `histcite-python-0.1.1/PKG-INFO` & `histcite-python-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: histcite-python
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python interface to histcite.
 Home-page: https://github.com/doublessay/histcite-python
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: histcite,web of science,citation network
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
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HistCite工具的Python实现
 
 由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为中科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在较多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/whatsnew/v2.0.0.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` `80%` 的功能，并且可以跨平台使用。
```

### Comparing `histcite-python-0.1.1/README.md` & `histcite-python-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `histcite-python-0.1.1/histcite/cli.py` & `histcite-python-0.1.2/histcite/cli.py`

 * *Files identical despite different names*

### Comparing `histcite-python-0.1.1/histcite/compute_metrics.py` & `histcite-python-0.1.2/histcite/compute_metrics.py`

 * *Files identical despite different names*

### Comparing `histcite-python-0.1.1/histcite/network_graph.py` & `histcite-python-0.1.2/histcite/network_graph.py`

 * *Files identical despite different names*

### Comparing `histcite-python-0.1.1/histcite/parse_citation.py` & `histcite-python-0.1.2/histcite/parse_citation.py`

 * *Files identical despite different names*

### Comparing `histcite-python-0.1.1/histcite/process_table.py` & `histcite-python-0.1.2/histcite/process_table.py`

 * *Files identical despite different names*

### Comparing `histcite-python-0.1.1/histcite_python.egg-info/PKG-INFO` & `histcite-python-0.1.2/histcite_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: histcite-python
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python interface to histcite.
 Home-page: https://github.com/doublessay/histcite-python
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: histcite,web of science,citation network
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
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HistCite工具的Python实现
 
 由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为中科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在较多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/whatsnew/v2.0.0.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` `80%` 的功能，并且可以跨平台使用。
```

### Comparing `histcite-python-0.1.1/test/test_parse_citation.py` & `histcite-python-0.1.2/test/test_parse_citation.py`

 * *Files identical despite different names*

