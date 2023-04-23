# Comparing `tmp/common-xmjz-0.1.1.tar.gz` & `tmp/common-xmjz-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\common-xmjz-0.1.1.tar", last modified: Sun Apr 23 10:48:28 2023, max compression
+gzip compressed data, was "dist\common-xmjz-0.1.2.tar", last modified: Sun Apr 23 10:58:12 2023, max compression
```

## Comparing `common-xmjz-0.1.1.tar` & `common-xmjz-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 10:48:28.177017 common-xmjz-0.1.1/
--rw-rw-rw-   0        0        0      634 2023-04-23 10:48:28.177017 common-xmjz-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-23 10:48:28.176018 common-xmjz-0.1.1/common_xmjz.egg-info/
--rw-rw-rw-   0        0        0      634 2023-04-23 10:48:28.000000 common-xmjz-0.1.1/common_xmjz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      165 2023-04-23 10:48:28.000000 common-xmjz-0.1.1/common_xmjz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 10:48:28.000000 common-xmjz-0.1.1/common_xmjz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-23 10:48:28.000000 common-xmjz-0.1.1/common_xmjz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 10:48:28.177017 common-xmjz-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     3879 2023-04-23 10:48:23.000000 common-xmjz-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-23 10:48:28.176018 common-xmjz-0.1.1/xmjz/
--rw-rw-rw-   0        0        0        0 2023-04-23 10:43:32.000000 common-xmjz-0.1.1/xmjz/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:58:12.372532 common-xmjz-0.1.2/
+-rw-rw-rw-   0        0        0      634 2023-04-23 10:58:12.372532 common-xmjz-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-23 10:58:12.371533 common-xmjz-0.1.2/common_xmjz.egg-info/
+-rw-rw-rw-   0        0        0      634 2023-04-23 10:58:12.000000 common-xmjz-0.1.2/common_xmjz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2023-04-23 10:58:12.000000 common-xmjz-0.1.2/common_xmjz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 10:58:12.000000 common-xmjz-0.1.2/common_xmjz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-23 10:58:12.000000 common-xmjz-0.1.2/common_xmjz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 10:58:12.372532 common-xmjz-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     3879 2023-04-23 10:54:42.000000 common-xmjz-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:58:12.371533 common-xmjz-0.1.2/xmjz/
+-rw-rw-rw-   0        0        0        0 2023-04-23 10:43:32.000000 common-xmjz-0.1.2/xmjz/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:58:12.371533 common-xmjz-0.1.2/xmjz/common/
+-rw-rw-rw-   0        0        0        0 2023-04-23 10:43:32.000000 common-xmjz-0.1.2/xmjz/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:58:12.372532 common-xmjz-0.1.2/xmjz/common/mysql/
+-rw-rw-rw-   0        0        0        0 2023-04-23 10:07:49.000000 common-xmjz-0.1.2/xmjz/common/mysql/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 10:58:12.372532 common-xmjz-0.1.2/xmjz/common/mysql/helper/
+-rw-rw-rw-   0        0        0     1946 2023-04-23 10:57:08.000000 common-xmjz-0.1.2/xmjz/common/mysql/helper/__init__.py
```

### Comparing `common-xmjz-0.1.1/PKG-INFO` & `common-xmjz-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-xmjz
-Version: 0.1.1
+Version: 0.1.2
 Summary: common-xmjz
 Home-page: https://github.com/me/myproject
 Author: xmjz
 Author-email: xxx@example.com
 License: MIT
 Description: common-xmjz
 Platform: UNKNOWN
```

### Comparing `common-xmjz-0.1.1/common_xmjz.egg-info/PKG-INFO` & `common-xmjz-0.1.2/common_xmjz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-xmjz
-Version: 0.1.1
+Version: 0.1.2
 Summary: common-xmjz
 Home-page: https://github.com/me/myproject
 Author: xmjz
 Author-email: xxx@example.com
 License: MIT
 Description: common-xmjz
 Platform: UNKNOWN
```

### Comparing `common-xmjz-0.1.1/setup.py` & `common-xmjz-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'common-xmjz'
 DESCRIPTION = 'common-xmjz'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'xxx@example.com'
 AUTHOR = 'xmjz'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

