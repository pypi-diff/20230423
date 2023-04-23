# Comparing `tmp/spatialmath-python-1.1.6.tar.gz` & `tmp/spatialmath-python-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatialmath-python-1.1.6.tar", last modified: Sun Apr  2 00:19:09 2023, max compression
+gzip compressed data, was "spatialmath-python-1.1.7.tar", last modified: Sun Apr 23 02:10:40 2023, max compression
```

## Comparing `spatialmath-python-1.1.6.tar` & `spatialmath-python-1.1.7.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-04-02 00:19:09.575842 spatialmath-python-1.1.6/
--rw-r--r--   0 corkep     (503) staff       (20)     1068 2020-05-03 01:56:32.000000 spatialmath-python-1.1.6/LICENSE
--rw-rw----   0 corkep     (503) staff       (20)    15921 2023-04-02 00:19:09.575235 spatialmath-python-1.1.6/PKG-INFO
--rw-r--r--   0 corkep     (503) staff       (20)    14506 2023-03-08 07:55:36.000000 spatialmath-python-1.1.6/README.md
--rw-rw----   0 corkep     (503) staff       (20)     2238 2023-04-02 00:17:42.000000 spatialmath-python-1.1.6/pyproject.toml
--rw-rw----   0 corkep     (503) staff       (20)       38 2023-04-02 00:19:09.575975 spatialmath-python-1.1.6/setup.cfg
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-04-02 00:19:09.500229 spatialmath-python-1.1.6/spatialmath/
--rw-rw----   0 corkep     (503) staff       (20)    10807 2023-02-26 06:08:44.000000 spatialmath-python-1.1.6/spatialmath/DualQuaternion.py
--rw-rw----   0 corkep     (503) staff       (20)     1223 2023-03-06 05:53:49.000000 spatialmath-python-1.1.6/spatialmath/__init__.py
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-04-02 00:19:09.563407 spatialmath-python-1.1.6/spatialmath/base/
--rw-r--r--   0 corkep     (503) staff       (20)     6133 2023-03-15 07:14:42.000000 spatialmath-python-1.1.6/spatialmath/base/__init__.py
--rw-rw----   0 corkep     (503) staff       (20)     4376 2023-02-26 06:08:44.000000 spatialmath-python-1.1.6/spatialmath/base/_types_311.py
--rw-rw----   0 corkep     (503) staff       (20)     3668 2023-02-27 02:47:31.000000 spatialmath-python-1.1.6/spatialmath/base/_types_35.py
--rw-rw----   0 corkep     (503) staff       (20)     4453 2023-02-26 06:08:44.000000 spatialmath-python-1.1.6/spatialmath/base/_types_39.py
--rwxrwx---   0 corkep     (503) staff       (20)    28884 2023-03-21 10:14:47.000000 spatialmath-python-1.1.6/spatialmath/base/animate.py
--rw-r--r--   0 corkep     (503) staff       (20)      600 2021-05-23 01:42:29.000000 spatialmath-python-1.1.6/spatialmath/base/animationbug.py
--rw-r--r--   0 corkep     (503) staff       (20)    21504 2023-03-16 00:24:27.000000 spatialmath-python-1.1.6/spatialmath/base/argcheck.py
--rw-r--r--   0 corkep     (503) staff       (20)    62686 2023-03-27 10:00:18.000000 spatialmath-python-1.1.6/spatialmath/base/graphics.py
--rwxr--r--   0 corkep     (503) staff       (20)     2091 2021-05-23 01:42:29.000000 spatialmath-python-1.1.6/spatialmath/base/m2p.py
--rw-r--r--   0 corkep     (503) staff       (20)    11666 2023-03-06 07:02:14.000000 spatialmath-python-1.1.6/spatialmath/base/numeric.py
--rwxrwx---   0 corkep     (503) staff       (20)    29711 2023-03-28 10:16:43.000000 spatialmath-python-1.1.6/spatialmath/base/quaternions.py
--rw-rw----   0 corkep     (503) staff       (20)     6973 2023-02-27 02:51:57.000000 spatialmath-python-1.1.6/spatialmath/base/symbolic.py
--rw-r--r--   0 corkep     (503) staff       (20)     2526 2023-02-01 09:24:26.000000 spatialmath-python-1.1.6/spatialmath/base/timing.py
--rw-r--r--   0 corkep     (503) staff       (20)    45818 2023-03-28 11:10:08.000000 spatialmath-python-1.1.6/spatialmath/base/transforms2d.py
--rw-rw----   0 corkep     (503) staff       (20)   110878 2023-03-28 22:05:19.000000 spatialmath-python-1.1.6/spatialmath/base/transforms3d.py
--rw-rw----   0 corkep     (503) staff       (20)    24862 2023-03-26 07:02:50.000000 spatialmath-python-1.1.6/spatialmath/base/transformsNd.py
--rw-r--r--   0 corkep     (503) staff       (20)     1700 2023-02-01 09:24:27.000000 spatialmath-python-1.1.6/spatialmath/base/trplot2.py
--rw-rw----   0 corkep     (503) staff       (20)      229 2023-02-26 06:08:44.000000 spatialmath-python-1.1.6/spatialmath/base/types.py
--rw-rw----   0 corkep     (503) staff       (20)    19884 2023-03-26 23:53:23.000000 spatialmath-python-1.1.6/spatialmath/base/vectors.py
--rw-rw----   0 corkep     (503) staff       (20)    23373 2023-03-04 22:46:52.000000 spatialmath-python-1.1.6/spatialmath/baseposelist.py
--rw-rw----   0 corkep     (503) staff       (20)    61462 2023-03-28 22:02:18.000000 spatialmath-python-1.1.6/spatialmath/baseposematrix.py
--rwxr--r--   0 corkep     (503) staff       (20)    33236 2023-03-08 07:53:49.000000 spatialmath-python-1.1.6/spatialmath/geom2d.py
--rwxrwx---   0 corkep     (503) staff       (20)    44799 2023-02-26 06:08:44.000000 spatialmath-python-1.1.6/spatialmath/geom3d.py
--rw-r--r--   0 corkep     (503) staff       (20)      504 2023-02-19 01:27:48.000000 spatialmath-python-1.1.6/spatialmath/play_with_types.py
--rw-r--r--   0 corkep     (503) staff       (20)      669 2023-02-02 19:54:18.000000 spatialmath-python-1.1.6/spatialmath/pluckertest.py
--rw-rw----   0 corkep     (503) staff       (20)    19401 2023-03-04 23:19:51.000000 spatialmath-python-1.1.6/spatialmath/pose2d.py
--rw-r--r--   0 corkep     (503) staff       (20)    62223 2023-03-15 05:37:23.000000 spatialmath-python-1.1.6/spatialmath/pose3d.py
--rw-r--r--   0 corkep     (503) staff       (20)      194 2023-02-02 19:54:18.000000 spatialmath-python-1.1.6/spatialmath/profiling.py
--rw-rw----   0 corkep     (503) staff       (20)    78885 2023-03-15 08:35:40.000000 spatialmath-python-1.1.6/spatialmath/quaternion.py
--rw-rw----   0 corkep     (503) staff       (20)    25874 2023-02-26 06:08:44.000000 spatialmath-python-1.1.6/spatialmath/spatialvector.py
--rw-r--r--   0 corkep     (503) staff       (20)      666 2023-02-02 19:54:18.000000 spatialmath-python-1.1.6/spatialmath/test.py
--rwxrwx---   0 corkep     (503) staff       (20)     8106 2023-02-26 06:08:44.000000 spatialmath-python-1.1.6/spatialmath/timing.py
--rw-r--r--   0 corkep     (503) staff       (20)       69 2020-09-23 08:34:00.000000 spatialmath-python-1.1.6/spatialmath/timing_constructor.py
--rw-r--r--   0 corkep     (503) staff       (20)    54965 2023-03-15 07:59:52.000000 spatialmath-python-1.1.6/spatialmath/twist.py
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-04-02 00:19:09.566372 spatialmath-python-1.1.6/spatialmath_python.egg-info/
--rw-rw----   0 corkep     (503) staff       (20)    15921 2023-04-02 00:19:09.000000 spatialmath-python-1.1.6/spatialmath_python.egg-info/PKG-INFO
--rw-rw----   0 corkep     (503) staff       (20)     1449 2023-04-02 00:19:09.000000 spatialmath-python-1.1.6/spatialmath_python.egg-info/SOURCES.txt
--rw-rw----   0 corkep     (503) staff       (20)        1 2023-04-02 00:19:09.000000 spatialmath-python-1.1.6/spatialmath_python.egg-info/dependency_links.txt
--rw-rw----   0 corkep     (503) staff       (20)      230 2023-04-02 00:19:09.000000 spatialmath-python-1.1.6/spatialmath_python.egg-info/requires.txt
--rw-rw----   0 corkep     (503) staff       (20)       12 2023-04-02 00:19:09.000000 spatialmath-python-1.1.6/spatialmath_python.egg-info/top_level.txt
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-04-02 00:19:09.574497 spatialmath-python-1.1.6/tests/
--rw-r--r--   0 corkep     (503) staff       (20)     4072 2021-03-28 05:22:23.000000 spatialmath-python-1.1.6/tests/test_baseposelist.py
--rw-r--r--   0 corkep     (503) staff       (20)     3323 2021-01-16 23:30:46.000000 spatialmath-python-1.1.6/tests/test_dualquaternion.py
--rwxr--r--   0 corkep     (503) staff       (20)     8051 2023-03-08 02:59:23.000000 spatialmath-python-1.1.6/tests/test_geom2d.py
--rwxrwx---   0 corkep     (503) staff       (20)     9378 2023-02-26 06:08:44.000000 spatialmath-python-1.1.6/tests/test_geom3d.py
--rwxr--r--   0 corkep     (503) staff       (20)    13380 2021-04-06 10:29:33.000000 spatialmath-python-1.1.6/tests/test_pose2d.py
--rwxr--r--   0 corkep     (503) staff       (20)    33496 2021-04-06 10:29:51.000000 spatialmath-python-1.1.6/tests/test_pose3d.py
--rw-rw----   0 corkep     (503) staff       (20)    32754 2023-02-26 06:08:44.000000 spatialmath-python-1.1.6/tests/test_quaternion.py
--rw-r--r--   0 corkep     (503) staff       (20)     7266 2020-11-08 07:59:28.000000 spatialmath-python-1.1.6/tests/test_spatialvector.py
--rwxrwx---   0 corkep     (503) staff       (20)    10657 2023-02-26 06:08:44.000000 spatialmath-python-1.1.6/tests/test_twist.py
+drwxrwx---   0 corkep     (503) staff       (20)        0 2023-04-23 02:10:40.185419 spatialmath-python-1.1.7/
+-rw-r--r--   0 corkep     (503) staff       (20)     1068 2020-05-03 01:56:32.000000 spatialmath-python-1.1.7/LICENSE
+-rw-rw----   0 corkep     (503) staff       (20)    15921 2023-04-23 02:10:40.184791 spatialmath-python-1.1.7/PKG-INFO
+-rw-r--r--   0 corkep     (503) staff       (20)    14506 2023-03-08 07:55:36.000000 spatialmath-python-1.1.7/README.md
+-rw-rw----   0 corkep     (503) staff       (20)     2238 2023-04-23 02:10:25.000000 spatialmath-python-1.1.7/pyproject.toml
+-rw-rw----   0 corkep     (503) staff       (20)       38 2023-04-23 02:10:40.185592 spatialmath-python-1.1.7/setup.cfg
+drwxrwx---   0 corkep     (503) staff       (20)        0 2023-04-23 02:10:40.148255 spatialmath-python-1.1.7/spatialmath/
+-rw-rw----   0 corkep     (503) staff       (20)    10807 2023-02-26 06:08:44.000000 spatialmath-python-1.1.7/spatialmath/DualQuaternion.py
+-rw-rw----   0 corkep     (503) staff       (20)     1223 2023-03-06 05:53:49.000000 spatialmath-python-1.1.7/spatialmath/__init__.py
+drwxrwx---   0 corkep     (503) staff       (20)        0 2023-04-23 02:10:40.172054 spatialmath-python-1.1.7/spatialmath/base/
+-rw-r--r--   0 corkep     (503) staff       (20)     6133 2023-03-15 07:14:42.000000 spatialmath-python-1.1.7/spatialmath/base/__init__.py
+-rw-rw----   0 corkep     (503) staff       (20)     4376 2023-02-26 06:08:44.000000 spatialmath-python-1.1.7/spatialmath/base/_types_311.py
+-rw-rw----   0 corkep     (503) staff       (20)     3668 2023-02-27 02:47:31.000000 spatialmath-python-1.1.7/spatialmath/base/_types_35.py
+-rw-rw----   0 corkep     (503) staff       (20)     4453 2023-02-26 06:08:44.000000 spatialmath-python-1.1.7/spatialmath/base/_types_39.py
+-rwxrwx---   0 corkep     (503) staff       (20)    28884 2023-03-21 10:14:47.000000 spatialmath-python-1.1.7/spatialmath/base/animate.py
+-rw-r--r--   0 corkep     (503) staff       (20)      600 2021-05-23 01:42:29.000000 spatialmath-python-1.1.7/spatialmath/base/animationbug.py
+-rw-r--r--   0 corkep     (503) staff       (20)    21504 2023-03-16 00:24:27.000000 spatialmath-python-1.1.7/spatialmath/base/argcheck.py
+-rw-r--r--   0 corkep     (503) staff       (20)    62772 2023-04-23 00:46:05.000000 spatialmath-python-1.1.7/spatialmath/base/graphics.py
+-rwxr--r--   0 corkep     (503) staff       (20)     2091 2021-05-23 01:42:29.000000 spatialmath-python-1.1.7/spatialmath/base/m2p.py
+-rw-r--r--   0 corkep     (503) staff       (20)    11666 2023-03-06 07:02:14.000000 spatialmath-python-1.1.7/spatialmath/base/numeric.py
+-rwxrwx---   0 corkep     (503) staff       (20)    29711 2023-03-28 10:16:43.000000 spatialmath-python-1.1.7/spatialmath/base/quaternions.py
+-rw-rw----   0 corkep     (503) staff       (20)     6973 2023-02-27 02:51:57.000000 spatialmath-python-1.1.7/spatialmath/base/symbolic.py
+-rw-r--r--   0 corkep     (503) staff       (20)     2526 2023-02-01 09:24:26.000000 spatialmath-python-1.1.7/spatialmath/base/timing.py
+-rw-r--r--   0 corkep     (503) staff       (20)    45818 2023-03-28 11:10:08.000000 spatialmath-python-1.1.7/spatialmath/base/transforms2d.py
+-rw-rw----   0 corkep     (503) staff       (20)   110878 2023-03-28 22:05:19.000000 spatialmath-python-1.1.7/spatialmath/base/transforms3d.py
+-rw-rw----   0 corkep     (503) staff       (20)    24862 2023-03-26 07:02:50.000000 spatialmath-python-1.1.7/spatialmath/base/transformsNd.py
+-rw-r--r--   0 corkep     (503) staff       (20)     1700 2023-02-01 09:24:27.000000 spatialmath-python-1.1.7/spatialmath/base/trplot2.py
+-rw-rw----   0 corkep     (503) staff       (20)      229 2023-02-26 06:08:44.000000 spatialmath-python-1.1.7/spatialmath/base/types.py
+-rw-rw----   0 corkep     (503) staff       (20)    19884 2023-03-26 23:53:23.000000 spatialmath-python-1.1.7/spatialmath/base/vectors.py
+-rw-rw----   0 corkep     (503) staff       (20)    23373 2023-03-04 22:46:52.000000 spatialmath-python-1.1.7/spatialmath/baseposelist.py
+-rw-rw----   0 corkep     (503) staff       (20)    61462 2023-03-28 22:02:18.000000 spatialmath-python-1.1.7/spatialmath/baseposematrix.py
+-rwxr--r--   0 corkep     (503) staff       (20)    33236 2023-03-08 07:53:49.000000 spatialmath-python-1.1.7/spatialmath/geom2d.py
+-rwxrwx---   0 corkep     (503) staff       (20)    44799 2023-02-26 06:08:44.000000 spatialmath-python-1.1.7/spatialmath/geom3d.py
+-rw-r--r--   0 corkep     (503) staff       (20)      504 2023-02-19 01:27:48.000000 spatialmath-python-1.1.7/spatialmath/play_with_types.py
+-rw-r--r--   0 corkep     (503) staff       (20)      669 2023-02-02 19:54:18.000000 spatialmath-python-1.1.7/spatialmath/pluckertest.py
+-rw-rw----   0 corkep     (503) staff       (20)    19401 2023-03-04 23:19:51.000000 spatialmath-python-1.1.7/spatialmath/pose2d.py
+-rw-r--r--   0 corkep     (503) staff       (20)    62223 2023-03-15 05:37:23.000000 spatialmath-python-1.1.7/spatialmath/pose3d.py
+-rw-r--r--   0 corkep     (503) staff       (20)      194 2023-02-02 19:54:18.000000 spatialmath-python-1.1.7/spatialmath/profiling.py
+-rw-rw----   0 corkep     (503) staff       (20)    78885 2023-03-15 08:35:40.000000 spatialmath-python-1.1.7/spatialmath/quaternion.py
+-rw-rw----   0 corkep     (503) staff       (20)    25874 2023-02-26 06:08:44.000000 spatialmath-python-1.1.7/spatialmath/spatialvector.py
+-rw-r--r--   0 corkep     (503) staff       (20)      666 2023-02-02 19:54:18.000000 spatialmath-python-1.1.7/spatialmath/test.py
+-rwxrwx---   0 corkep     (503) staff       (20)     8106 2023-02-26 06:08:44.000000 spatialmath-python-1.1.7/spatialmath/timing.py
+-rw-r--r--   0 corkep     (503) staff       (20)       69 2020-09-23 08:34:00.000000 spatialmath-python-1.1.7/spatialmath/timing_constructor.py
+-rw-r--r--   0 corkep     (503) staff       (20)    54965 2023-03-15 07:59:52.000000 spatialmath-python-1.1.7/spatialmath/twist.py
+drwxrwx---   0 corkep     (503) staff       (20)        0 2023-04-23 02:10:40.175264 spatialmath-python-1.1.7/spatialmath_python.egg-info/
+-rw-rw----   0 corkep     (503) staff       (20)    15921 2023-04-23 02:10:40.000000 spatialmath-python-1.1.7/spatialmath_python.egg-info/PKG-INFO
+-rw-rw----   0 corkep     (503) staff       (20)     1449 2023-04-23 02:10:40.000000 spatialmath-python-1.1.7/spatialmath_python.egg-info/SOURCES.txt
+-rw-rw----   0 corkep     (503) staff       (20)        1 2023-04-23 02:10:40.000000 spatialmath-python-1.1.7/spatialmath_python.egg-info/dependency_links.txt
+-rw-rw----   0 corkep     (503) staff       (20)      230 2023-04-23 02:10:40.000000 spatialmath-python-1.1.7/spatialmath_python.egg-info/requires.txt
+-rw-rw----   0 corkep     (503) staff       (20)       12 2023-04-23 02:10:40.000000 spatialmath-python-1.1.7/spatialmath_python.egg-info/top_level.txt
+drwxrwx---   0 corkep     (503) staff       (20)        0 2023-04-23 02:10:40.183727 spatialmath-python-1.1.7/tests/
+-rw-r--r--   0 corkep     (503) staff       (20)     4072 2021-03-28 05:22:23.000000 spatialmath-python-1.1.7/tests/test_baseposelist.py
+-rw-r--r--   0 corkep     (503) staff       (20)     3323 2021-01-16 23:30:46.000000 spatialmath-python-1.1.7/tests/test_dualquaternion.py
+-rwxr--r--   0 corkep     (503) staff       (20)     8051 2023-03-08 02:59:23.000000 spatialmath-python-1.1.7/tests/test_geom2d.py
+-rwxrwx---   0 corkep     (503) staff       (20)     9378 2023-02-26 06:08:44.000000 spatialmath-python-1.1.7/tests/test_geom3d.py
+-rwxr--r--   0 corkep     (503) staff       (20)    13380 2021-04-06 10:29:33.000000 spatialmath-python-1.1.7/tests/test_pose2d.py
+-rwxr--r--   0 corkep     (503) staff       (20)    33496 2021-04-06 10:29:51.000000 spatialmath-python-1.1.7/tests/test_pose3d.py
+-rw-rw----   0 corkep     (503) staff       (20)    32754 2023-02-26 06:08:44.000000 spatialmath-python-1.1.7/tests/test_quaternion.py
+-rw-r--r--   0 corkep     (503) staff       (20)     7266 2020-11-08 07:59:28.000000 spatialmath-python-1.1.7/tests/test_spatialvector.py
+-rwxrwx---   0 corkep     (503) staff       (20)    10657 2023-02-26 06:08:44.000000 spatialmath-python-1.1.7/tests/test_twist.py
```

### Comparing `spatialmath-python-1.1.6/LICENSE` & `spatialmath-python-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/PKG-INFO` & `spatialmath-python-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialmath-python
-Version: 1.1.6
+Version: 1.1.7
 Summary: Provides spatial maths capability for Python
 Author-email: Peter Corke <rvc@petercorke.com>
 Project-URL: Homepage, https://github.com/petercorke/spatialmath-python
 Project-URL: Bug Tracker, https://github.com/petercorke/spatialmath-python/issues
 Project-URL: Documentation, https://petercorke.github.io/petercorke/spatialmath-python
 Project-URL: Source, https://github.com/petercorke/petercorke/spatialmath-python
 Keywords: spatial-math,spatial math,SO2,SE2,SO3,SE3,SO(2),SE(2),SO(3),SE(3),twist,product of exponential,translation,orientation,angle-axis,Lie group,skew symmetric matrix,pose,translation,rotation matrix,rigid body transform,homogeneous transformation,Euler angles,roll-pitch-yaw angles,quaternion,unit-quaternion,robotics,robot vision,computer vision
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spatialmath-python Version: 1.1.6 Summary: Provides
+Metadata-Version: 2.1 Name: spatialmath-python Version: 1.1.7 Summary: Provides
 spatial maths capability for Python Author-email: Peter Corke
 petercorke.com> Project-URL: Homepage, https://github.com/petercorke/
 spatialmath-python Project-URL: Bug Tracker, https://github.com/petercorke/
 spatialmath-python/issues Project-URL: Documentation, https://
 petercorke.github.io/petercorke/spatialmath-python Project-URL: Source, https:/
 /github.com/petercorke/petercorke/spatialmath-python Keywords: spatial-
 math,spatial math,SO2,SE2,SO3,SE3,SO(2),SE(2),SO(3),SE(3),twist,product of
```

### Comparing `spatialmath-python-1.1.6/README.md` & `spatialmath-python-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/pyproject.toml` & `spatialmath-python-1.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "spatialmath-python"
-version = "1.1.6"
+version = "1.1.7"
 authors = [
   { name="Peter Corke", email="rvc@petercorke.com" },
 ]
 description = "Provides spatial maths capability for Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `spatialmath-python-1.1.6/spatialmath/DualQuaternion.py` & `spatialmath-python-1.1.7/spatialmath/DualQuaternion.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/spatialmath/__init__.py` & `spatialmath-python-1.1.7/spatialmath/__init__.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/spatialmath/base/__init__.py` & `spatialmath-python-1.1.7/spatialmath/base/__init__.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/spatialmath/base/_types_311.py` & `spatialmath-python-1.1.7/spatialmath/base/_types_311.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/spatialmath/base/_types_35.py` & `spatialmath-python-1.1.7/spatialmath/base/_types_35.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/spatialmath/base/_types_39.py` & `spatialmath-python-1.1.7/spatialmath/base/_types_39.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/spatialmath/base/animate.py` & `spatialmath-python-1.1.7/spatialmath/base/animate.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/spatialmath/base/animationbug.py` & `spatialmath-python-1.1.7/spatialmath/base/animationbug.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/spatialmath/base/argcheck.py` & `spatialmath-python-1.1.7/spatialmath/base/argcheck.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/spatialmath/base/graphics.py` & `spatialmath-python-1.1.7/spatialmath/base/graphics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1566,15 +1566,15 @@
 
         plt.sca(ax)
         # plt.axes(ax)
 
         return ax
 
     def plotvol2(
-        dim: ArrayLike,
+        dim: ArrayLike = None,
         ax: Optional[plt.Axes] = None,
         equal: Optional[bool] = True,
         grid: Optional[bool] = False,
         labels: Optional[bool] = True,
         new: Optional[bool] = False,
     ) -> plt.Axes:
         """
@@ -1597,18 +1597,23 @@
         [A, B, C, D]     A:B     C:D
         ==============  ======  ======
 
         :seealso: :func:`plotvol3`, :func:`expand_dims`
         """
         ax = axes_logic(ax, 2, new=new)
 
-        dims = expand_dims(dim, 2)
+        if dim is None:
+            ax.autoscale(True)
+        else:
+            dims = expand_dims(dim, 2)
+            ax.axis(dims)
+
         # if ax is None:
         #     ax = plt.subplot()
-        ax.axis(dims)
+
         if labels:
             ax.set_xlabel("X")
             ax.set_ylabel("Y")
 
         if equal:
             ax.set_aspect("equal")
         if grid:
```

### Comparing `spatialmath-python-1.1.6/spatialmath/base/m2p.py` & `spatialmath-python-1.1.7/spatialmath/base/m2p.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/spatialmath/base/numeric.py` & `spatialmath-python-1.1.7/spatialmath/base/numeric.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/spatialmath/base/quaternions.py` & `spatialmath-python-1.1.7/spatialmath/base/quaternions.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/spatialmath/base/symbolic.py` & `spatialmath-python-1.1.7/spatialmath/base/symbolic.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/spatialmath/base/timing.py` & `spatialmath-python-1.1.7/spatialmath/base/timing.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/spatialmath/base/transforms2d.py` & `spatialmath-python-1.1.7/spatialmath/base/transforms2d.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/spatialmath/base/transforms3d.py` & `spatialmath-python-1.1.7/spatialmath/base/transforms3d.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/spatialmath/base/transformsNd.py` & `spatialmath-python-1.1.7/spatialmath/base/transformsNd.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/spatialmath/base/trplot2.py` & `spatialmath-python-1.1.7/spatialmath/base/trplot2.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/spatialmath/base/vectors.py` & `spatialmath-python-1.1.7/spatialmath/base/vectors.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/spatialmath/baseposelist.py` & `spatialmath-python-1.1.7/spatialmath/baseposelist.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/spatialmath/baseposematrix.py` & `spatialmath-python-1.1.7/spatialmath/baseposematrix.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/spatialmath/geom2d.py` & `spatialmath-python-1.1.7/spatialmath/geom2d.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/spatialmath/geom3d.py` & `spatialmath-python-1.1.7/spatialmath/geom3d.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/spatialmath/pluckertest.py` & `spatialmath-python-1.1.7/spatialmath/pluckertest.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/spatialmath/pose2d.py` & `spatialmath-python-1.1.7/spatialmath/pose2d.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/spatialmath/pose3d.py` & `spatialmath-python-1.1.7/spatialmath/pose3d.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/spatialmath/quaternion.py` & `spatialmath-python-1.1.7/spatialmath/quaternion.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/spatialmath/spatialvector.py` & `spatialmath-python-1.1.7/spatialmath/spatialvector.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/spatialmath/test.py` & `spatialmath-python-1.1.7/spatialmath/test.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/spatialmath/timing.py` & `spatialmath-python-1.1.7/spatialmath/timing.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/spatialmath/twist.py` & `spatialmath-python-1.1.7/spatialmath/twist.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/spatialmath_python.egg-info/PKG-INFO` & `spatialmath-python-1.1.7/spatialmath_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialmath-python
-Version: 1.1.6
+Version: 1.1.7
 Summary: Provides spatial maths capability for Python
 Author-email: Peter Corke <rvc@petercorke.com>
 Project-URL: Homepage, https://github.com/petercorke/spatialmath-python
 Project-URL: Bug Tracker, https://github.com/petercorke/spatialmath-python/issues
 Project-URL: Documentation, https://petercorke.github.io/petercorke/spatialmath-python
 Project-URL: Source, https://github.com/petercorke/petercorke/spatialmath-python
 Keywords: spatial-math,spatial math,SO2,SE2,SO3,SE3,SO(2),SE(2),SO(3),SE(3),twist,product of exponential,translation,orientation,angle-axis,Lie group,skew symmetric matrix,pose,translation,rotation matrix,rigid body transform,homogeneous transformation,Euler angles,roll-pitch-yaw angles,quaternion,unit-quaternion,robotics,robot vision,computer vision
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spatialmath-python Version: 1.1.6 Summary: Provides
+Metadata-Version: 2.1 Name: spatialmath-python Version: 1.1.7 Summary: Provides
 spatial maths capability for Python Author-email: Peter Corke
 petercorke.com> Project-URL: Homepage, https://github.com/petercorke/
 spatialmath-python Project-URL: Bug Tracker, https://github.com/petercorke/
 spatialmath-python/issues Project-URL: Documentation, https://
 petercorke.github.io/petercorke/spatialmath-python Project-URL: Source, https:/
 /github.com/petercorke/petercorke/spatialmath-python Keywords: spatial-
 math,spatial math,SO2,SE2,SO3,SE3,SO(2),SE(2),SO(3),SE(3),twist,product of
```

### Comparing `spatialmath-python-1.1.6/spatialmath_python.egg-info/SOURCES.txt` & `spatialmath-python-1.1.7/spatialmath_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/tests/test_baseposelist.py` & `spatialmath-python-1.1.7/tests/test_baseposelist.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/tests/test_dualquaternion.py` & `spatialmath-python-1.1.7/tests/test_dualquaternion.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/tests/test_geom2d.py` & `spatialmath-python-1.1.7/tests/test_geom2d.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/tests/test_geom3d.py` & `spatialmath-python-1.1.7/tests/test_geom3d.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/tests/test_pose2d.py` & `spatialmath-python-1.1.7/tests/test_pose2d.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/tests/test_pose3d.py` & `spatialmath-python-1.1.7/tests/test_pose3d.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/tests/test_quaternion.py` & `spatialmath-python-1.1.7/tests/test_quaternion.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/tests/test_spatialvector.py` & `spatialmath-python-1.1.7/tests/test_spatialvector.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.6/tests/test_twist.py` & `spatialmath-python-1.1.7/tests/test_twist.py`

 * *Files identical despite different names*

