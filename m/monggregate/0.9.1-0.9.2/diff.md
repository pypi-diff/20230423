# Comparing `tmp/monggregate-0.9.1.tar.gz` & `tmp/monggregate-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monggregate-0.9.1.tar", last modified: Thu Dec 29 21:55:25 2022, max compression
+gzip compressed data, was "monggregate-0.9.2.tar", last modified: Thu Dec 29 21:58:06 2022, max compression
```

## Comparing `monggregate-0.9.1.tar` & `monggregate-0.9.2.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxrwxrwx   0        0        0        0 2022-12-29 21:55:25.580356 monggregate-0.9.1/
--rw-rw-rw-   0        0        0     1086 2022-12-29 15:05:31.000000 monggregate-0.9.1/LICENSE
--rw-rw-rw-   0        0        0     7017 2022-12-29 21:55:25.575959 monggregate-0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     4840 2022-12-29 21:54:19.000000 monggregate-0.9.1/README.md
-drwxrwxrwx   0        0        0        0 2022-12-29 21:55:24.193839 monggregate-0.9.1/monggregate/
--rw-rw-rw-   0        0        0      394 2022-12-29 21:54:55.000000 monggregate-0.9.1/monggregate/__init__.py
--rw-rw-rw-   0        0        0     1840 2022-12-29 14:43:41.000000 monggregate-0.9.1/monggregate/base.py
-drwxrwxrwx   0        0        0        0 2022-12-29 21:55:24.282825 monggregate-0.9.1/monggregate/expressions/
--rw-rw-rw-   0        0        0     3392 2022-12-29 14:43:41.000000 monggregate-0.9.1/monggregate/expressions/__init__.py
--rw-rw-rw-   0        0        0      614 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/expressions/aggregation_variables.py
--rw-rw-rw-   0        0        0      519 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/expressions/content.py
--rw-rw-rw-   0        0        0    10782 2022-12-29 14:43:41.000000 monggregate-0.9.1/monggregate/expressions/expressions.py
--rw-rw-rw-   0        0        0      662 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/expressions/fields.py
--rw-rw-rw-   0        0        0     5173 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/index.py
-drwxrwxrwx   0        0        0        0 2022-12-29 21:55:24.302825 monggregate-0.9.1/monggregate/operators/
--rw-rw-rw-   0        0        0     1252 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-29 21:55:24.460482 monggregate-0.9.1/monggregate/operators/accumulators/
--rw-rw-rw-   0        0        0      556 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/accumulators/__init__.py
--rw-rw-rw-   0        0        0     1121 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/accumulators/accumulator.py
--rw-rw-rw-   0        0        0     2919 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/accumulators/avg.py
--rw-rw-rw-   0        0        0     1855 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/accumulators/count.py
--rw-rw-rw-   0        0        0     2421 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/accumulators/first.py
--rw-rw-rw-   0        0        0     2116 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/accumulators/last.py
--rw-rw-rw-   0        0        0     3119 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/accumulators/max.py
--rw-rw-rw-   0        0        0     3084 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/accumulators/min.py
--rw-rw-rw-   0        0        0     1300 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/accumulators/push.py
--rw-rw-rw-   0        0        0     3714 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/accumulators/sum.py
-drwxrwxrwx   0        0        0        0 2022-12-29 21:55:24.711506 monggregate-0.9.1/monggregate/operators/array/
--rw-rw-rw-   0        0        0      698 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/array/__init__.py
--rw-rw-rw-   0        0        0     3112 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/array/array.py
--rw-rw-rw-   0        0        0     2361 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/array/array_to_object.py
--rw-rw-rw-   0        0        0     4043 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/array/filter.py
--rw-rw-rw-   0        0        0     3657 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/array/first.py
--rw-rw-rw-   0        0        0     1874 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/array/in_.py
--rw-rw-rw-   0        0        0     1447 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/array/is_array.py
--rw-rw-rw-   0        0        0     3892 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/array/last.py
--rw-rw-rw-   0        0        0     2421 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/array/max_n.py
--rw-rw-rw-   0        0        0     2420 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/array/min_n.py
--rw-rw-rw-   0        0        0     1323 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/array/size.py
--rw-rw-rw-   0        0        0     3573 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/array/sort_array.py
-drwxrwxrwx   0        0        0        0 2022-12-29 21:55:24.767354 monggregate-0.9.1/monggregate/operators/boolean/
--rw-rw-rw-   0        0        0      204 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/boolean/__init__.py
--rw-rw-rw-   0        0        0     2464 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/boolean/and_.py
--rw-rw-rw-   0        0        0     1071 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/boolean/boolean.py
--rw-rw-rw-   0        0        0     1473 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/boolean/not_.py
--rw-rw-rw-   0        0        0     1540 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/boolean/or_.py
-drwxrwxrwx   0        0        0        0 2022-12-29 21:55:24.867374 monggregate-0.9.1/monggregate/operators/comparison/
--rw-rw-rw-   0        0        0      621 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/comparison/__init__.py
--rw-rw-rw-   0        0        0     1490 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/comparison/cmp.py
--rw-rw-rw-   0        0        0     1306 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/comparison/comparator.py
--rw-rw-rw-   0        0        0     1455 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/comparison/eq.py
--rw-rw-rw-   0        0        0     1509 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/comparison/gt.py
--rw-rw-rw-   0        0        0     1520 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/comparison/gte.py
--rw-rw-rw-   0        0        0     1455 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/comparison/lt.py
--rw-rw-rw-   0        0        0     1516 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/comparison/lte.py
--rw-rw-rw-   0        0        0     1470 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/comparison/ne.py
-drwxrwxrwx   0        0        0        0 2022-12-29 21:55:24.909339 monggregate-0.9.1/monggregate/operators/objects/
--rw-rw-rw-   0        0        0      208 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/objects/__init__.py
--rw-rw-rw-   0        0        0     1996 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/objects/merge_objects.py
--rw-rw-rw-   0        0        0     1101 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/objects/object_.py
--rw-rw-rw-   0        0        0     1829 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/objects/object_to_array.py
--rw-rw-rw-   0        0        0      268 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/operators/operator.py
--rw-rw-rw-   0        0        0    22788 2022-12-29 14:43:41.000000 monggregate-0.9.1/monggregate/pipeline.py
-drwxrwxrwx   0        0        0        0 2022-12-29 21:55:25.284198 monggregate-0.9.1/monggregate/stages/
--rw-rw-rw-   0        0        0     1793 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/stages/__init__.py
--rw-rw-rw-   0        0        0     5685 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/stages/bucket.py
--rw-rw-rw-   0        0        0     7206 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/stages/bucket_auto.py
--rw-rw-rw-   0        0        0     1808 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/stages/count.py
--rw-rw-rw-   0        0        0     4275 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/stages/group.py
--rw-rw-rw-   0        0        0     2857 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/stages/limit.py
--rw-rw-rw-   0        0        0    15896 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/stages/lookup.py
--rw-rw-rw-   0        0        0     2755 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/stages/match.py
--rw-rw-rw-   0        0        0     6438 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/stages/out.py
--rw-rw-rw-   0        0        0    10333 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/stages/project.py
--rw-rw-rw-   0        0        0     3994 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/stages/replace_root.py
--rw-rw-rw-   0        0        0     2351 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/stages/sample.py
--rw-rw-rw-   0        0        0     2002 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/stages/set.py
--rw-rw-rw-   0        0        0     3056 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/stages/skip.py
--rw-rw-rw-   0        0        0    10443 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/stages/sort.py
--rw-rw-rw-   0        0        0     2973 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/stages/sort_by_count.py
--rw-rw-rw-   0        0        0     1344 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/stages/stage.py
--rw-rw-rw-   0        0        0     3943 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/stages/unwind.py
--rw-rw-rw-   0        0        0     1953 2022-12-29 14:40:46.000000 monggregate-0.9.1/monggregate/utils.py
-drwxrwxrwx   0        0        0        0 2022-12-29 21:55:24.220900 monggregate-0.9.1/monggregate.egg-info/
--rw-rw-rw-   0        0        0     7017 2022-12-29 21:55:22.000000 monggregate-0.9.1/monggregate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3024 2022-12-29 21:55:23.000000 monggregate-0.9.1/monggregate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-29 21:55:22.000000 monggregate-0.9.1/monggregate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2022-12-29 21:55:23.000000 monggregate-0.9.1/monggregate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-12-29 21:55:23.000000 monggregate-0.9.1/monggregate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1390 2022-12-29 21:54:55.000000 monggregate-0.9.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-12-29 21:55:25.582588 monggregate-0.9.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-12-29 21:55:25.567971 monggregate-0.9.1/test/
--rw-rw-rw-   0        0        0     3222 2022-12-29 14:40:46.000000 monggregate-0.9.1/test/test_docstrings.py
--rw-rw-rw-   0        0        0     1064 2022-12-29 14:40:46.000000 monggregate-0.9.1/test/test_expressions.py
--rw-rw-rw-   0        0        0     3979 2022-12-29 14:40:46.000000 monggregate-0.9.1/test/test_operators_accumulators.py
--rw-rw-rw-   0        0        0     5586 2022-12-29 14:40:46.000000 monggregate-0.9.1/test/test_operators_array.py
--rw-rw-rw-   0        0        0     2346 2022-12-29 14:40:46.000000 monggregate-0.9.1/test/test_operators_boolean.py
--rw-rw-rw-   0        0        0     3237 2022-12-29 14:40:46.000000 monggregate-0.9.1/test/test_operators_comparison.py
--rw-rw-rw-   0        0        0     1257 2022-12-29 14:40:46.000000 monggregate-0.9.1/test/test_operators_objects.py
--rw-rw-rw-   0        0        0      247 2022-12-29 14:40:46.000000 monggregate-0.9.1/test/test_package.py
--rw-rw-rw-   0        0        0      274 2022-12-29 14:40:46.000000 monggregate-0.9.1/test/test_signatures.py
--rw-rw-rw-   0        0        0    17706 2022-12-29 15:06:51.000000 monggregate-0.9.1/test/test_stages.py
+drwxrwxrwx   0        0        0        0 2022-12-29 21:58:06.413267 monggregate-0.9.2/
+-rw-rw-rw-   0        0        0     1086 2022-12-29 15:05:31.000000 monggregate-0.9.2/LICENSE
+-rw-rw-rw-   0        0        0     7022 2022-12-29 21:58:06.412238 monggregate-0.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4845 2022-12-29 21:57:07.000000 monggregate-0.9.2/README.md
+drwxrwxrwx   0        0        0        0 2022-12-29 21:58:06.154053 monggregate-0.9.2/monggregate/
+-rw-rw-rw-   0        0        0      394 2022-12-29 21:57:40.000000 monggregate-0.9.2/monggregate/__init__.py
+-rw-rw-rw-   0        0        0     1840 2022-12-29 14:43:41.000000 monggregate-0.9.2/monggregate/base.py
+drwxrwxrwx   0        0        0        0 2022-12-29 21:58:06.189589 monggregate-0.9.2/monggregate/expressions/
+-rw-rw-rw-   0        0        0     3392 2022-12-29 14:43:41.000000 monggregate-0.9.2/monggregate/expressions/__init__.py
+-rw-rw-rw-   0        0        0      614 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/expressions/aggregation_variables.py
+-rw-rw-rw-   0        0        0      519 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/expressions/content.py
+-rw-rw-rw-   0        0        0    10782 2022-12-29 14:43:41.000000 monggregate-0.9.2/monggregate/expressions/expressions.py
+-rw-rw-rw-   0        0        0      662 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/expressions/fields.py
+-rw-rw-rw-   0        0        0     5173 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/index.py
+drwxrwxrwx   0        0        0        0 2022-12-29 21:58:06.196521 monggregate-0.9.2/monggregate/operators/
+-rw-rw-rw-   0        0        0     1252 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-29 21:58:06.233138 monggregate-0.9.2/monggregate/operators/accumulators/
+-rw-rw-rw-   0        0        0      556 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/accumulators/__init__.py
+-rw-rw-rw-   0        0        0     1121 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/accumulators/accumulator.py
+-rw-rw-rw-   0        0        0     2919 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/accumulators/avg.py
+-rw-rw-rw-   0        0        0     1855 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/accumulators/count.py
+-rw-rw-rw-   0        0        0     2421 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/accumulators/first.py
+-rw-rw-rw-   0        0        0     2116 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/accumulators/last.py
+-rw-rw-rw-   0        0        0     3119 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/accumulators/max.py
+-rw-rw-rw-   0        0        0     3084 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/accumulators/min.py
+-rw-rw-rw-   0        0        0     1300 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/accumulators/push.py
+-rw-rw-rw-   0        0        0     3714 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/accumulators/sum.py
+drwxrwxrwx   0        0        0        0 2022-12-29 21:58:06.278136 monggregate-0.9.2/monggregate/operators/array/
+-rw-rw-rw-   0        0        0      698 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/array/__init__.py
+-rw-rw-rw-   0        0        0     3112 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/array/array.py
+-rw-rw-rw-   0        0        0     2361 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/array/array_to_object.py
+-rw-rw-rw-   0        0        0     4043 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/array/filter.py
+-rw-rw-rw-   0        0        0     3657 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/array/first.py
+-rw-rw-rw-   0        0        0     1874 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/array/in_.py
+-rw-rw-rw-   0        0        0     1447 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/array/is_array.py
+-rw-rw-rw-   0        0        0     3892 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/array/last.py
+-rw-rw-rw-   0        0        0     2421 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/array/max_n.py
+-rw-rw-rw-   0        0        0     2420 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/array/min_n.py
+-rw-rw-rw-   0        0        0     1323 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/array/size.py
+-rw-rw-rw-   0        0        0     3573 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/array/sort_array.py
+drwxrwxrwx   0        0        0        0 2022-12-29 21:58:06.296249 monggregate-0.9.2/monggregate/operators/boolean/
+-rw-rw-rw-   0        0        0      204 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/boolean/__init__.py
+-rw-rw-rw-   0        0        0     2464 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/boolean/and_.py
+-rw-rw-rw-   0        0        0     1071 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/boolean/boolean.py
+-rw-rw-rw-   0        0        0     1473 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/boolean/not_.py
+-rw-rw-rw-   0        0        0     1540 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/boolean/or_.py
+drwxrwxrwx   0        0        0        0 2022-12-29 21:58:06.323621 monggregate-0.9.2/monggregate/operators/comparison/
+-rw-rw-rw-   0        0        0      621 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/comparison/__init__.py
+-rw-rw-rw-   0        0        0     1490 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/comparison/cmp.py
+-rw-rw-rw-   0        0        0     1306 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/comparison/comparator.py
+-rw-rw-rw-   0        0        0     1455 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/comparison/eq.py
+-rw-rw-rw-   0        0        0     1509 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/comparison/gt.py
+-rw-rw-rw-   0        0        0     1520 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/comparison/gte.py
+-rw-rw-rw-   0        0        0     1455 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/comparison/lt.py
+-rw-rw-rw-   0        0        0     1516 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/comparison/lte.py
+-rw-rw-rw-   0        0        0     1470 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/comparison/ne.py
+drwxrwxrwx   0        0        0        0 2022-12-29 21:58:06.334130 monggregate-0.9.2/monggregate/operators/objects/
+-rw-rw-rw-   0        0        0      208 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/objects/__init__.py
+-rw-rw-rw-   0        0        0     1996 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/objects/merge_objects.py
+-rw-rw-rw-   0        0        0     1101 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/objects/object_.py
+-rw-rw-rw-   0        0        0     1829 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/objects/object_to_array.py
+-rw-rw-rw-   0        0        0      268 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/operators/operator.py
+-rw-rw-rw-   0        0        0    22788 2022-12-29 14:43:41.000000 monggregate-0.9.2/monggregate/pipeline.py
+drwxrwxrwx   0        0        0        0 2022-12-29 21:58:06.384815 monggregate-0.9.2/monggregate/stages/
+-rw-rw-rw-   0        0        0     1793 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/stages/__init__.py
+-rw-rw-rw-   0        0        0     5685 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/stages/bucket.py
+-rw-rw-rw-   0        0        0     7206 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/stages/bucket_auto.py
+-rw-rw-rw-   0        0        0     1808 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/stages/count.py
+-rw-rw-rw-   0        0        0     4275 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/stages/group.py
+-rw-rw-rw-   0        0        0     2857 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/stages/limit.py
+-rw-rw-rw-   0        0        0    15896 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/stages/lookup.py
+-rw-rw-rw-   0        0        0     2755 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/stages/match.py
+-rw-rw-rw-   0        0        0     6438 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/stages/out.py
+-rw-rw-rw-   0        0        0    10333 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/stages/project.py
+-rw-rw-rw-   0        0        0     3994 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/stages/replace_root.py
+-rw-rw-rw-   0        0        0     2351 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/stages/sample.py
+-rw-rw-rw-   0        0        0     2002 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/stages/set.py
+-rw-rw-rw-   0        0        0     3056 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/stages/skip.py
+-rw-rw-rw-   0        0        0    10443 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/stages/sort.py
+-rw-rw-rw-   0        0        0     2973 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/stages/sort_by_count.py
+-rw-rw-rw-   0        0        0     1344 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/stages/stage.py
+-rw-rw-rw-   0        0        0     3943 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/stages/unwind.py
+-rw-rw-rw-   0        0        0     1953 2022-12-29 14:40:46.000000 monggregate-0.9.2/monggregate/utils.py
+drwxrwxrwx   0        0        0        0 2022-12-29 21:58:06.171048 monggregate-0.9.2/monggregate.egg-info/
+-rw-rw-rw-   0        0        0     7022 2022-12-29 21:58:05.000000 monggregate-0.9.2/monggregate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3024 2022-12-29 21:58:06.000000 monggregate-0.9.2/monggregate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-12-29 21:58:05.000000 monggregate-0.9.2/monggregate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2022-12-29 21:58:05.000000 monggregate-0.9.2/monggregate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2022-12-29 21:58:05.000000 monggregate-0.9.2/monggregate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1390 2022-12-29 21:57:40.000000 monggregate-0.9.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2022-12-29 21:58:06.414318 monggregate-0.9.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-12-29 21:58:06.409236 monggregate-0.9.2/test/
+-rw-rw-rw-   0        0        0     3222 2022-12-29 14:40:46.000000 monggregate-0.9.2/test/test_docstrings.py
+-rw-rw-rw-   0        0        0     1064 2022-12-29 14:40:46.000000 monggregate-0.9.2/test/test_expressions.py
+-rw-rw-rw-   0        0        0     3979 2022-12-29 14:40:46.000000 monggregate-0.9.2/test/test_operators_accumulators.py
+-rw-rw-rw-   0        0        0     5586 2022-12-29 14:40:46.000000 monggregate-0.9.2/test/test_operators_array.py
+-rw-rw-rw-   0        0        0     2346 2022-12-29 14:40:46.000000 monggregate-0.9.2/test/test_operators_boolean.py
+-rw-rw-rw-   0        0        0     3237 2022-12-29 14:40:46.000000 monggregate-0.9.2/test/test_operators_comparison.py
+-rw-rw-rw-   0        0        0     1257 2022-12-29 14:40:46.000000 monggregate-0.9.2/test/test_operators_objects.py
+-rw-rw-rw-   0        0        0      247 2022-12-29 14:40:46.000000 monggregate-0.9.2/test/test_package.py
+-rw-rw-rw-   0        0        0      274 2022-12-29 14:40:46.000000 monggregate-0.9.2/test/test_signatures.py
+-rw-rw-rw-   0        0        0    17706 2022-12-29 15:06:51.000000 monggregate-0.9.2/test/test_stages.py
```

### Comparing `monggregate-0.9.1/LICENSE` & `monggregate-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/PKG-INFO` & `monggregate-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monggregate
-Version: 0.9.1
+Version: 0.9.2
 Summary: MongoDB aggregation pipelines made easy. Joins, grouping, counting and much more...
 Home-page: https://github.com/VianneyMI/monggregate
 Author-email: Vianney Mixtur <vianney.mixtur@outlook.fr>
 License: The MIT License (MIT)
         Copyright © 2022 Vianney Mixtur
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -54,15 +54,15 @@
 4. Install the repo locally by executing the following command: ` python -m pip install -e .`
 
 ### PIP
 
 The repo is now available on PyPI:
 
 ```shell
-pip install beanie
+pip install monggregate
 ```
 
 ## Usage
 
 The below examples reference the  MongoDB sample_mflix database
 
 ### ... through the stage classes
```

### Comparing `monggregate-0.9.1/README.md` & `monggregate-0.9.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 4. Install the repo locally by executing the following command: ` python -m pip install -e .`
 
 ### PIP
 
 The repo is now available on PyPI:
 
 ```shell
-pip install beanie
+pip install monggregate
 ```
 
 ## Usage
 
 The below examples reference the  MongoDB sample_mflix database
 
 ### ... through the stage classes
```

### Comparing `monggregate-0.9.1/monggregate/base.py` & `monggregate-0.9.2/monggregate/base.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/expressions/__init__.py` & `monggregate-0.9.2/monggregate/expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/expressions/aggregation_variables.py` & `monggregate-0.9.2/monggregate/expressions/aggregation_variables.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/expressions/content.py` & `monggregate-0.9.2/monggregate/expressions/content.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/expressions/expressions.py` & `monggregate-0.9.2/monggregate/expressions/expressions.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/expressions/fields.py` & `monggregate-0.9.2/monggregate/expressions/fields.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/index.py` & `monggregate-0.9.2/monggregate/index.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/__init__.py` & `monggregate-0.9.2/monggregate/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/accumulators/__init__.py` & `monggregate-0.9.2/monggregate/operators/accumulators/__init__.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/accumulators/accumulator.py` & `monggregate-0.9.2/monggregate/operators/accumulators/accumulator.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/accumulators/avg.py` & `monggregate-0.9.2/monggregate/operators/accumulators/avg.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/accumulators/count.py` & `monggregate-0.9.2/monggregate/operators/accumulators/count.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/accumulators/first.py` & `monggregate-0.9.2/monggregate/operators/accumulators/first.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/accumulators/last.py` & `monggregate-0.9.2/monggregate/operators/accumulators/last.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/accumulators/max.py` & `monggregate-0.9.2/monggregate/operators/accumulators/max.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/accumulators/min.py` & `monggregate-0.9.2/monggregate/operators/accumulators/min.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/accumulators/push.py` & `monggregate-0.9.2/monggregate/operators/accumulators/push.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/accumulators/sum.py` & `monggregate-0.9.2/monggregate/operators/accumulators/sum.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/array/__init__.py` & `monggregate-0.9.2/monggregate/operators/array/__init__.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/array/array.py` & `monggregate-0.9.2/monggregate/operators/array/array.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/array/array_to_object.py` & `monggregate-0.9.2/monggregate/operators/array/array_to_object.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/array/filter.py` & `monggregate-0.9.2/monggregate/operators/array/filter.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/array/first.py` & `monggregate-0.9.2/monggregate/operators/array/first.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/array/in_.py` & `monggregate-0.9.2/monggregate/operators/array/in_.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/array/is_array.py` & `monggregate-0.9.2/monggregate/operators/array/is_array.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/array/last.py` & `monggregate-0.9.2/monggregate/operators/array/last.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/array/max_n.py` & `monggregate-0.9.2/monggregate/operators/array/max_n.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/array/min_n.py` & `monggregate-0.9.2/monggregate/operators/array/min_n.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/array/size.py` & `monggregate-0.9.2/monggregate/operators/array/size.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/array/sort_array.py` & `monggregate-0.9.2/monggregate/operators/array/sort_array.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/boolean/and_.py` & `monggregate-0.9.2/monggregate/operators/boolean/and_.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/boolean/boolean.py` & `monggregate-0.9.2/monggregate/operators/boolean/boolean.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/boolean/not_.py` & `monggregate-0.9.2/monggregate/operators/boolean/not_.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/boolean/or_.py` & `monggregate-0.9.2/monggregate/operators/boolean/or_.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/comparison/__init__.py` & `monggregate-0.9.2/monggregate/operators/comparison/__init__.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/comparison/cmp.py` & `monggregate-0.9.2/monggregate/operators/comparison/cmp.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/comparison/comparator.py` & `monggregate-0.9.2/monggregate/operators/comparison/comparator.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/comparison/eq.py` & `monggregate-0.9.2/monggregate/operators/comparison/eq.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/comparison/gt.py` & `monggregate-0.9.2/monggregate/operators/comparison/gt.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/comparison/gte.py` & `monggregate-0.9.2/monggregate/operators/comparison/gte.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/comparison/lt.py` & `monggregate-0.9.2/monggregate/operators/comparison/lt.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/comparison/lte.py` & `monggregate-0.9.2/monggregate/operators/comparison/lte.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/comparison/ne.py` & `monggregate-0.9.2/monggregate/operators/comparison/ne.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/objects/merge_objects.py` & `monggregate-0.9.2/monggregate/operators/objects/merge_objects.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/objects/object_.py` & `monggregate-0.9.2/monggregate/operators/objects/object_.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/operators/objects/object_to_array.py` & `monggregate-0.9.2/monggregate/operators/objects/object_to_array.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/pipeline.py` & `monggregate-0.9.2/monggregate/pipeline.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/stages/__init__.py` & `monggregate-0.9.2/monggregate/stages/__init__.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/stages/bucket.py` & `monggregate-0.9.2/monggregate/stages/bucket.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/stages/bucket_auto.py` & `monggregate-0.9.2/monggregate/stages/bucket_auto.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/stages/count.py` & `monggregate-0.9.2/monggregate/stages/count.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/stages/group.py` & `monggregate-0.9.2/monggregate/stages/group.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/stages/limit.py` & `monggregate-0.9.2/monggregate/stages/limit.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/stages/lookup.py` & `monggregate-0.9.2/monggregate/stages/lookup.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/stages/match.py` & `monggregate-0.9.2/monggregate/stages/match.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/stages/out.py` & `monggregate-0.9.2/monggregate/stages/out.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/stages/project.py` & `monggregate-0.9.2/monggregate/stages/project.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/stages/replace_root.py` & `monggregate-0.9.2/monggregate/stages/replace_root.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/stages/sample.py` & `monggregate-0.9.2/monggregate/stages/sample.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/stages/set.py` & `monggregate-0.9.2/monggregate/stages/set.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/stages/skip.py` & `monggregate-0.9.2/monggregate/stages/skip.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/stages/sort.py` & `monggregate-0.9.2/monggregate/stages/sort.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/stages/sort_by_count.py` & `monggregate-0.9.2/monggregate/stages/sort_by_count.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/stages/stage.py` & `monggregate-0.9.2/monggregate/stages/stage.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/stages/unwind.py` & `monggregate-0.9.2/monggregate/stages/unwind.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate/utils.py` & `monggregate-0.9.2/monggregate/utils.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/monggregate.egg-info/PKG-INFO` & `monggregate-0.9.2/monggregate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monggregate
-Version: 0.9.1
+Version: 0.9.2
 Summary: MongoDB aggregation pipelines made easy. Joins, grouping, counting and much more...
 Home-page: https://github.com/VianneyMI/monggregate
 Author-email: Vianney Mixtur <vianney.mixtur@outlook.fr>
 License: The MIT License (MIT)
         Copyright © 2022 Vianney Mixtur
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -54,15 +54,15 @@
 4. Install the repo locally by executing the following command: ` python -m pip install -e .`
 
 ### PIP
 
 The repo is now available on PyPI:
 
 ```shell
-pip install beanie
+pip install monggregate
 ```
 
 ## Usage
 
 The below examples reference the  MongoDB sample_mflix database
 
 ### ... through the stage classes
```

### Comparing `monggregate-0.9.1/monggregate.egg-info/SOURCES.txt` & `monggregate-0.9.2/monggregate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/pyproject.toml` & `monggregate-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "monggregate"
-version = "0.9.1"
+version = "0.9.2"
 description = "MongoDB aggregation pipelines made easy. Joins, grouping, counting and much more..."
 readme = "README.md"
 authors = [{ name = "Vianney Mixtur", email = "vianney.mixtur@outlook.fr" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -29,15 +29,15 @@
 mongo = ["pymongo >= 3.0.0"]
 dev = ["bumpver", "pytest", "mypy", "pylint"]
 
 [project.urls]
 Homepage = "https://github.com/VianneyMI/monggregate"
 
 [tool.bumpver]
-current_version = "0.9.1"
+current_version = "0.9.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `monggregate-0.9.1/test/test_docstrings.py` & `monggregate-0.9.2/test/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/test/test_expressions.py` & `monggregate-0.9.2/test/test_expressions.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/test/test_operators_accumulators.py` & `monggregate-0.9.2/test/test_operators_accumulators.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/test/test_operators_array.py` & `monggregate-0.9.2/test/test_operators_array.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/test/test_operators_boolean.py` & `monggregate-0.9.2/test/test_operators_boolean.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/test/test_operators_comparison.py` & `monggregate-0.9.2/test/test_operators_comparison.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/test/test_operators_objects.py` & `monggregate-0.9.2/test/test_operators_objects.py`

 * *Files identical despite different names*

### Comparing `monggregate-0.9.1/test/test_stages.py` & `monggregate-0.9.2/test/test_stages.py`

 * *Files identical despite different names*

