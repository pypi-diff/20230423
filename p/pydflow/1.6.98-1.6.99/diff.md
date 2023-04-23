# Comparing `tmp/pydflow-1.6.98.tar.gz` & `tmp/pydflow-1.6.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydflow-1.6.98.tar", last modified: Tue Mar 28 04:07:48 2023, max compression
+gzip compressed data, was "pydflow-1.6.99.tar", last modified: Tue Mar 28 10:11:02 2023, max compression
```

## Comparing `pydflow-1.6.98.tar` & `pydflow-1.6.99.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 04:07:48.859172 pydflow-1.6.98/
--rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-03-28 04:07:40.000000 pydflow-1.6.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    36305 2023-03-28 04:07:48.859172 pydflow-1.6.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35995 2023-03-28 04:07:40.000000 pydflow-1.6.98/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 04:07:48.859172 pydflow-1.6.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-03-28 04:07:40.000000 pydflow-1.6.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 04:07:48.851172 pydflow-1.6.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 04:07:48.851172 pydflow-1.6.98/src/dflow/
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/argo_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 04:07:48.855172 pydflow-1.6.98/src/dflow/client/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17690 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/client/v1alpha1_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/client/v1alpha1_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/client/v1alpha1_retry_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/client/v1alpha1_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/client/v1alpha1_value_from.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/context_syntax.py
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    48414 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    21452 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/op_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 04:07:48.855172 pydflow-1.6.98/src/dflow/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/plugins/bohrium.py
--rw-r--r--   0 runner    (1001) docker     (123)    20216 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/plugins/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/plugins/lebesgue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/plugins/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/plugins/oss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/plugins/ray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 04:07:48.855172 pydflow-1.6.98/src/dflow/python/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8641 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/python/op.py
--rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/python/opio.py
--rw-r--r--   0 runner    (1001) docker     (123)    29578 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/python/python_op_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    12004 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/python/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    16413 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)    96089 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/util_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    26034 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    42148 2023-03-28 04:07:40.000000 pydflow-1.6.98/src/dflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 04:07:48.855172 pydflow-1.6.98/src/pydflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36305 2023-03-28 04:07:48.000000 pydflow-1.6.98/src/pydflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-03-28 04:07:48.000000 pydflow-1.6.98/src/pydflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 04:07:48.000000 pydflow-1.6.98/src/pydflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-28 04:07:48.000000 pydflow-1.6.98/src/pydflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-28 04:07:48.000000 pydflow-1.6.98/src/pydflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-28 04:07:48.000000 pydflow-1.6.98/src/pydflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 04:07:48.855172 pydflow-1.6.98/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-03-28 04:07:40.000000 pydflow-1.6.98/tests/test_big_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-03-28 04:07:40.000000 pydflow-1.6.98/tests/test_conditional_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-03-28 04:07:40.000000 pydflow-1.6.98/tests/test_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-03-28 04:07:40.000000 pydflow-1.6.98/tests/test_group_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-03-28 04:07:40.000000 pydflow-1.6.98/tests/test_makevasp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-03-28 04:07:40.000000 pydflow-1.6.98/tests/test_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-03-28 04:07:40.000000 pydflow-1.6.98/tests/test_recurse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-03-28 04:07:40.000000 pydflow-1.6.98/tests/test_reuse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-03-28 04:07:40.000000 pydflow-1.6.98/tests/test_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-03-28 04:07:40.000000 pydflow-1.6.98/tests/test_subpath_slices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:11:02.899428 pydflow-1.6.99/
+-rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-03-28 10:10:52.000000 pydflow-1.6.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    36305 2023-03-28 10:11:02.899428 pydflow-1.6.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35995 2023-03-28 10:10:52.000000 pydflow-1.6.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 10:11:02.899428 pydflow-1.6.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-03-28 10:10:52.000000 pydflow-1.6.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:11:02.891428 pydflow-1.6.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:11:02.895428 pydflow-1.6.99/src/dflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/argo_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:11:02.895428 pydflow-1.6.99/src/dflow/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17690 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/client/v1alpha1_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/client/v1alpha1_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/client/v1alpha1_retry_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/client/v1alpha1_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/client/v1alpha1_value_from.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/context_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48414 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21452 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/op_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:11:02.895428 pydflow-1.6.99/src/dflow/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14475 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/plugins/bohrium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20216 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/plugins/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/plugins/lebesgue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/plugins/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/plugins/oss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/plugins/ray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:11:02.895428 pydflow-1.6.99/src/dflow/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8641 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/python/op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/python/opio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29578 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/python/python_op_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12004 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/python/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16413 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96089 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/util_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26096 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42148 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:11:02.895428 pydflow-1.6.99/src/pydflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    36305 2023-03-28 10:11:02.000000 pydflow-1.6.99/src/pydflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-03-28 10:11:02.000000 pydflow-1.6.99/src/pydflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 10:11:02.000000 pydflow-1.6.99/src/pydflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-28 10:11:02.000000 pydflow-1.6.99/src/pydflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-28 10:11:02.000000 pydflow-1.6.99/src/pydflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-28 10:11:02.000000 pydflow-1.6.99/src/pydflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:11:02.899428 pydflow-1.6.99/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-03-28 10:10:52.000000 pydflow-1.6.99/tests/test_big_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-03-28 10:10:52.000000 pydflow-1.6.99/tests/test_conditional_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-03-28 10:10:52.000000 pydflow-1.6.99/tests/test_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-03-28 10:10:52.000000 pydflow-1.6.99/tests/test_group_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-03-28 10:10:52.000000 pydflow-1.6.99/tests/test_makevasp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-03-28 10:10:52.000000 pydflow-1.6.99/tests/test_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-03-28 10:10:52.000000 pydflow-1.6.99/tests/test_recurse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-03-28 10:10:52.000000 pydflow-1.6.99/tests/test_reuse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-03-28 10:10:52.000000 pydflow-1.6.99/tests/test_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-03-28 10:10:52.000000 pydflow-1.6.99/tests/test_subpath_slices.py
```

### Comparing `pydflow-1.6.98/LICENSE` & `pydflow-1.6.99/LICENSE`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/PKG-INFO` & `pydflow-1.6.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydflow
-Version: 1.6.98
+Version: 1.6.99
 Summary: Dflow is a Python framework for constructing scientific computing workflows employing Argo Workflows as the workflow engine.
 Author: Xinzijian Liu
 License: LGPLv3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pydflow-1.6.98/README.md` & `pydflow-1.6.99/README.md`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/setup.py` & `pydflow-1.6.99/setup.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/src/dflow/__init__.py` & `pydflow-1.6.99/src/dflow/__init__.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/src/dflow/argo_objects.py` & `pydflow-1.6.99/src/dflow/argo_objects.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/src/dflow/client/v1alpha1_artifact.py` & `pydflow-1.6.99/src/dflow/client/v1alpha1_artifact.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/src/dflow/client/v1alpha1_parameter.py` & `pydflow-1.6.99/src/dflow/client/v1alpha1_parameter.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/src/dflow/client/v1alpha1_retry_strategy.py` & `pydflow-1.6.99/src/dflow/client/v1alpha1_retry_strategy.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/src/dflow/client/v1alpha1_sequence.py` & `pydflow-1.6.99/src/dflow/client/v1alpha1_sequence.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/src/dflow/client/v1alpha1_value_from.py` & `pydflow-1.6.99/src/dflow/client/v1alpha1_value_from.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/src/dflow/common.py` & `pydflow-1.6.99/src/dflow/common.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/src/dflow/config.py` & `pydflow-1.6.99/src/dflow/config.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/src/dflow/context_syntax.py` & `pydflow-1.6.99/src/dflow/context_syntax.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/src/dflow/dag.py` & `pydflow-1.6.99/src/dflow/dag.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/src/dflow/executor.py` & `pydflow-1.6.99/src/dflow/executor.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/src/dflow/io.py` & `pydflow-1.6.99/src/dflow/io.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/src/dflow/main.py` & `pydflow-1.6.99/src/dflow/main.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/src/dflow/op_template.py` & `pydflow-1.6.99/src/dflow/op_template.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/src/dflow/plugins/bohrium.py` & `pydflow-1.6.99/src/dflow/plugins/bohrium.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,15 +334,16 @@
                     client = tiefblue.Client(base_url=self.tiefblue_url,
                                              token=self.token)
                     res = client.list(prefix=prefix, recursive=recursive,
                                       next_token=next_token)
                 else:
                     raise e
             for obj in res["objects"]:
-                if recursive and obj["path"][-1:] == "/":
+                if (recursive or obj["path"] == prefix) and \
+                        obj["path"].endswith("/"):
                     continue
                 keys.append(obj["path"])
             if not res["hasNext"]:
                 break
             next_token = res["nextToken"]
         return keys
```

### Comparing `pydflow-1.6.98/src/dflow/plugins/dispatcher.py` & `pydflow-1.6.99/src/dflow/plugins/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/src/dflow/plugins/lebesgue.py` & `pydflow-1.6.99/src/dflow/plugins/lebesgue.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/src/dflow/plugins/metadata.py` & `pydflow-1.6.99/src/dflow/plugins/metadata.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/src/dflow/plugins/oss.py` & `pydflow-1.6.99/src/dflow/plugins/oss.py`

 * *Files 13% similar despite different names*

```diff
@@ -52,14 +52,16 @@
                 marker = r.next_marker
         else:
             marker = ""
             while True:
                 r = self.bucket.list_objects(prefix, delimiter="/",
                                              marker=marker)
                 for obj in r.object_list:
+                    if obj.key == prefix and obj.key.endswith("/"):
+                        continue
                     keys.append(obj.key)
                 for key in r.prefix_list:
                     keys.append(key)
                 if not r.is_truncated:
                     break
                 marker = r.next_marker
         return keys
```

### Comparing `pydflow-1.6.98/src/dflow/plugins/ray.py` & `pydflow-1.6.99/src/dflow/plugins/ray.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/src/dflow/python/op.py` & `pydflow-1.6.99/src/dflow/python/op.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/src/dflow/python/opio.py` & `pydflow-1.6.99/src/dflow/python/opio.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/src/dflow/python/python_op_template.py` & `pydflow-1.6.99/src/dflow/python/python_op_template.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/src/dflow/python/utils.py` & `pydflow-1.6.99/src/dflow/python/utils.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/src/dflow/resource.py` & `pydflow-1.6.99/src/dflow/resource.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/src/dflow/slurm.py` & `pydflow-1.6.99/src/dflow/slurm.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/src/dflow/step.py` & `pydflow-1.6.99/src/dflow/step.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/src/dflow/steps.py` & `pydflow-1.6.99/src/dflow/steps.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/src/dflow/task.py` & `pydflow-1.6.99/src/dflow/task.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/src/dflow/util_ops.py` & `pydflow-1.6.99/src/dflow/util_ops.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/src/dflow/utils.py` & `pydflow-1.6.99/src/dflow/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,15 @@
 
     if slice is not None:
         sub_path = path_list_of_artifact(artifact)[slice]
         key = key + "/" + sub_path
         path = os.path.join(path, os.path.dirname(sub_path))
         download_s3(key=key, recursive=True, path=path, keep_dir=True,
                     **kwargs)
+        path = os.path.join(path, os.path.basename(sub_path))
         remove_empty_dir_tag(path)
         return path
 
     path = download_s3(key=key, recursive=True, path=path, **kwargs)
     if key[-4:] == ".tgz" and extract:
         path = os.path.join(path, os.path.basename(key))
         tf = tarfile.open(path, "r:gz")
```

### Comparing `pydflow-1.6.98/src/dflow/workflow.py` & `pydflow-1.6.99/src/dflow/workflow.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/src/pydflow.egg-info/PKG-INFO` & `pydflow-1.6.99/src/pydflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydflow
-Version: 1.6.98
+Version: 1.6.99
 Summary: Dflow is a Python framework for constructing scientific computing workflows employing Argo Workflows as the workflow engine.
 Author: Xinzijian Liu
 License: LGPLv3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pydflow-1.6.98/src/pydflow.egg-info/SOURCES.txt` & `pydflow-1.6.99/src/pydflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/tests/test_big_parameter.py` & `pydflow-1.6.99/tests/test_big_parameter.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/tests/test_conditional_outputs.py` & `pydflow-1.6.99/tests/test_conditional_outputs.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/tests/test_dag.py` & `pydflow-1.6.99/tests/test_dag.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/tests/test_group_size.py` & `pydflow-1.6.99/tests/test_group_size.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/tests/test_makevasp.py` & `pydflow-1.6.99/tests/test_makevasp.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/tests/test_python.py` & `pydflow-1.6.99/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/tests/test_recurse.py` & `pydflow-1.6.99/tests/test_recurse.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/tests/test_reuse.py` & `pydflow-1.6.99/tests/test_reuse.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/tests/test_slices.py` & `pydflow-1.6.99/tests/test_slices.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.98/tests/test_subpath_slices.py` & `pydflow-1.6.99/tests/test_subpath_slices.py`

 * *Files identical despite different names*

