# Comparing `tmp/pwproxy-0.0.8.tar.gz` & `tmp/pwproxy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwproxy-0.0.8.tar", last modified: Sun Apr 23 04:14:03 2023, max compression
+gzip compressed data, was "pwproxy-0.0.9.tar", last modified: Sun Apr 23 04:20:57 2023, max compression
```

## Comparing `pwproxy-0.0.8.tar` & `pwproxy-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 04:14:03.211185 pwproxy-0.0.8/
--rw-rw-rw-   0        0        0    11558 2023-04-23 04:11:21.000000 pwproxy-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1218 2023-04-23 04:14:03.210181 pwproxy-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      970 2023-04-23 04:11:21.000000 pwproxy-0.0.8/README.md
--rw-rw-rw-   0        0        0      641 2023-04-23 04:12:14.000000 pwproxy-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-23 04:14:03.211185 pwproxy-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-23 04:14:03.200188 pwproxy-0.0.8/src/
--rw-rw-rw-   0        0        0        0 2023-04-23 04:11:21.000000 pwproxy-0.0.8/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 04:14:03.202185 pwproxy-0.0.8/src/pwproxy/
--rw-rw-rw-   0        0        0      567 2023-04-23 04:11:21.000000 pwproxy-0.0.8/src/pwproxy/__init__.py
--rw-rw-rw-   0        0        0     1028 2023-04-23 04:11:21.000000 pwproxy-0.0.8/src/pwproxy/function.py
--rw-rw-rw-   0        0        0     2184 2023-04-23 04:11:21.000000 pwproxy-0.0.8/src/pwproxy/run.py
-drwxrwxrwx   0        0        0        0 2023-04-23 04:14:03.205183 pwproxy-0.0.8/src/pwproxy.egg-info/
--rw-rw-rw-   0        0        0     1218 2023-04-23 04:14:02.000000 pwproxy-0.0.8/src/pwproxy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2023-04-23 04:14:03.000000 pwproxy-0.0.8/src/pwproxy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 04:14:02.000000 pwproxy-0.0.8/src/pwproxy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-23 04:14:02.000000 pwproxy-0.0.8/src/pwproxy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-23 04:14:02.000000 pwproxy-0.0.8/src/pwproxy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-23 04:14:03.209181 pwproxy-0.0.8/test/
--rw-rw-rw-   0        0        0      366 2023-04-23 04:11:21.000000 pwproxy-0.0.8/test/test_1.py
--rw-rw-rw-   0        0        0      637 2023-04-23 04:11:21.000000 pwproxy-0.0.8/test/test_2.py
--rw-rw-rw-   0        0        0      342 2023-04-23 04:11:21.000000 pwproxy-0.0.8/test/test_3.py
--rw-rw-rw-   0        0        0      351 2023-04-23 04:11:21.000000 pwproxy-0.0.8/test/test_4.py
--rw-rw-rw-   0        0        0      466 2023-04-23 04:11:21.000000 pwproxy-0.0.8/test/test_5.py
+drwxrwxrwx   0        0        0        0 2023-04-23 04:20:57.285225 pwproxy-0.0.9/
+-rw-rw-rw-   0        0        0    11558 2023-04-23 04:11:21.000000 pwproxy-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1254 2023-04-23 04:20:57.285225 pwproxy-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      947 2023-04-23 04:20:17.000000 pwproxy-0.0.9/README.md
+-rw-rw-rw-   0        0        0      714 2023-04-23 04:20:30.000000 pwproxy-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-23 04:20:57.285225 pwproxy-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-23 04:20:57.274227 pwproxy-0.0.9/src/
+-rw-rw-rw-   0        0        0        0 2023-04-23 04:11:21.000000 pwproxy-0.0.9/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 04:20:57.276229 pwproxy-0.0.9/src/pwproxy/
+-rw-rw-rw-   0        0        0      567 2023-04-23 04:11:21.000000 pwproxy-0.0.9/src/pwproxy/__init__.py
+-rw-rw-rw-   0        0        0     1028 2023-04-23 04:11:21.000000 pwproxy-0.0.9/src/pwproxy/function.py
+-rw-rw-rw-   0        0        0     2184 2023-04-23 04:11:21.000000 pwproxy-0.0.9/src/pwproxy/run.py
+drwxrwxrwx   0        0        0        0 2023-04-23 04:20:57.280225 pwproxy-0.0.9/src/pwproxy.egg-info/
+-rw-rw-rw-   0        0        0     1254 2023-04-23 04:20:56.000000 pwproxy-0.0.9/src/pwproxy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-04-23 04:20:57.000000 pwproxy-0.0.9/src/pwproxy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 04:20:56.000000 pwproxy-0.0.9/src/pwproxy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-23 04:20:56.000000 pwproxy-0.0.9/src/pwproxy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-23 04:20:56.000000 pwproxy-0.0.9/src/pwproxy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 04:20:57.284226 pwproxy-0.0.9/test/
+-rw-rw-rw-   0        0        0      366 2023-04-23 04:11:21.000000 pwproxy-0.0.9/test/test_1.py
+-rw-rw-rw-   0        0        0      637 2023-04-23 04:11:21.000000 pwproxy-0.0.9/test/test_2.py
+-rw-rw-rw-   0        0        0      342 2023-04-23 04:11:21.000000 pwproxy-0.0.9/test/test_3.py
+-rw-rw-rw-   0        0        0      351 2023-04-23 04:11:21.000000 pwproxy-0.0.9/test/test_4.py
+-rw-rw-rw-   0        0        0      466 2023-04-23 04:11:21.000000 pwproxy-0.0.9/test/test_5.py
```

### Comparing `pwproxy-0.0.8/LICENSE` & `pwproxy-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pwproxy-0.0.8/PKG-INFO` & `pwproxy-0.0.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: pwproxy
-Version: 0.0.8
+Version: 0.0.9
 Author-email: gc <895091550@qq.com>
+Project-URL: Homepage, https://github.com/gcil125/pwproxy
 Keywords: playwright,mitmproxy,intercept request,modify response
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pwproxy
 
@@ -16,15 +17,15 @@
 优点
 
 1. 基于playwright，直接调用本地浏览器，不用以设置代理的方式启动浏览器, mitmproxy必须以冷启动设置代理的方法启动本地浏览器才能实现拦截
 2. 不需要考虑安全证书的问题
 
 # 安装
 
-`pip install pwproxy-X.X.X-py3-none-any.whl`
+`pip install pwproxy`
 
 # 使用
 
 <hr>
 目录结构:<br>
 
 ```python
```

### Comparing `pwproxy-0.0.8/README.md` & `pwproxy-0.0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 优点
 
 1. 基于playwright，直接调用本地浏览器，不用以设置代理的方式启动浏览器, mitmproxy必须以冷启动设置代理的方法启动本地浏览器才能实现拦截
 2. 不需要考虑安全证书的问题
 
 # 安装
 
-`pip install pwproxy-X.X.X-py3-none-any.whl`
+`pip install pwproxy`
 
 # 使用
 
 <hr>
 目录结构:<br>
 
 ```python
```

### Comparing `pwproxy-0.0.8/src/pwproxy/__init__.py` & `pwproxy-0.0.9/src/pwproxy/__init__.py`

 * *Files identical despite different names*

### Comparing `pwproxy-0.0.8/src/pwproxy/function.py` & `pwproxy-0.0.9/src/pwproxy/function.py`

 * *Files identical despite different names*

### Comparing `pwproxy-0.0.8/src/pwproxy/run.py` & `pwproxy-0.0.9/src/pwproxy/run.py`

 * *Files identical despite different names*

### Comparing `pwproxy-0.0.8/src/pwproxy.egg-info/PKG-INFO` & `pwproxy-0.0.9/src/pwproxy.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: pwproxy
-Version: 0.0.8
+Version: 0.0.9
 Author-email: gc <895091550@qq.com>
+Project-URL: Homepage, https://github.com/gcil125/pwproxy
 Keywords: playwright,mitmproxy,intercept request,modify response
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pwproxy
 
@@ -16,15 +17,15 @@
 优点
 
 1. 基于playwright，直接调用本地浏览器，不用以设置代理的方式启动浏览器, mitmproxy必须以冷启动设置代理的方法启动本地浏览器才能实现拦截
 2. 不需要考虑安全证书的问题
 
 # 安装
 
-`pip install pwproxy-X.X.X-py3-none-any.whl`
+`pip install pwproxy`
 
 # 使用
 
 <hr>
 目录结构:<br>
 
 ```python
```

### Comparing `pwproxy-0.0.8/test/test_2.py` & `pwproxy-0.0.9/test/test_2.py`

 * *Files identical despite different names*

