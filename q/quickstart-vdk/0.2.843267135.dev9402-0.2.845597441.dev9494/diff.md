# Comparing `tmp/quickstart-vdk-0.2.843267135.dev9402.tar.gz` & `tmp/quickstart-vdk-0.2.845597441.dev9494.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstart-vdk-0.2.843267135.dev9402.tar", last modified: Thu Apr 20 10:59:07 2023, max compression
+gzip compressed data, was "quickstart-vdk-0.2.845597441.dev9494.tar", last modified: Sun Apr 23 04:20:13 2023, max compression
```

## Comparing `quickstart-vdk-0.2.843267135.dev9402.tar` & `quickstart-vdk-0.2.845597441.dev9494.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:59:07.804111 quickstart-vdk-0.2.843267135.dev9402/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-04-20 10:59:07.804111 quickstart-vdk-0.2.843267135.dev9402/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-04-20 10:58:54.000000 quickstart-vdk-0.2.843267135.dev9402/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:59:07.804111 quickstart-vdk-0.2.843267135.dev9402/quickstart_vdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-04-20 10:59:07.000000 quickstart-vdk-0.2.843267135.dev9402/quickstart_vdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2023-04-20 10:59:07.000000 quickstart-vdk-0.2.843267135.dev9402/quickstart_vdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 10:59:07.000000 quickstart-vdk-0.2.843267135.dev9402/quickstart_vdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-04-20 10:59:07.000000 quickstart-vdk-0.2.843267135.dev9402/quickstart_vdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-20 10:59:07.000000 quickstart-vdk-0.2.843267135.dev9402/quickstart_vdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 10:59:07.804111 quickstart-vdk-0.2.843267135.dev9402/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1299 2023-04-20 10:58:58.000000 quickstart-vdk-0.2.843267135.dev9402/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:59:07.804111 quickstart-vdk-0.2.843267135.dev9402/tests/
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-04-20 10:58:54.000000 quickstart-vdk-0.2.843267135.dev9402/tests/test_dummy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 04:20:13.866061 quickstart-vdk-0.2.845597441.dev9494/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-04-23 04:20:13.866061 quickstart-vdk-0.2.845597441.dev9494/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-04-23 04:17:29.000000 quickstart-vdk-0.2.845597441.dev9494/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 04:20:13.866061 quickstart-vdk-0.2.845597441.dev9494/quickstart_vdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-04-23 04:20:13.000000 quickstart-vdk-0.2.845597441.dev9494/quickstart_vdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2023-04-23 04:20:13.000000 quickstart-vdk-0.2.845597441.dev9494/quickstart_vdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 04:20:13.000000 quickstart-vdk-0.2.845597441.dev9494/quickstart_vdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-04-23 04:20:13.000000 quickstart-vdk-0.2.845597441.dev9494/quickstart_vdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-23 04:20:13.000000 quickstart-vdk-0.2.845597441.dev9494/quickstart_vdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 04:20:13.866061 quickstart-vdk-0.2.845597441.dev9494/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2023-04-23 04:20:02.000000 quickstart-vdk-0.2.845597441.dev9494/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 04:20:13.866061 quickstart-vdk-0.2.845597441.dev9494/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-04-23 04:17:29.000000 quickstart-vdk-0.2.845597441.dev9494/tests/test_dummy.py
```

### Comparing `quickstart-vdk-0.2.843267135.dev9402/PKG-INFO` & `quickstart-vdk-0.2.845597441.dev9494/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.843267135.dev9402
+Version: 0.2.845597441.dev9494
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.843267135.dev9402/quickstart_vdk.egg-info/PKG-INFO` & `quickstart-vdk-0.2.845597441.dev9494/quickstart_vdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.843267135.dev9402
+Version: 0.2.845597441.dev9494
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.843267135.dev9402/setup.py` & `quickstart-vdk-0.2.845597441.dev9494/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.2.843267135.dev9402"
+__version__ = "0.2.845597441.dev9494"
 
 setuptools.setup(
     name="quickstart-vdk",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.",
     long_description=pathlib.Path("README.md").read_text(),
```

