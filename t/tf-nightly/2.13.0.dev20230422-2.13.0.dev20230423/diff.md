# Comparing `tmp/tf_nightly-2.13.0.dev20230422-cp39-cp39-win_amd64.whl.zip` & `tmp/tf_nightly-2.13.0.dev20230423-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 2060 bytes, number of entries: 4
--rw-rw-r--  2.0 unx     2622 b- defN 23-Apr-22 09:15 tf_nightly-2.13.0.dev20230422.dist-info/METADATA
--rw-rw-r--  2.0 unx       99 b- defN 23-Apr-22 09:15 tf_nightly-2.13.0.dev20230422.dist-info/WHEEL
--rw-rw-r--  2.0 unx        1 b- defN 23-Apr-22 09:15 tf_nightly-2.13.0.dev20230422.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      361 b- defN 23-Apr-22 09:15 tf_nightly-2.13.0.dev20230422.dist-info/RECORD
-4 files, 3083 bytes uncompressed, 1350 bytes compressed:  56.2%
+Zip file size: 2059 bytes, number of entries: 4
+-rw-rw-r--  2.0 unx     2622 b- defN 23-Apr-23 09:16 tf_nightly-2.13.0.dev20230423.dist-info/METADATA
+-rw-rw-r--  2.0 unx       99 b- defN 23-Apr-23 09:16 tf_nightly-2.13.0.dev20230423.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        1 b- defN 23-Apr-23 09:16 tf_nightly-2.13.0.dev20230423.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      361 b- defN 23-Apr-23 09:16 tf_nightly-2.13.0.dev20230423.dist-info/RECORD
+4 files, 3083 bytes uncompressed, 1349 bytes compressed:  56.2%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: tf_nightly-2.13.0.dev20230422.dist-info/METADATA
+Filename: tf_nightly-2.13.0.dev20230423.dist-info/METADATA
 Comment: 
 
-Filename: tf_nightly-2.13.0.dev20230422.dist-info/WHEEL
+Filename: tf_nightly-2.13.0.dev20230423.dist-info/WHEEL
 Comment: 
 
-Filename: tf_nightly-2.13.0.dev20230422.dist-info/top_level.txt
+Filename: tf_nightly-2.13.0.dev20230423.dist-info/top_level.txt
 Comment: 
 
-Filename: tf_nightly-2.13.0.dev20230422.dist-info/RECORD
+Filename: tf_nightly-2.13.0.dev20230423.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `tf_nightly-2.13.0.dev20230422.dist-info/METADATA` & `tf_nightly-2.13.0.dev20230423.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf-nightly
-Version: 2.13.0.dev20230422
+Version: 2.13.0.dev20230423
 Summary: TensorFlow is an open source machine learning framework for everyone.
 Home-page: https://www.tensorflow.org/
 Author: Google Inc.
 Author-email: packages@tensorflow.org
 License: Apache 2.0
 Download-URL: https://github.com/tensorflow/tensorflow/tags
 Keywords: tensorflow tensor machine learning
@@ -25,17 +25,17 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: tf-nightly-macos (==2.13.0-dev20230422) ; platform_system == "Darwin" and platform_machine == "arm64"
-Requires-Dist: tf-nightly-cpu-aws (==2.13.0-dev20230422) ; platform_system == "Linux" and (platform_machine == "arm64" or platform_machine == "aarch64")
-Requires-Dist: tf-nightly-intel (==2.13.0-dev20230422) ; platform_system == "Windows"
+Requires-Dist: tf-nightly-macos (==2.13.0-dev20230423) ; platform_system == "Darwin" and platform_machine == "arm64"
+Requires-Dist: tf-nightly-cpu-aws (==2.13.0-dev20230423) ; platform_system == "Linux" and (platform_machine == "arm64" or platform_machine == "aarch64")
+Requires-Dist: tf-nightly-intel (==2.13.0-dev20230423) ; platform_system == "Windows"
 
 [![Python](https://img.shields.io/pypi/pyversions/tensorflow.svg?style=plastic)](https://badge.fury.io/py/tensorflow)
 [![PyPI](https://badge.fury.io/py/tensorflow.svg)](https://badge.fury.io/py/tensorflow)
 
 TensorFlow is an open source software library for high performance numerical
 computation. Its flexible architecture allows easy deployment of computation
 across a variety of platforms (CPUs, GPUs, TPUs), and from desktops to clusters
```

