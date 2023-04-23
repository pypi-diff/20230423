# Comparing `tmp/codewithgpu-test-0.1.0.tar.gz` & `tmp/codewithgpu-test-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codewithgpu-test-0.1.0.tar", last modified: Sun Apr 23 07:19:00 2023, max compression
+gzip compressed data, was "codewithgpu-test-0.1.1.tar", last modified: Sun Apr 23 07:24:11 2023, max compression
```

## Comparing `codewithgpu-test-0.1.0.tar` & `codewithgpu-test-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 daiab     (1000) daiab     (1000)        0 2023-04-23 07:19:00.575249 codewithgpu-test-0.1.0/
--rw-r--r--   0 daiab     (1000) daiab     (1000)     3379 2023-04-23 07:19:00.575249 codewithgpu-test-0.1.0/PKG-INFO
--rw-r--r--   0 daiab     (1000) daiab     (1000)     2142 2023-04-21 09:27:22.000000 codewithgpu-test-0.1.0/README.md
-drwxr-xr-x   0 daiab     (1000) daiab     (1000)        0 2023-04-23 07:19:00.575249 codewithgpu-test-0.1.0/codewithgpu/
--rw-r--r--   0 daiab     (1000) daiab     (1000)     1046 2023-04-23 04:43:49.000000 codewithgpu-test-0.1.0/codewithgpu/__init__.py
-drwxr-xr-x   0 daiab     (1000) daiab     (1000)        0 2023-04-23 07:19:00.575249 codewithgpu-test-0.1.0/codewithgpu/model/
--rw-r--r--   0 daiab     (1000) daiab     (1000)      761 2023-04-23 05:19:24.000000 codewithgpu-test-0.1.0/codewithgpu/model/__init__.py
--rw-r--r--   0 daiab     (1000) daiab     (1000)     2403 2023-04-23 05:21:18.000000 codewithgpu-test-0.1.0/codewithgpu/model/download.py
-drwxr-xr-x   0 daiab     (1000) daiab     (1000)        0 2023-04-23 07:19:00.575249 codewithgpu-test-0.1.0/codewithgpu/utils/
--rw-r--r--   0 daiab     (1000) daiab     (1000)      746 2023-04-21 09:27:22.000000 codewithgpu-test-0.1.0/codewithgpu/utils/__init__.py
--rw-r--r--   0 daiab     (1000) daiab     (1000)     3193 2023-04-23 07:14:57.000000 codewithgpu-test-0.1.0/codewithgpu/utils/cg_cli.py
--rw-r--r--   0 daiab     (1000) daiab     (1000)     3741 2023-04-21 09:27:22.000000 codewithgpu-test-0.1.0/codewithgpu/utils/logging.py
--rw-r--r--   0 daiab     (1000) daiab     (1000)     1226 2023-04-21 09:27:22.000000 codewithgpu-test-0.1.0/codewithgpu/utils/unittest_util.py
-drwxr-xr-x   0 daiab     (1000) daiab     (1000)        0 2023-04-23 07:19:00.575249 codewithgpu-test-0.1.0/codewithgpu_test.egg-info/
--rw-r--r--   0 daiab     (1000) daiab     (1000)     3379 2023-04-23 07:19:00.000000 codewithgpu-test-0.1.0/codewithgpu_test.egg-info/PKG-INFO
--rw-r--r--   0 daiab     (1000) daiab     (1000)      466 2023-04-23 07:19:00.000000 codewithgpu-test-0.1.0/codewithgpu_test.egg-info/SOURCES.txt
--rw-r--r--   0 daiab     (1000) daiab     (1000)        1 2023-04-23 07:19:00.000000 codewithgpu-test-0.1.0/codewithgpu_test.egg-info/dependency_links.txt
--rw-r--r--   0 daiab     (1000) daiab     (1000)       64 2023-04-23 07:19:00.000000 codewithgpu-test-0.1.0/codewithgpu_test.egg-info/entry_points.txt
--rw-r--r--   0 daiab     (1000) daiab     (1000)       58 2023-04-23 07:19:00.000000 codewithgpu-test-0.1.0/codewithgpu_test.egg-info/requires.txt
--rw-r--r--   0 daiab     (1000) daiab     (1000)       48 2023-04-23 07:19:00.000000 codewithgpu-test-0.1.0/codewithgpu_test.egg-info/top_level.txt
--rw-r--r--   0 daiab     (1000) daiab     (1000)       38 2023-04-23 07:19:00.575249 codewithgpu-test-0.1.0/setup.cfg
--rw-r--r--   0 daiab     (1000) daiab     (1000)     5534 2023-04-23 04:44:59.000000 codewithgpu-test-0.1.0/setup.py
+drwxr-xr-x   0 daiab     (1000) daiab     (1000)        0 2023-04-23 07:24:11.965248 codewithgpu-test-0.1.1/
+-rw-r--r--   0 daiab     (1000) daiab     (1000)     3379 2023-04-23 07:24:11.965248 codewithgpu-test-0.1.1/PKG-INFO
+-rw-r--r--   0 daiab     (1000) daiab     (1000)     2142 2023-04-21 09:27:22.000000 codewithgpu-test-0.1.1/README.md
+drwxr-xr-x   0 daiab     (1000) daiab     (1000)        0 2023-04-23 07:24:11.965248 codewithgpu-test-0.1.1/codewithgpu/
+-rw-r--r--   0 daiab     (1000) daiab     (1000)     1046 2023-04-23 07:24:00.000000 codewithgpu-test-0.1.1/codewithgpu/__init__.py
+drwxr-xr-x   0 daiab     (1000) daiab     (1000)        0 2023-04-23 07:24:11.965248 codewithgpu-test-0.1.1/codewithgpu/model/
+-rw-r--r--   0 daiab     (1000) daiab     (1000)      761 2023-04-23 05:19:24.000000 codewithgpu-test-0.1.1/codewithgpu/model/__init__.py
+-rw-r--r--   0 daiab     (1000) daiab     (1000)     2403 2023-04-23 05:21:18.000000 codewithgpu-test-0.1.1/codewithgpu/model/download.py
+drwxr-xr-x   0 daiab     (1000) daiab     (1000)        0 2023-04-23 07:24:11.965248 codewithgpu-test-0.1.1/codewithgpu/utils/
+-rw-r--r--   0 daiab     (1000) daiab     (1000)      746 2023-04-21 09:27:22.000000 codewithgpu-test-0.1.1/codewithgpu/utils/__init__.py
+-rw-r--r--   0 daiab     (1000) daiab     (1000)     3193 2023-04-23 07:14:57.000000 codewithgpu-test-0.1.1/codewithgpu/utils/cg_cli.py
+-rw-r--r--   0 daiab     (1000) daiab     (1000)     3741 2023-04-21 09:27:22.000000 codewithgpu-test-0.1.1/codewithgpu/utils/logging.py
+-rw-r--r--   0 daiab     (1000) daiab     (1000)     1226 2023-04-21 09:27:22.000000 codewithgpu-test-0.1.1/codewithgpu/utils/unittest_util.py
+drwxr-xr-x   0 daiab     (1000) daiab     (1000)        0 2023-04-23 07:24:11.965248 codewithgpu-test-0.1.1/codewithgpu_test.egg-info/
+-rw-r--r--   0 daiab     (1000) daiab     (1000)     3379 2023-04-23 07:24:11.000000 codewithgpu-test-0.1.1/codewithgpu_test.egg-info/PKG-INFO
+-rw-r--r--   0 daiab     (1000) daiab     (1000)      427 2023-04-23 07:24:11.000000 codewithgpu-test-0.1.1/codewithgpu_test.egg-info/SOURCES.txt
+-rw-r--r--   0 daiab     (1000) daiab     (1000)        1 2023-04-23 07:24:11.000000 codewithgpu-test-0.1.1/codewithgpu_test.egg-info/dependency_links.txt
+-rw-r--r--   0 daiab     (1000) daiab     (1000)       64 2023-04-23 07:24:11.000000 codewithgpu-test-0.1.1/codewithgpu_test.egg-info/entry_points.txt
+-rw-r--r--   0 daiab     (1000) daiab     (1000)       48 2023-04-23 07:24:11.000000 codewithgpu-test-0.1.1/codewithgpu_test.egg-info/top_level.txt
+-rw-r--r--   0 daiab     (1000) daiab     (1000)       38 2023-04-23 07:24:11.965248 codewithgpu-test-0.1.1/setup.cfg
+-rw-r--r--   0 daiab     (1000) daiab     (1000)     5375 2023-04-23 07:22:10.000000 codewithgpu-test-0.1.1/setup.py
```

### Comparing `codewithgpu-test-0.1.0/PKG-INFO` & `codewithgpu-test-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codewithgpu-test
-Version: 0.1.0
+Version: 0.1.1
 Summary: CodeWithGPU Python Client
 Home-page: https://github.com/seetacloud/codewithgpu
 Author: SeetaCloud
 License: Apache License
 Description: # CodeWithGPU
         
         <p align="center">
```

### Comparing `codewithgpu-test-0.1.0/README.md` & `codewithgpu-test-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `codewithgpu-test-0.1.0/codewithgpu/__init__.py` & `codewithgpu-test-0.1.1/codewithgpu/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,11 +17,11 @@
 
 from __future__ import absolute_import as _absolute_import
 from __future__ import division as _division
 from __future__ import print_function as _print_function
 
 
 # Version
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 # Attributes
 __all__ = [_s for _s in dir() if not _s.startswith('_')]
```

### Comparing `codewithgpu-test-0.1.0/codewithgpu/model/__init__.py` & `codewithgpu-test-0.1.1/codewithgpu/model/__init__.py`

 * *Files identical despite different names*

### Comparing `codewithgpu-test-0.1.0/codewithgpu/model/download.py` & `codewithgpu-test-0.1.1/codewithgpu/model/download.py`

 * *Files identical despite different names*

### Comparing `codewithgpu-test-0.1.0/codewithgpu/utils/__init__.py` & `codewithgpu-test-0.1.1/codewithgpu/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `codewithgpu-test-0.1.0/codewithgpu/utils/cg_cli.py` & `codewithgpu-test-0.1.1/codewithgpu/utils/cg_cli.py`

 * *Files identical despite different names*

### Comparing `codewithgpu-test-0.1.0/codewithgpu/utils/logging.py` & `codewithgpu-test-0.1.1/codewithgpu/utils/logging.py`

 * *Files identical despite different names*

### Comparing `codewithgpu-test-0.1.0/codewithgpu/utils/unittest_util.py` & `codewithgpu-test-0.1.1/codewithgpu/utils/unittest_util.py`

 * *Files identical despite different names*

### Comparing `codewithgpu-test-0.1.0/codewithgpu_test.egg-info/PKG-INFO` & `codewithgpu-test-0.1.1/codewithgpu_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codewithgpu-test
-Version: 0.1.0
+Version: 0.1.1
 Summary: CodeWithGPU Python Client
 Home-page: https://github.com/seetacloud/codewithgpu
 Author: SeetaCloud
 License: Apache License
 Description: # CodeWithGPU
         
         <p align="center">
```

### Comparing `codewithgpu-test-0.1.0/setup.py` & `codewithgpu-test-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,19 +121,15 @@
     long_description=args.long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/seetacloud/codewithgpu',
     author='SeetaCloud',
     license='Apache License',
     packages=find_packages('codewithgpu'),
     cmdclass={'build_py': BuildPyCommand, 'install': InstallCommand},
-    install_requires=['numpy',
-                      'protobuf>=3.9.1,<=3.20.1',
-                      'opencv-python',
-                      'flask',
-                      'gradio'],
+    install_requires=[],
     entry_points={
           "console_scripts": [
               "cg = codewithgpu.model.download:download_cli",
           ],
       },
     classifiers=['Development Status :: 5 - Production/Stable',
                  'Intended Audience :: Developers',
```

