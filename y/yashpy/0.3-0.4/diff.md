# Comparing `tmp/yashpy-0.3.tar.gz` & `tmp/yashpy-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yashpy-0.3.tar", last modified: Sat Apr 22 15:44:21 2023, max compression
+gzip compressed data, was "yashpy-0.4.tar", last modified: Sat Apr 22 16:42:55 2023, max compression
```

## Comparing `yashpy-0.3.tar` & `yashpy-0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 15:44:21.909423 yashpy-0.3/
--rw-rw-rw-   0        0        0      175 2023-04-22 15:44:21.908335 yashpy-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1091 2023-04-22 07:53:52.000000 yashpy-0.3/licence.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 15:44:21.909423 yashpy-0.3/setup.cfg
--rw-rw-rw-   0        0        0      245 2023-04-22 15:39:10.000000 yashpy-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-22 15:44:21.708001 yashpy-0.3/yashpy/
--rw-rw-rw-   0        0        0      374 2023-04-22 15:39:22.000000 yashpy-0.3/yashpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 15:44:21.903940 yashpy-0.3/yashpy.egg-info/
--rw-rw-rw-   0        0        0      175 2023-04-22 15:44:20.000000 yashpy-0.3/yashpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      159 2023-04-22 15:44:20.000000 yashpy-0.3/yashpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 15:44:20.000000 yashpy-0.3/yashpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-22 15:44:20.000000 yashpy-0.3/yashpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-22 16:42:55.137008 yashpy-0.4/
+-rw-rw-rw-   0        0        0      175 2023-04-22 16:42:55.135056 yashpy-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1091 2023-04-22 07:53:52.000000 yashpy-0.4/licence.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 16:42:55.137984 yashpy-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      245 2023-04-22 16:38:55.000000 yashpy-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 16:42:55.042340 yashpy-0.4/yashpy/
+-rw-rw-rw-   0        0        0     1439 2023-04-22 16:38:19.000000 yashpy-0.4/yashpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 16:42:55.129251 yashpy-0.4/yashpy.egg-info/
+-rw-rw-rw-   0        0        0      175 2023-04-22 16:42:54.000000 yashpy-0.4/yashpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      159 2023-04-22 16:42:54.000000 yashpy-0.4/yashpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 16:42:54.000000 yashpy-0.4/yashpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-22 16:42:54.000000 yashpy-0.4/yashpy.egg-info/top_level.txt
```

### Comparing `yashpy-0.3/licence.txt` & `yashpy-0.4/licence.txt`

 * *Files identical despite different names*

