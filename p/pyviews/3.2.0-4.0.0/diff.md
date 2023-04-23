# Comparing `tmp/pyviews-3.2.0.tar.gz` & `tmp/pyviews-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyviews-3.2.0.tar", last modified: Wed Nov 16 09:12:14 2022, max compression
+gzip compressed data, was "pyviews-4.0.0.tar", last modified: Sun Apr 23 12:07:55 2023, max compression
```

## Comparing `pyviews-3.2.0.tar` & `pyviews-4.0.0.tar`

### file list

```diff
@@ -1,51 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 09:12:14.414983 pyviews-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-11-16 09:11:51.000000 pyviews-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-16 09:11:51.000000 pyviews-3.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2225 2022-11-16 09:12:14.414983 pyviews-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1432 2022-11-16 09:11:51.000000 pyviews-3.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1163 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 09:12:14.402983 pyviews-3.2.0/pyviews/
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyviews/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 09:12:14.406983 pyviews-3.2.0/pyviews/binding/
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyviews/binding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2622 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyviews/binding/binder.py
--rw-r--r--   0 runner    (1001) docker     (121)     3262 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyviews/binding/expression.py
--rw-r--r--   0 runner    (1001) docker     (121)      395 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyviews/binding/inject.py
--rw-r--r--   0 runner    (1001) docker     (121)     2242 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyviews/binding/inline.py
--rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyviews/binding/observable.py
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyviews/binding/once.py
--rw-r--r--   0 runner    (1001) docker     (121)      652 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyviews/binding/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     2117 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyviews/binding/twoways.py
--rw-r--r--   0 runner    (1001) docker     (121)     3468 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyviews/binding_node.py
--rw-r--r--   0 runner    (1001) docker     (121)     1925 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyviews/code.py
--rw-r--r--   0 runner    (1001) docker     (121)     6736 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyviews/containers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 09:12:14.410983 pyviews-3.2.0/pyviews/core/
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyviews/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      547 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyviews/core/binding.py
--rw-r--r--   0 runner    (1001) docker     (121)     3383 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyviews/core/error.py
--rw-r--r--   0 runner    (1001) docker     (121)     4796 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyviews/core/observable.py
--rw-r--r--   0 runner    (1001) docker     (121)      736 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyviews/core/reflection.py
--rw-r--r--   0 runner    (1001) docker     (121)     2697 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyviews/core/rendering.py
--rw-r--r--   0 runner    (1001) docker     (121)     5191 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyviews/core/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 09:12:14.410983 pyviews-3.2.0/pyviews/expression/
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyviews/expression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      786 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyviews/expression/error.py
--rw-r--r--   0 runner    (1001) docker     (121)     5043 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyviews/expression/expression.py
--rw-r--r--   0 runner    (1001) docker     (121)      975 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyviews/expression/parsing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1910 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyviews/pipes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2304 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyviews/presenter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 09:12:14.410983 pyviews-3.2.0/pyviews/rendering/
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyviews/rendering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2362 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyviews/rendering/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     5326 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyviews/rendering/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyviews/rendering/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1340 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyviews/rendering/views.py
--rw-r--r--   0 runner    (1001) docker     (121)     1213 2022-11-16 09:11:51.000000 pyviews-3.2.0/pyviews/setters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 09:12:14.402983 pyviews-3.2.0/pyviews.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2225 2022-11-16 09:12:14.000000 pyviews-3.2.0/pyviews.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1023 2022-11-16 09:12:14.000000 pyviews-3.2.0/pyviews.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 09:12:14.000000 pyviews-3.2.0/pyviews.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-11-16 09:12:14.000000 pyviews-3.2.0/pyviews.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-16 09:12:14.000000 pyviews-3.2.0/pyviews.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-16 09:12:14.414983 pyviews-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-11-16 09:11:51.000000 pyviews-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:07:55.066591 pyviews-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-23 12:07:33.000000 pyviews-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-23 12:07:55.066591 pyviews-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-23 12:07:33.000000 pyviews-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:07:55.058591 pyviews-4.0.0/pyviews/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:07:55.062591 pyviews-4.0.0/pyviews/binding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/binding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/binding/binder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/binding/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/binding/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/binding/inject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/binding/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/binding/observable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/binding/once.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:07:55.062591 pyviews-4.0.0/pyviews/binding/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/binding/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/binding/tests/binder_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/binding/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/binding/tests/config_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/binding/tests/expression_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/binding/tests/inject_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/binding/tests/inline_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/binding/tests/observable_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/binding/tests/once_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/binding/tests/twoways_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/binding/twoways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/binding_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/containers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:07:55.062591 pyviews-4.0.0/pyviews/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/core/binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/core/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/core/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/core/reflection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/core/rendering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:07:55.062591 pyviews-4.0.0/pyviews/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/core/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/core/tests/binding_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/core/tests/error_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/core/tests/expression_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/core/tests/reflection_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/core/tests/rendering_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/core/tests/xml_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/core/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/pipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/presenter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:07:55.062591 pyviews-4.0.0/pyviews/rendering/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/rendering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/rendering/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/rendering/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/rendering/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:07:55.066591 pyviews-4.0.0/pyviews/rendering/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/rendering/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/rendering/tests/config_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/rendering/tests/context_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/rendering/tests/pipeline_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/rendering/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/setters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:07:55.066591 pyviews-4.0.0/pyviews/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/tests/binding_node_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/tests/code_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/tests/containers_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/tests/pipes_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/tests/presenter_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-04-23 12:07:33.000000 pyviews-4.0.0/pyviews/tests/setters_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:07:55.058591 pyviews-4.0.0/pyviews.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-23 12:07:55.000000 pyviews-4.0.0/pyviews.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-23 12:07:55.000000 pyviews-4.0.0/pyviews.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 12:07:55.000000 pyviews-4.0.0/pyviews.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-23 12:07:55.000000 pyviews-4.0.0/pyviews.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 12:07:55.000000 pyviews-4.0.0/pyviews.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 12:07:55.066591 pyviews-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-23 12:07:33.000000 pyviews-4.0.0/setup.py
```

### Comparing `pyviews-3.2.0/LICENSE` & `pyviews-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyviews-3.2.0/PKG-INFO` & `pyviews-4.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyviews
-Version: 3.2.0
+Version: 4.0.0
 Summary: Base package for xml views
 Project-URL: Homepage, https://github.com/eumis/pyviews
 Keywords: binding,pyviews,python,mvvm,tkviews,wxviews
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyviews-3.2.0/README.md` & `pyviews-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pyviews-3.2.0/pyviews/binding/binder.py` & `pyviews-4.0.0/pyviews/binding/binder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Binder"""
 
-from typing import Optional, Union, Callable, NamedTuple
+from typing import Callable, NamedTuple, Optional, Union
 
-from pyviews.core import BindingError, Node, Setter, XmlAttr, Binding, InstanceNode
+from pyviews.core.binding import Binding, BindingError
+from pyviews.core.rendering import InstanceNode, Node, Setter
+from pyviews.core.xml import XmlAttr
 
 
 class BindingContext(dict):
     """Used as binding arguments passed to binder and rule step"""
 
     @property
     def node(self) -> Union[Node, InstanceNode]:
@@ -53,16 +55,20 @@
 
 class Binder:
     """Applies binding"""
 
     def __init__(self):
         self._rules = {}
 
-    def add_rule(self, binding_type: str, bind: Callable[[BindingContext], Optional[Binding]],
-                 suitable: Optional[Callable[[BindingContext], bool]] = None):
+    def add_rule(
+        self,
+        binding_type: str,
+        bind: Callable[[BindingContext], Optional[Binding]],
+        suitable: Optional[Callable[[BindingContext], bool]] = None
+    ):
         """Adds new rule"""
         suitable = suitable if suitable else lambda _: True
         if binding_type not in self._rules:
             self._rules[binding_type] = []
 
         self._rules[binding_type].insert(0, BindingRule(suitable, bind))
```

### Comparing `pyviews-3.2.0/pyviews/binding/expression.py` & `pyviews-4.0.0/pyviews/binding/expression.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,78 +1,63 @@
 """Expression binding"""
 
 from functools import partial
-from typing import Callable, List, Any
+from typing import Any, Callable, List, Set, Union
 
 from pyviews.binding.binder import BindingContext
-from pyviews.core import Binding, BindingCallback, InheritedDict, Observable, BindingError, \
-    PyViewsError
-from pyviews.core import error_handling
-from pyviews.expression import Expression, ObjectNode, execute
-from pyviews.expression.expression import ENTRY, ATTRIBUTE, INDEX
-
-_GET_VALUE = {
-    ENTRY: lambda inst, key: inst.get(key),
-    ATTRIBUTE: getattr,
-    INDEX: lambda inst, key: inst[key]
-}
+from pyviews.core.binding import Bindable, BindableRecord, Binding, BindingCallback, BindingError, recording
+from pyviews.core.error import PyViewsError, error_handling
+from pyviews.core.expression import Expression, execute
+from pyviews.core.rendering import NodeGlobals
 
 
 class ExpressionBinding(Binding):
     """Binds target to expression result"""
 
-    def __init__(self, callback: BindingCallback, expression: Expression, expr_vars: InheritedDict):
+    def __init__(self, callback: BindingCallback, expression: Expression, expr_vars: NodeGlobals):
         super().__init__()
         self._callback: BindingCallback = callback
         self._expression: Expression = expression
         self._destroy_functions: List[Callable] = []
-        self._vars: InheritedDict = expr_vars
+        self._vars: NodeGlobals = expr_vars
 
-    def bind(self, execute_callback=True):
+    def bind(self, execute_callback = True):
         self.destroy()
-        objects_tree = self._expression.get_object_tree()
+        with recording() as records:
+            value = execute(self._expression, self._vars)
         with error_handling(BindingError, self._add_error_info):
-            self._create_dependencies(self._vars, objects_tree)
+            self._create_dependencies(records)
         if execute_callback:
-            self._execute_callback()
+            self._callback(value)
 
-    def _create_dependencies(self, inst: Any, var_tree: ObjectNode):
-        if isinstance(inst, Observable):
-            self._subscribe_for_changes(inst, var_tree)
-
-        for entry in var_tree.children:
-            key = execute(entry.key, self._vars.to_dictionary()) \
-                if isinstance(entry.key, Expression) else entry.key
-            child_inst = _GET_VALUE[entry.type](inst, key)
-            if child_inst is not None:
-                self._create_dependencies(child_inst, entry)
+    def _create_dependencies(self, records: Set[BindableRecord]):
+        for record in records:
+            self._subscribe_for_changes(record.bindable, record.key)
 
-    def _subscribe_for_changes(self, inst: Observable, var_tree: ObjectNode):
+    def _subscribe_for_changes(self, inst: Bindable, key: str):
         try:
-            for entry in var_tree.children:
-                inst.observe(entry.key, self._update_callback)
-                self._destroy_functions.append(
-                    partial(inst.release, entry.key, self._update_callback))
+            inst.observe(key, self._update_callback)
+            self._destroy_functions.append(partial(inst.release, key, self._update_callback))
         except KeyError:
             pass
 
     def _update_callback(self, new_val, old_val):
         with error_handling(BindingError, self._add_error_info):
-            if isinstance(new_val, Observable) or isinstance(old_val, Observable):
+            if isinstance(new_val, Bindable) or isinstance(old_val, Bindable):
                 self.bind()
             else:
                 self._execute_callback()
 
     def _add_error_info(self, error: PyViewsError):
         error.add_info('Binding', self)
         error.add_info('Expression', self._expression.code)
         error.add_info('Callback', self._callback)
 
     def _execute_callback(self):
-        value = execute(self._expression, self._vars.to_dictionary())
+        value = execute(self._expression, self._vars)
         self._callback(value)
 
     def destroy(self):
         for destroy in self._destroy_functions:
             destroy()
         self._destroy_functions = []
 
@@ -80,7 +65,21 @@
 def bind_setter_to_expression(context: BindingContext) -> Binding:
     """Binds callback to expression result changes"""
     expr = Expression(context.expression_body)
     callback = partial(context.setter, context.node, context.xml_attr.name)
     binding = ExpressionBinding(callback, expr, context.node.node_globals)
     binding.bind()
     return binding
+
+
+def get_expression_callback(expression: Union[str, Expression], expr_vars: NodeGlobals) -> BindingCallback:
+    """Returns callback that sets value to property expression"""
+    if isinstance(expression, Expression):
+        expression = expression.code
+    set_expression = Expression(f'{expression} = _expression_callback_value', 'exec')
+    return partial(_expression_callback, set_expression, expr_vars)
+
+
+def _expression_callback(expression: Expression, node_globals: NodeGlobals, value: Any):
+    node_globals['_expression_callback_value'] = value
+    execute(expression, node_globals)
+    node_globals.pop('_expression_callback_value')
```

### Comparing `pyviews-3.2.0/pyviews/binding/inline.py` & `pyviews-4.0.0/pyviews/binding/inline.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 """Inline binding"""
 
 from functools import partial
 
 from pyviews.binding.binder import BindingContext
-from pyviews.expression import Expression, execute
-from pyviews.core import Binding, BindingCallback, error_handling, BindingError, PyViewsError
-from pyviews.core import InheritedDict
+from pyviews.core.binding import Binding, BindingCallback, BindingError
+from pyviews.core.error import PyViewsError, error_handling
+from pyviews.core.expression import Expression, execute
+from pyviews.core.rendering import NodeGlobals
 
 
 class InlineBinding(Binding):
     """Inline binding"""
 
-    def __init__(self, callback: BindingCallback, bind_expression: Expression,
-                 value_expression: Expression,
-                 expr_vars: InheritedDict):
+    def __init__(
+        self,
+        callback: BindingCallback,
+        bind_expression: Expression,
+        value_expression: Expression,
+        expr_vars: NodeGlobals
+    ):
         super().__init__()
         self._callback: BindingCallback = callback
         self._bind_expression: Expression = bind_expression
         self._value_expression: Expression = value_expression
         self._expression_vars = expr_vars
 
         self._destroy = None
 
     def bind(self):
         self.destroy()
-        with error_handling(BindingError('Error occurred during inline binding'),
-                            self._add_error_info):
-            bind = execute(self._bind_expression, self._expression_vars.to_dictionary())
+        with error_handling(BindingError('Error occurred during inline binding'), self._add_error_info):
+            bind = execute(self._bind_expression, self._expression_vars)
             self._destroy = bind(self._execute_callback)
         self._execute_callback()
 
     def _execute_callback(self):
         with error_handling(BindingError, self._add_error_info):
-            value = execute(self._value_expression, self._expression_vars.to_dictionary())
+            value = execute(self._value_expression, self._expression_vars)
             self._callback(value)
 
     def _add_error_info(self, error: PyViewsError):
         error.add_info('Binding', self)
         error.add_info('Bind expression', self._bind_expression.code)
         error.add_info('Value expression', self._value_expression.code)
         error.add_info('Binding callback', self._callback)
```

### Comparing `pyviews-3.2.0/pyviews/binding/observable.py` & `pyviews-4.0.0/pyviews/binding/observable.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Observable binding"""
 
-from pyviews.core import Binding, BindingCallback, BindingError, PyViewsError
-from pyviews.core import Observable, error_handling
+from pyviews.core.binding import Bindable, Binding, BindingCallback, BindingError
+from pyviews.core.error import PyViewsError, error_handling
 
 
 class ObservableBinding(Binding):
     """Binds to observable property"""
 
-    def __init__(self, callback: BindingCallback, observable: Observable, observable_property: str):
+    def __init__(self, callback: BindingCallback, observable: Bindable, observable_property: str):
         super().__init__()
         self._callback = callback
         self._observable = observable
         self._property = observable_property
 
     def bind(self):
         self.destroy()
```

### Comparing `pyviews-3.2.0/pyviews/binding/setup.py` & `pyviews-4.0.0/pyviews/binding/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Binding setup"""
 
+from typing import Optional
 from injectool import add_singleton
 
 from pyviews.binding.binder import Binder
-from pyviews.binding.inject import inject_binding
-from pyviews.binding.once import run_once
 from pyviews.binding.expression import bind_setter_to_expression
+from pyviews.binding.inject import inject_binding
 from pyviews.binding.inline import bind_inline
+from pyviews.binding.once import run_once
 
 
-def use_binding(binder: Binder = None):
+def use_binding(binder: Optional[Binder] = None):
     """setup binder and default bindings"""
     binder = binder if binder else Binder()
+    add_singleton(Binder, binder)
     binder.add_rule('once', run_once)
     binder.add_rule('oneway', bind_setter_to_expression)
     binder.add_rule('inline', bind_inline)
     binder.add_rule('inject', inject_binding)
-    add_singleton(Binder, binder)
```

### Comparing `pyviews-3.2.0/pyviews/binding_node.py` & `pyviews-4.0.0/pyviews/binding_node.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-from typing import Any, NamedTuple, Optional, Union, List
+from typing import Any, List, NamedTuple, Optional, Union
 
-from pyviews.binding import ExpressionBinding
-from pyviews.core import XmlNode, InheritedDict, Node, Setter, Binding
-from pyviews.expression import is_expression, parse_expression, Expression, execute
+from pyviews.binding.expression import ExpressionBinding
+from pyviews.core.binding import Binding
+from pyviews.core.expression import Expression, execute, is_expression, parse_expression
+from pyviews.core.rendering import Node, NodeGlobals, RenderingContext, Setter
+from pyviews.core.xml import XmlNode
 from pyviews.pipes import get_setter
-from pyviews.rendering import RenderingPipeline, RenderingContext
+from pyviews.rendering.pipeline import RenderingPipeline
 
 
 class BindingProperty(NamedTuple):
     name: str
     setter: Setter
     value: Union[Expression, Any]
 
 
 class BindingNode(Node):
-    def __init__(self, xml_node: XmlNode, node_globals: Optional[InheritedDict] = None):
-        super().__init__(xml_node, node_globals=node_globals)
+
+    def __init__(self, xml_node: XmlNode, node_globals: Optional[NodeGlobals] = None):
+        super().__init__(xml_node, node_globals = node_globals)
         self.properties: List[BindingProperty] = []
         self.target: Any = None
         self.when_changed: Optional[Expression] = None
         self.when_true: Optional[Expression] = None
         self.execute_on_bind: bool = True
         self.binding: Optional[Binding] = None
 
@@ -27,71 +30,68 @@
         if self.binding is not None:
             self.binding.destroy()
             self.binding = None
 
 
 def get_binding_pipeline() -> RenderingPipeline:
     """Returns setup for container"""
-    return RenderingPipeline(pipes=[
-        apply_attributes,
-        set_target,
-        bind_changed,
-        bind_true
-    ], name='container pipeline', create_node=create_binding_node)
+    return RenderingPipeline(
+        pipes = [apply_attributes, set_target, bind_changed, bind_true],
+        name = 'container pipeline',
+        create_node = create_binding_node
+    )
 
 
 def apply_attributes(node: BindingNode, _: RenderingContext):
     """Rendering pipe: records attributes to bind"""
     for attr in node.xml_node.attrs:
         value = attr.value.strip() if attr.value else ''
         if is_expression(value):
             value = Expression(parse_expression(value)[1])
         if attr.name == 'when_changed':
             node.when_changed = value
         elif attr.name == 'when_true':
             node.when_true = value
         elif attr.name in node.__dict__:
-            setattr(node, attr.name, execute(value, node.node_globals.to_dictionary()))
+            setattr(node, attr.name, execute(value, node.node_globals))
         else:
             setter = get_setter(attr)
             node.properties.append(BindingProperty(attr.name, setter, value))
 
 
 def set_target(node: BindingNode, context: RenderingContext):
     """Rendering pipe: sets target"""
     if node.target is None:
         node.target = context.parent_node
 
 
 def bind_changed(node: BindingNode, _: RenderingContext):
     """Rendering pipe: creates binding"""
     if node.when_changed:
-        binding = ExpressionBinding(lambda _: binding_callback(node), node.when_changed,
-                                    node.node_globals)
+        binding = ExpressionBinding(lambda _: binding_callback(node), node.when_changed, node.node_globals)
         binding.bind(node.execute_on_bind)
         node.binding = binding
 
 
 def binding_callback(node: BindingNode):
     for prop in node.properties:
-        value = execute(prop.value, node.node_globals.to_dictionary()) \
+        value = execute(prop.value, node.node_globals) \
             if isinstance(prop.value, Expression) else prop.value
         prop.setter(node.target, prop.name, value)
 
 
 def bind_true(node: BindingNode, _: RenderingContext):
     """Rendering pipe: creates binding"""
     if node.when_true:
-        binding = ExpressionBinding(lambda _: binding_true_callback(node), node.when_true,
-                                    node.node_globals)
+        binding = ExpressionBinding(lambda _: binding_true_callback(node), node.when_true, node.node_globals)
         binding.bind(node.execute_on_bind)
         node.binding = binding
 
 
 def binding_true_callback(node: BindingNode):
-    value = execute(node.when_true, node.node_globals.to_dictionary())
+    value = execute(node.when_true, node.node_globals)
     if value:
         binding_callback(node)
 
 
 def create_binding_node(context: RenderingContext) -> BindingNode:
     return BindingNode(context.xml_node, context.node_globals)
```

### Comparing `pyviews-3.2.0/pyviews/code.py` & `pyviews-4.0.0/pyviews/code.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """Contains logic for Code node"""
 
 from sys import exc_info
 from textwrap import dedent
 from traceback import extract_tb
 from typing import Optional
-from pyviews.core import Node, XmlNode, ViewInfo
-from pyviews.expression import ExpressionError
-from pyviews.rendering.common import RenderingContext
+
+from pyviews.core.error import ViewInfo
+from pyviews.core.expression import ExpressionError
+from pyviews.core.rendering import Node
+from pyviews.core.xml import XmlNode
+from pyviews.rendering.context import RenderingContext
 from pyviews.rendering.pipeline import RenderingPipeline
 
 
 class Code(Node):
     """Wrapper under python code inside view"""
 
     def __init__(self, xml_node):
@@ -19,36 +22,38 @@
 
 def run_code(node: Code, context: RenderingContext):
     """Rendering step: executes node content as python module and adds its definitions to globals"""
     if not node.xml_node.text:
         return
     code = node.xml_node.text
     try:
-        globs = context.node_globals.to_dictionary()
+        globs = context.node_globals.copy()
         exec(dedent(code), globs)
         _update_context(globs, context)
     except SyntaxError as err:
         error = _get_error(node.xml_node, err, err.lineno)
         raise error from err
     except BaseException:
         info = exc_info()
         cause, line_number = info[1], extract_tb(info[2])[-1][1]
         error = _get_error(node.xml_node, cause, line_number)
         raise error from cause
 
 
 def _update_context(globs: dict, context: RenderingContext):
-    definitions = [(key, value) for key, value in globs.items()
-                   if key != '__builtins__' and key not in context.node_globals]
+    definitions = [
+        (key, value) for key, value in globs.items() if key != '__builtins__' and key not in context.node_globals
+    ]
     for key, value in definitions:
         context.parent_node.node_globals[key] = value
 
 
 def _get_error(xml_node: XmlNode, cause: Optional[BaseException], line_number: Optional[int]) -> ExpressionError:
     error = ExpressionError()
     error.cause_error = cause
     error.add_view_info(ViewInfo('<Code>', line_number))
     error.add_view_info(xml_node.view_info)
     return error
 
+
 def get_code_pipeline() -> RenderingPipeline[Code, RenderingContext]:
-    return RenderingPipeline[Code, RenderingContext](pipes=[run_code])
+    return RenderingPipeline[Code, RenderingContext](pipes = [run_code])
```

### Comparing `pyviews-3.2.0/pyviews/containers.py` & `pyviews-4.0.0/pyviews/containers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,87 +1,83 @@
 """Contains methods for node setups creation"""
-from typing import Any
+from typing import Any, Optional
 
-from pyviews.core import Node, XmlNode
-from pyviews.core.observable import InheritedDict, Observable
-from pyviews.pipes import render_children, apply_attributes
-from pyviews.rendering import RenderingPipeline, render, RenderingContext, get_child_context
-from pyviews.rendering.views import render_view
+from pyviews.core.binding import Bindable
+from pyviews.core.rendering import Node, NodeGlobals, RenderingContext
+from pyviews.core.xml import XmlNode
+from pyviews.pipes import apply_attributes, render_children
+from pyviews.rendering.context import get_child_context
+from pyviews.rendering.pipeline import RenderingPipeline, render, render_view
 
 
 class Container(Node):
     """Used to combine some xml elements"""
 
 
 def get_container_pipeline() -> RenderingPipeline:
     """Returns setup for container"""
-    return RenderingPipeline(pipes=[
-        apply_attributes,
-        render_container_children
-    ], name='container pipeline')
+    return RenderingPipeline(pipes = [apply_attributes, render_container_children], name = 'container pipeline')
 
 
 def render_container_children(node, context: RenderingContext):
     """Renders container children"""
     render_children(node, context, get_child_context)
 
 
-class View(Container, Observable):
+class View(Container, Bindable):
     """Loads xml from another file"""
 
-    def __init__(self, xml_node: XmlNode, node_globals: InheritedDict = None):
-        Observable.__init__(self)
-        Container.__init__(self, xml_node, node_globals=node_globals)
-        self._name = None
+    def __init__(self, xml_node: XmlNode, node_globals: Optional[NodeGlobals] = None):
+        Bindable.__init__(self)
+        Container.__init__(self, xml_node, node_globals = node_globals)
+        self._name: Optional[str] = None
 
     @property
-    def name(self) -> str:
+    def name(self) -> Optional[str]:
         """Returns view name"""
         return self._name
 
     @name.setter
-    def name(self, value: str):
+    def name(self, value: Optional[str]):
         old_name = self._name
         self._name = value
         self._notify('name', value, old_name)
 
 
 def get_view_pipeline() -> RenderingPipeline:
     """Returns setup for container"""
-    return RenderingPipeline(pipes=[
-        apply_attributes,
-        render_view_content,
-        rerender_on_view_change
-    ], name='view pipeline')
+    return RenderingPipeline(
+        pipes = [apply_attributes, render_view_content, rerender_on_view_change], name = 'view pipeline'
+    )
 
 
 def render_view_content(node: View, context: RenderingContext):
     """Finds view by name attribute and renders it as view node child"""
     if node.name:
         child_context = get_child_context(node.xml_node, node, context)
         content = render_view(node.name, child_context)
         node.add_child(content)
 
 
 def rerender_on_view_change(node: View, context: RenderingContext):
     """Subscribes to name change and renders new view"""
-    node.observe('name', lambda _, __: _rerender_view(node, context))
+    node.observe('name', lambda *_: _rerender_view(node, context))
 
 
 def _rerender_view(node: View, context: RenderingContext):
     node.destroy_children()
     render_view_content(node, context)
 
 
-class For(Container, Observable):
+class For(Container, Bindable):
     """Renders children for every item in items collection"""
 
-    def __init__(self, xml_node: XmlNode, node_globals: InheritedDict = None):
-        Observable.__init__(self)
-        Container.__init__(self, xml_node, node_globals=node_globals)
+    def __init__(self, xml_node: XmlNode, node_globals: Optional[NodeGlobals] = None):
+        Bindable.__init__(self)
+        Container.__init__(self, xml_node, node_globals = node_globals)
         self._items = []
 
     @property
     def items(self):
         """Returns items"""
         return self._items
 
@@ -90,47 +86,44 @@
         old_items = self._items
         self._items = value
         self._notify('items', value, old_items)
 
 
 def get_for_pipeline() -> RenderingPipeline:
     """Returns setup for For node"""
-    return RenderingPipeline(pipes=[
-        apply_attributes,
-        render_for_items,
-        rerender_on_items_change
-    ], name='for pipeline')
+    return RenderingPipeline(
+        pipes = [apply_attributes, render_for_items, rerender_on_items_change], name = 'for pipeline'
+    )
 
 
 def render_for_items(node: For, context: RenderingContext):
     """Renders For children"""
     _render_for_children(node, node.items, context)
 
 
-def _render_for_children(node: For, items: list, context: RenderingContext, index_shift=0):
+def _render_for_children(node: For, items: list, context: RenderingContext, index_shift = 0):
     item_xml_nodes = node.xml_node.children
     for index, item in enumerate(items):
         for xml_node in item_xml_nodes:
             child_context = _get_for_child_args(xml_node, index + index_shift, item, node, context)
             child = render(child_context)
             node.add_child(child)
 
 
-def _get_for_child_args(xml_node: XmlNode, index: int, item: Any,
-                        parent_node: For, context: RenderingContext):
+def _get_for_child_args(xml_node: XmlNode, index: int, item: Any, parent_node: For, context: RenderingContext):
     child_context = get_child_context(xml_node, parent_node, context)
     child_globals = child_context.node_globals
     child_globals['index'] = index
     child_globals['item'] = item
     return child_context
 
 
 def rerender_on_items_change(node: For, context: RenderingContext):
     """Subscribes to items change and updates children"""
-    node.observe('items', lambda _, __: _on_items_changed(node, context))
+    node.observe('items', lambda *_: _on_items_changed(node, context))
 
 
 def _on_items_changed(node: For, context: RenderingContext):
     _destroy_overflow(node)
     _update_existing(node)
     _create_not_existing(node, context)
 
@@ -165,20 +158,20 @@
     item_children_count = len(node.xml_node.children)
     start = int(len(node.children) / item_children_count)
     end = len(node.items)
     items = [node.items[i] for i in range(start, end)]
     _render_for_children(node, items, context, start)
 
 
-class If(Container, Observable):
+class If(Container, Bindable):
     """Renders children if condition is True"""
 
-    def __init__(self, xml_node: XmlNode, node_globals: InheritedDict = None):
-        Observable.__init__(self)
-        Container.__init__(self, xml_node, node_globals=node_globals)
+    def __init__(self, xml_node: XmlNode, node_globals: Optional[NodeGlobals] = None):
+        Bindable.__init__(self)
+        Container.__init__(self, xml_node, node_globals = node_globals)
         self._condition = False
 
     @property
     def condition(self):
         """Returns condition"""
         return self._condition
 
@@ -187,28 +180,24 @@
         old_condition = self._condition
         self._condition = value
         self._notify('condition', value, old_condition)
 
 
 def get_if_pipeline() -> RenderingPipeline:
     """Returns setup for For node"""
-    return RenderingPipeline(pipes=[
-        apply_attributes,
-        render_if,
-        rerender_on_condition_change
-    ], name='if pipeline')
+    return RenderingPipeline(pipes = [apply_attributes, render_if, rerender_on_condition_change], name = 'if pipeline')
 
 
 def render_if(node: If, context: RenderingContext):
     """Renders children nodes if condition is true"""
     if node.condition:
         render_children(node, context, get_child_context)
 
 
 def rerender_on_condition_change(node: If, context: RenderingContext):
     """Rerenders if on condition change"""
-    node.observe('condition', lambda _, __: _on_condition_change(node, context))
+    node.observe('condition', lambda *_: _on_condition_change(node, context))
 
 
 def _on_condition_change(node: If, context: RenderingContext):
     node.destroy_children()
     render_if(node, context)
```

### Comparing `pyviews-3.2.0/pyviews/core/error.py` & `pyviews-4.0.0/pyviews/core/error.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """Common core functionality"""
 
+from collections import namedtuple
 from contextlib import contextmanager
 from os import linesep
-from collections import namedtuple
 from sys import exc_info
-from typing import Callable, Optional, Union, Type, Generator, List, Any
+from typing import Any, Callable, Generator, List, Optional, Type, Union
 
 ViewInfo = namedtuple('ViewInfo', ['view', 'line'])
 
 
 class PyViewsError(Exception):
     """Base error class for custom exceptions"""
 
-    def __init__(self, message: str = '', view_info: Optional[ViewInfo] = None):
+    def __init__(self, message: Optional[str] = None, view_info: Optional[ViewInfo] = None):
         super().__init__(linesep)
         self.infos: List[str] = []
         self.view_infos: List[ViewInfo] = []
-        # noinspection PyTypeChecker
         self.cause_error: Optional[BaseException] = None
-        self.message = message
+        self.message = message if message else ''
         if view_info:
             self.add_view_info(view_info)
 
     def add_info(self, header: str, message: Any):
         """Adds "header: message" line to error message"""
         try:
             next(info for info in self.infos if info.startswith(header))
@@ -37,31 +36,30 @@
         """Adds view information to error message"""
         try:
             next(info for info in self.view_infos if info.view == view_info.view)
         except StopIteration:
             self.view_infos.insert(0, view_info)
 
     def __str__(self) -> str:
-        self.args = (linesep.join(self._get_messages()),) + self.args[1:]
+        self.args = (linesep.join(self._get_messages()), ) + self.args[1:]
         return super().__str__()
 
     def _get_messages(self) -> Generator[str, None, None]:
         yield from self._get_info()
         yield from self._get_error()
         yield from self._get_view_info()
 
     def _get_info(self) -> Generator[str, None, None]:
         yield self._get_separator('Info')
         yield from self.infos
 
     def _get_error(self) -> Generator[str, None, None]:
         yield self._get_separator(self.__class__.__name__)
         if self.cause_error:
-            yield self._format_info('Cause error',
-                                    f'{type(self.cause_error).__name__} - {self.cause_error}')
+            yield self._format_info('Cause error', f'{type(self.cause_error).__name__} - {self.cause_error}')
         if self.message:
             yield self._format_info('Message', self.message)
 
     def _get_view_info(self) -> Generator[str, None, None]:
         yield self._get_separator('View info')
         for i, view_info in enumerate(self.view_infos):
             yield '{0}Line {1} in "{2}"'.format(i * '\t', view_info.line, view_info.view)
@@ -69,16 +67,18 @@
     @staticmethod
     def _get_separator(title: str):
         count = 100 - len(title)
         return f'{linesep}{title} {count * "-"}'
 
 
 @contextmanager
-def error_handling(error_to_raise: Union[PyViewsError, Type[PyViewsError]],
-                   add_error_info: Optional[Callable[[PyViewsError], None]] = None):
+def error_handling(
+    error_to_raise: Union[PyViewsError, Type[PyViewsError]],
+    add_error_info: Optional[Callable[[PyViewsError], None]] = None
+):
     """handles error and raises PyViewsError with custom error info"""
     add_error_info = add_error_info if add_error_info is not None else _do_nothing
     try:
         yield
     except PyViewsError as error:
         add_error_info(error)
         raise
```

### Comparing `pyviews-3.2.0/pyviews/core/reflection.py` & `pyviews-4.0.0/pyviews/core/reflection.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """Import in runtime by fullname"""
 
 from importlib import import_module
+from typing import Any, Tuple
 
 
-def import_path(path):
+def import_path(path: str) -> Any:
     """Imports module, class, function by full name"""
     try:
         return import_module(path)
     except ImportError:
         return _import_module_entry(path)
     except BaseException as exc:
         raise ImportError(path) from exc
 
 
-def _import_module_entry(path):
+def _import_module_entry(path: str) -> Any:
     (module, name) = _split_by_last_dot(path)
     try:
         module = import_module(module)
         return module.__dict__[name]
     except BaseException as exc:
         raise ImportError(path) from exc
 
 
-def _split_by_last_dot(expr):
+def _split_by_last_dot(expr: str) -> Tuple[str, str]:
     last_dot = expr.rfind('.')
     if last_dot == -1:
-        return expr, None
+        return expr, ''
     return expr[:last_dot], expr[last_dot + 1:]
```

### Comparing `pyviews-3.2.0/pyviews/core/xml.py` & `pyviews-4.0.0/pyviews/core/xml.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Xml parsing"""
 
-# pylint:disable=wrong-import-order
 from collections import namedtuple
-from typing import List, Optional, Tuple, NamedTuple, Generator
-from xml.parsers.expat import ParserCreate, ExpatError
+from typing import Generator, List, NamedTuple, Optional, Tuple, cast
+from xml.parsers.expat import ExpatError, ParserCreate, XMLParserType
 
-from .error import PyViewsError, ViewInfo
+from injectool import dependency
+
+from pyviews.core.error import PyViewsError, ViewInfo
 
 
 class XmlAttr(NamedTuple):
     """Parsed xml attribute"""
     name: str
     value: Optional[str] = None
     namespace: Optional[str] = None
@@ -33,16 +34,16 @@
 Element = namedtuple('Element', ['node', 'namespaces'])
 
 
 class Parser:
     """Wrapper under xml.parsers.expat for parsing xml files"""
 
     def __init__(self):
-        self._parser = None
-        self._root = None
+        self._parser: XMLParserType = cast(XMLParserType, None)
+        self._root: XmlNode = cast(XmlNode, None)
         self._elements: List[Element] = []
         self._namespaces = {}
         self._view_name = None
 
     def parse(self, xml_file, view_name: Optional[str] = None) -> XmlNode:
         """Parses xml file with xml_path and returns XmlNode"""
         self._setup_parser()
@@ -54,15 +55,15 @@
 
         root = self._root
         self._reset()
         return root
 
     def _setup_parser(self):
         self._parser = ParserCreate()
-        self._parser.ordered_attributes = 1
+        self._parser.ordered_attributes = True
         self._parser.buffer_text = True
 
         self._parser.StartElementHandler = self._start_element
         self._parser.EndElementHandler = self._end_element
         self._parser.CharacterDataHandler = self._set_text
 
     def _start_element(self, full_name: str, keys: List[str]):
@@ -78,15 +79,15 @@
 
     def _create_xml_node(self, full_name: str, attrs: List[ElementAttr]) -> XmlNode:
         (namespace, name) = self._get_namespace_and_name(full_name, True)
         value_attrs = list(self._get_attributes(attrs))
         view_info = ViewInfo(self._view_name, self._parser.CurrentLineNumber)
         return XmlNode(namespace, name, '', [], value_attrs, view_info)
 
-    def _get_namespace_and_name(self, full_name: str, use_default=False) -> Tuple[str, str]:
+    def _get_namespace_and_name(self, full_name: str, use_default = False) -> Tuple[Optional[str], str]:
         if ':' in full_name:
             return self._split(full_name)
         namespace = self._get_default_namespace() if use_default else None
         return namespace, full_name
 
     def _split(self, full_name: str) -> Tuple[str, str]:
         parts = full_name.split(':')
@@ -129,18 +130,22 @@
         except IndexError:
             self._root = node
 
     def _set_text(self, text):
         if text:
             item = self._elements[-1]
             # noinspection PyProtectedMember
-            node = item.node._replace(text=text)
+            node = item.node._replace(text = text)
             self._elements[-1] = Element(node, item.namespaces)
 
     def _reset(self):
-        self._parser = None
-        self._root = None
+        self._parser = cast(XMLParserType, None)
+        self._root = cast(XmlNode, None)
         self._elements = []
         self._namespaces = {}
 
     def _get_view_info(self):
         return ViewInfo(self._view_name, self._parser.CurrentLineNumber)
+
+@dependency
+def parse(xml_file, view_name: Optional[str] = None) -> XmlNode:
+    return Parser().parse(xml_file, view_name)
```

### Comparing `pyviews-3.2.0/pyviews/pipes.py` & `pyviews-4.0.0/pyviews/pipes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Common rendering pipes"""
 
-from typing import Callable, Optional
+from typing import Any, Callable, Optional
 
 from injectool import resolve
 
-from pyviews.binding import Binder, BindingContext
-from pyviews.core import Node, XmlAttr, import_path, XmlNode, Setter
-from pyviews.expression import is_expression, parse_expression
-from pyviews.rendering import RenderingContext, render
+from pyviews.binding.binder import Binder, BindingContext
+from pyviews.core.expression import is_expression, parse_expression
+from pyviews.core.reflection import import_path
+from pyviews.core.rendering import Node, RenderingContext, Setter
+from pyviews.core.xml import XmlAttr, XmlNode
+from pyviews.rendering.pipeline import render
 
 
 def apply_attributes(node: Node, _: RenderingContext):
     """Rendering pipe: applies xml attributes to instance node and setups bindings"""
     for attr in node.xml_node.attrs:
         apply_attribute(node, attr)
 
@@ -19,38 +21,35 @@
 def apply_attribute(node: Node, attr: XmlAttr, setter: Optional[Setter] = None):
     """Maps xml attribute to instance node property and setups bindings"""
     setter = get_setter(attr) if setter is None else setter
     stripped_value = attr.value.strip() if attr.value else ''
     if is_expression(stripped_value):
         (binding_type, expr_body) = parse_expression(stripped_value)
         binder = resolve(Binder)
-        binder.bind(binding_type, BindingContext({
-            'node': node,
-            'expression_body': expr_body,
-            'setter': setter,
-            'xml_attr': attr
-        }))
+        binder.bind(
+            binding_type,
+            BindingContext({'node': node, 'expression_body': expr_body, 'setter': setter, 'xml_attr': attr})
+        )
     else:
         setter(node, attr.name, attr.value)
 
 
 def get_setter(attr: XmlAttr) -> Setter:
     """Returns setter for xml attribute"""
     if attr.namespace is None:
         return call_set_attr
     return import_path(attr.namespace)
 
 
-def call_set_attr(node: Node, key: str, value):
+def call_set_attr(node: Node, key: str, value: Any):
     """Setter: calls node setter"""
     node.set_attr(key, value)
 
 
 GetChildContextType = Callable[[XmlNode, Node, RenderingContext], RenderingContext]
 
 
-def render_children(node: Node, context: RenderingContext,
-                    get_child_context: GetChildContextType):
+def render_children(node: Node, context: RenderingContext, get_child_context: GetChildContextType):
     """renders node children"""
     for xml_node in node.xml_node.children:
         child_node = render(get_child_context(xml_node, node, context))
         node.add_child(child_node)
```

### Comparing `pyviews-3.2.0/pyviews/presenter.py` & `pyviews-4.0.0/pyviews/presenter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Presenter"""
 
 from abc import ABC
-from typing import Dict, Union
+from typing import Dict, Optional, Union
 
-from pyviews.core import XmlNode, InheritedDict, Node
-from pyviews.core.rendering import InstanceNode
+from pyviews.core.rendering import InstanceNode, Node, NodeGlobals, RenderingContext
+from pyviews.core.xml import XmlNode
 from pyviews.pipes import apply_attributes, render_children
-from pyviews.rendering import RenderingPipeline, RenderingContext, get_child_context
+from pyviews.rendering.context import get_child_context
+from pyviews.rendering.pipeline import RenderingPipeline
 
 
 class Presenter(ABC):
     """Base class for presenters"""
 
     def __init__(self):
         self._references: Dict[str, Union[Node, InstanceNode]] = {}
@@ -22,35 +23,33 @@
     def on_rendered(self):
         """called when child nodes are rendered"""
 
 
 class PresenterNode(InstanceNode):
     """Presenter node"""
 
-    def __init__(self, instance: 'Presenter', xml_node: XmlNode,
-                 node_globals: InheritedDict = None):
-        super().__init__(instance, xml_node, node_globals=node_globals)
+    def __init__(self, instance: Optional['Presenter'], xml_node: XmlNode, node_globals: Optional[NodeGlobals] = None):
+        super().__init__(instance, xml_node, node_globals = node_globals)
 
     @property
     def instance(self) -> Presenter:
         return self._instance
 
     @instance.setter
     def instance(self, value: Presenter):
         self._instance = value
 
 
 def get_presenter_pipeline() -> RenderingPipeline:
     """Returns setup for PresenterNode"""
-    return RenderingPipeline(pipes=[
-        apply_attributes,
-        add_presenter_to_globals,
-        render_presenter_children,
-        call_on_rendered
-    ], create_node=create_presenter_node, name='presenter pipeline')
+    return RenderingPipeline(
+        pipes = [apply_attributes, add_presenter_to_globals, render_presenter_children, call_on_rendered],
+        create_node = create_presenter_node,
+        name = 'presenter pipeline'
+    )
 
 
 def add_presenter_to_globals(node: PresenterNode, _: RenderingContext):
     """Adds presenter instance to globals with 'presenter' key"""
     node.node_globals['presenter'] = node.instance
 
 
@@ -62,14 +61,14 @@
 def render_presenter_children(node, context: RenderingContext):
     """Renders container children"""
     render_children(node, context, get_child_context)
 
 
 def create_presenter_node(context: RenderingContext) -> PresenterNode:
     """Create presenter node"""
-    return PresenterNode(None, context.xml_node, node_globals=context.node_globals)
+    return PresenterNode(None, context.xml_node, node_globals = context.node_globals)
 
 
 def add_reference(node: Node, _: str, value: str):
     """Adds node reference to presenter"""
     presenter: Presenter = node.node_globals['presenter']
     presenter.add_reference(value, node)
```

### Comparing `pyviews-3.2.0/pyviews/rendering/pipeline.py` & `pyviews-4.0.0/pyviews/rendering/pipeline.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 """Rendering pipeline. Node creation from xml node, attribute setup and binding creation"""
 
 from importlib import import_module
-from inspect import signature, Parameter
-from typing import Generic, List, Callable, Optional, TypeVar, Union, Type, Tuple, Dict, Any, cast, Collection
+from inspect import Parameter, signature
+from typing import Any, Callable, Collection, Dict, Generic, List, Optional, Tuple, Type, TypeVar, Union
 
-from injectool import resolve, DependencyError, dependency, SingletonResolver, get_container
+from injectool import DependencyError, add_singleton, dependency, resolve
 
-from pyviews.core import Node, InstanceNode, XmlNode
-from .common import RenderingContext, RenderingError, use_context
-from ..core.error import error_handling, PyViewsError
+from pyviews.core.error import PyViewsError, ViewInfo, error_handling
+from pyviews.core.rendering import InstanceNode, Node, RenderingContext, RenderingError
+from pyviews.core.xml import XmlNode
+from pyviews.rendering.context import use_context
+from pyviews.rendering.views import ViewError, get_view_root
 
-
-N = TypeVar('N', bound=Node)
-RC = TypeVar('RC', bound=RenderingContext)
+N = TypeVar('N', bound = Node)
+RC = TypeVar('RC', bound = RenderingContext)
 Pipe = Callable[[N, RC], None]
 CreateNode = Callable[[RC], N]
 
+
 class RenderingPipeline(Generic[N, RC]):
     """Creates and renders node"""
-    def __init__(self, pipes: Optional[List[Pipe[N, RC]]] = None,
-                 create_node: Optional[CreateNode[RC, N]] = None,
-                 name: Optional[str] = None):
+
+    def __init__(
+        self,
+        pipes: Optional[List[Pipe[N, RC]]] = None,
+        create_node: Optional[CreateNode[RC, N]] = None,
+        name: Optional[str] = None
+    ):
         self._name: Optional[str] = name
         self._pipes: List[Callable[[N, RC], None]] = pipes if pipes else []
         self._create_node: CreateNode = create_node if create_node else _create_node
 
     def run(self, context: RenderingContext) -> N:
         """Runs pipeline"""
         pipe: Optional[Pipe] = None
@@ -78,49 +84,55 @@
     except KeyError as key_error:
         msg_format = 'parameter with key "{0}" is not found in node args'
         raise RenderingError(msg_format.format(key_error.args[0])) from key_error
     return args, kwargs
 
 
 def _get_positional_args(parameters: Collection[Parameter], param_values: dict) -> List[Any]:
-    keys = [p.name for p in parameters
-            if p.kind in [Parameter.POSITIONAL_ONLY, Parameter.POSITIONAL_OR_KEYWORD]
-            and p.default == Parameter.empty]
+    keys = [
+        p.name for p in parameters
+        if p.kind in [Parameter.POSITIONAL_ONLY, Parameter.POSITIONAL_OR_KEYWORD] and p.default == Parameter.empty
+    ]
     return [param_values[key] for key in keys]
 
 
 def _get_optional_args(parameters: List[Parameter], param_values: dict) -> dict:
-    keys = [p.name for p in parameters
-            if p.kind in [Parameter.KEYWORD_ONLY, Parameter.POSITIONAL_OR_KEYWORD]
-            and p.default != Parameter.empty
-            and p.name in param_values]
+    keys = [
+        p.name for p in parameters if p.kind in [Parameter.KEYWORD_ONLY, Parameter.POSITIONAL_OR_KEYWORD]
+        and p.default != Parameter.empty and p.name in param_values
+    ]
     return {key: param_values[key] for key in keys}
 
 
 def get_pipeline(xml_node: XmlNode) -> RenderingPipeline:
     """Resolves pipeline by namespace and name or by namespace"""
     key = f'{xml_node.namespace}.{xml_node.name}'
     try:
-        return resolve(RenderingPipeline, key)
+        return resolve((RenderingPipeline, key))
     except DependencyError:
         try:
-            return resolve(RenderingPipeline, xml_node.namespace)
+            return resolve((RenderingPipeline, xml_node.namespace))
         except DependencyError as error:
             render_error = RenderingError('RenderingPipeline is not found')
             render_error.add_info('Used keys to resolve pipeline', f'{key}, {xml_node.namespace}')
             raise render_error from error
 
 
 @dependency
+def render_view(view_name: str, context: RenderingContext) -> Node:
+    """Renders view"""
+    with error_handling(ViewError, lambda e: e.add_view_info(ViewInfo(view_name, None))):
+        context.xml_node = get_view_root(view_name)
+        return render(context)
+
+
+@dependency
 def render(context: RenderingContext) -> Node:
     """Renders node from xml node"""
     with error_handling(RenderingError, lambda e: e.add_view_info(context.xml_node.view_info)):
         pipeline = get_pipeline(context.xml_node)
         return pipeline.run(context)
 
 
-def use_pipeline(pipeline: RenderingPipeline, class_path: str, resolver: Optional[SingletonResolver] = None):
+def use_pipeline(pipeline: RenderingPipeline, class_path: str):
     """Adds rendering pipeline for class path"""
-    if resolver is None:
-        container = get_container()
-        resolver = cast(SingletonResolver, container.get_resolver(RenderingPipeline))
-    resolver.set_value(pipeline, class_path)
+    add_singleton((RenderingPipeline, class_path), pipeline)
```

### Comparing `pyviews-3.2.0/pyviews/rendering/views.py` & `pyviews-4.0.0/pyviews/rendering/views.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,34 @@
 """View logic"""
 
 from os.path import join
 
-from injectool import resolve, dependency
+from injectool import resolve
 
-from pyviews.core import PyViewsError, ViewInfo, Node
-from pyviews.core.xml import Parser, XmlNode
-from .common import RenderingContext
-from .pipeline import render
-from ..core.error import error_handling
+from pyviews.core.error import PyViewsError
+from pyviews.core.xml import XmlNode, parse
 
 
 class ViewError(PyViewsError):
     """Common error for parsing exceptions"""
 
 
-@dependency
-def render_view(view_name: str, context: RenderingContext) -> Node:
-    """Renders view"""
-    with error_handling(ViewError,
-                        lambda e: e.add_view_info(ViewInfo(view_name, None))):
-        context.xml_node = get_view_root(view_name)
-        return render(context)
-
-
 _XML_CACHE = {}
 
 
 def get_view_root(view_name: str) -> XmlNode:
     """Parses xml file and return root XmlNode"""
     path = join(resolve('views_folder'), f'{view_name}.{resolve("view_ext")}')
     if path not in _XML_CACHE:
-        _parse_root(path, view_name)
+        parse_root(path, view_name)
     return _XML_CACHE[path]
 
 
-def _parse_root(path, view_name):
+def parse_root(path: str, view_name: str):
     try:
-        parser = Parser()
         with open(path, 'rb') as xml_file:
-            _XML_CACHE[path] = parser.parse(xml_file, view_name)
+            _XML_CACHE[path] = parse(xml_file, view_name)
     except FileNotFoundError as exc:
         error = ViewError('View is not found')
         error.add_info('View name', view_name)
         error.add_info('Path', path)
         raise error from exc
```

### Comparing `pyviews-3.2.0/pyviews/setters.py` & `pyviews-4.0.0/pyviews/setters.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Module with setters"""
 
-from typing import Any, NamedTuple, Iterable, Union
+from typing import Any, Iterable, NamedTuple, Union
 
 from injectool import resolve
 
-from pyviews.core import Node, import_path, InstanceNode
+from pyviews.core.reflection import import_path
+from pyviews.core.rendering import InstanceNode, Node
 
 
 def import_global(node: Node, key: str, path: Any):
     """Import passed module, class, function full name and stores it to node's globals"""
     node.node_globals[key] = import_path(path)
 
 
@@ -33,9 +34,9 @@
     """Returns Args tuple from parameters"""
     return Args(args_, kwargs)
 
 
 def call(node: Union[InstanceNode, Node], key: str, value: Args):
     """Calls node or node instance method"""
     target = node if hasattr(node, key) else \
-            node.instance if isinstance(node, InstanceNode) else node
+             node.instance if isinstance(node, InstanceNode) else node
     getattr(target, key)(*value.args, **value.kwargs)
```

### Comparing `pyviews-3.2.0/pyviews.egg-info/PKG-INFO` & `pyviews-4.0.0/pyviews.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyviews
-Version: 3.2.0
+Version: 4.0.0
 Summary: Base package for xml views
 Project-URL: Homepage, https://github.com/eumis/pyviews
 Keywords: binding,pyviews,python,mvvm,tkviews,wxviews
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
```

