# Comparing `tmp/sf-hamilton-1.9.0.tar.gz` & `tmp/sf-hamilton-1.9.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sf-hamilton-1.9.0.tar", last modified: Thu Jul 14 22:54:33 2022, max compression
+gzip compressed data, was "sf-hamilton-1.9.0rc0.tar", last modified: Wed Jul 13 21:28:33 2022, max compression
```

## Comparing `sf-hamilton-1.9.0.tar` & `sf-hamilton-1.9.0rc0.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-14 22:54:33.134707 sf-hamilton-1.9.0/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5502 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1886 2022-04-17 04:29:36.000000 sf-hamilton-1.9.0/CONTRIBUTING.md
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1612 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/LICENSE
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)       84 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/MANIFEST.in
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)    12258 2022-07-14 22:54:33.134277 sf-hamilton-1.9.0/PKG-INFO
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)    11035 2022-07-14 22:49:42.000000 sf-hamilton-1.9.0/README.md
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6918 2022-04-17 04:29:36.000000 sf-hamilton-1.9.0/basics.md
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5198 2022-07-14 22:49:42.000000 sf-hamilton-1.9.0/data_quality.md
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)    12472 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0/decorators.md
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3908 2022-07-03 00:06:31.000000 sf-hamilton-1.9.0/developer_setup.md
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-14 22:54:33.111415 sf-hamilton-1.9.0/graph_adapter_tests/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2022-05-31 21:09:37.000000 sf-hamilton-1.9.0/graph_adapter_tests/__init__.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-14 22:54:33.111635 sf-hamilton-1.9.0/graph_adapter_tests/h_dask/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_dask/__init__.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-14 22:54:33.116447 sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      571 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/bad_functions.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-14 22:54:33.116961 sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/config/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/config/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      111 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/config/default_config.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)       47 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/config/default_config_2.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      143 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/config/user_specified_config.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      405 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/config_modifier.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      525 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/cyclic_functions.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      741 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/data_quality.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3443 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/dq_dummy_examples.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      715 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/dummy_functions.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      301 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/example_module.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      306 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/extract_column_nodes.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      467 2022-04-17 04:29:36.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/extract_columns_execution_count.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      447 2022-04-17 04:29:36.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/functions_with_generics.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1356 2022-05-31 21:09:31.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/layered_decorators.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      195 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/only_import_me.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      998 2022-07-03 00:06:31.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/optional_dependencies.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1955 2022-04-17 04:29:36.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/parametrized_inputs.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      300 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/parametrized_nodes.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      258 2022-05-31 21:09:31.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/tagging.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      393 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/test_default_args.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      915 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/typing_vs_not_typing.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)       35 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/very_simple_dag.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1306 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_dask/test_h_dask.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-14 22:54:33.117394 sf-hamilton-1.9.0/graph_adapter_tests/h_ray/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_ray/__init__.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-14 22:54:33.119603 sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      571 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/bad_functions.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-14 22:54:33.120031 sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/config/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/config/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      111 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/config/default_config.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)       47 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/config/default_config_2.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      143 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/config/user_specified_config.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      405 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/config_modifier.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      525 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/cyclic_functions.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      741 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/data_quality.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3443 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/dq_dummy_examples.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      715 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/dummy_functions.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      301 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/example_module.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      306 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/extract_column_nodes.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      467 2022-04-17 04:29:36.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/extract_columns_execution_count.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      447 2022-04-17 04:29:36.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/functions_with_generics.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1356 2022-05-31 21:09:31.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/layered_decorators.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      195 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/only_import_me.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      998 2022-07-03 00:06:31.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/optional_dependencies.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1955 2022-04-17 04:29:36.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/parametrized_inputs.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      300 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/parametrized_nodes.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      258 2022-05-31 21:09:31.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/tagging.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      393 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/test_default_args.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      915 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/typing_vs_not_typing.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)       35 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/very_simple_dag.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1173 2022-05-31 21:09:37.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_ray/test_h_ray.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1269 2022-07-03 00:06:31.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_ray/test_h_ray_workflow.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-14 22:54:33.120416 sf-hamilton-1.9.0/graph_adapter_tests/h_spark/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)       57 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_spark/__init__.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-14 22:54:33.122937 sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      571 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/bad_functions.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-14 22:54:33.123325 sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/config/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/config/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      111 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/config/default_config.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)       47 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/config/default_config_2.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      143 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/config/user_specified_config.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      405 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/config_modifier.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      525 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/cyclic_functions.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      741 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/data_quality.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3443 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/dq_dummy_examples.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      715 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/dummy_functions.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      301 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/example_module.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      306 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/extract_column_nodes.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      467 2022-04-17 04:29:36.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/extract_columns_execution_count.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      447 2022-04-17 04:29:36.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/functions_with_generics.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1356 2022-05-31 21:09:31.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/layered_decorators.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      195 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/only_import_me.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      998 2022-07-03 00:06:31.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/optional_dependencies.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1955 2022-04-17 04:29:36.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/parametrized_inputs.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      300 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/parametrized_nodes.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      258 2022-05-31 21:09:31.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/tagging.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      393 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/test_default_args.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      915 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/typing_vs_not_typing.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)       35 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/very_simple_dag.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1523 2022-07-03 00:06:31.000000 sf-hamilton-1.9.0/graph_adapter_tests/h_spark/test_h_spark.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-14 22:54:33.126224 sf-hamilton-1.9.0/hamilton/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/hamilton/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2353 2022-07-04 21:09:35.000000 sf-hamilton-1.9.0/hamilton/ad_hoc_utils.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     7039 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0/hamilton/base.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-14 22:54:33.126967 sf-hamilton-1.9.0/hamilton/data_quality/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0/hamilton/data_quality/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4937 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0/hamilton/data_quality/base.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)    16891 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0/hamilton/data_quality/default_validators.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3061 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0/hamilton/data_quality/pandera_validators.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)    14835 2022-07-03 00:06:31.000000 sf-hamilton-1.9.0/hamilton/driver.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-14 22:54:33.127947 sf-hamilton-1.9.0/hamilton/experimental/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      314 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/hamilton/experimental/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5025 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/hamilton/experimental/h_dask.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6915 2022-05-31 21:09:37.000000 sf-hamilton-1.9.0/hamilton/experimental/h_ray.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5217 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/hamilton/experimental/h_spark.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)    42100 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0/hamilton/function_modifiers.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)    12400 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0/hamilton/function_modifiers_base.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)    23133 2022-07-03 00:06:31.000000 sf-hamilton-1.9.0/hamilton/graph.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      927 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/hamilton/log_setup.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2469 2022-06-02 22:14:26.000000 sf-hamilton-1.9.0/hamilton/models.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5973 2022-06-02 22:14:10.000000 sf-hamilton-1.9.0/hamilton/node.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)       20 2022-07-14 22:49:42.000000 sf-hamilton-1.9.0/hamilton/version.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)       36 2022-07-03 00:06:31.000000 sf-hamilton-1.9.0/requirements-test.txt
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)       64 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/requirements.txt
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)       38 2022-07-14 22:54:33.135220 sf-hamilton-1.9.0/setup.cfg
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3034 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0/setup.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-14 22:54:33.128940 sf-hamilton-1.9.0/sf_hamilton.egg-info/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)    12258 2022-07-14 22:54:33.000000 sf-hamilton-1.9.0/sf_hamilton.egg-info/PKG-INFO
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6342 2022-07-14 22:54:33.000000 sf-hamilton-1.9.0/sf_hamilton.egg-info/SOURCES.txt
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        1 2022-07-14 22:54:33.000000 sf-hamilton-1.9.0/sf_hamilton.egg-info/dependency_links.txt
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        1 2022-07-13 21:28:32.000000 sf-hamilton-1.9.0/sf_hamilton.egg-info/not-zip-safe
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      358 2022-07-14 22:54:33.000000 sf-hamilton-1.9.0/sf_hamilton.egg-info/requires.txt
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)       35 2022-07-14 22:54:33.000000 sf-hamilton-1.9.0/sf_hamilton.egg-info/top_level.txt
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-14 22:54:33.107600 sf-hamilton-1.9.0/tests/
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-14 22:54:33.131432 sf-hamilton-1.9.0/tests/resources/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/tests/resources/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      571 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/tests/resources/bad_functions.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-14 22:54:33.132400 sf-hamilton-1.9.0/tests/resources/config/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/tests/resources/config/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      111 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/tests/resources/config/default_config.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)       47 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/tests/resources/config/default_config_2.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      143 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/tests/resources/config/user_specified_config.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      405 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/tests/resources/config_modifier.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      525 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/tests/resources/cyclic_functions.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      741 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0/tests/resources/data_quality.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3443 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0/tests/resources/dq_dummy_examples.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      715 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/tests/resources/dummy_functions.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      301 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/tests/resources/example_module.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      306 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/tests/resources/extract_column_nodes.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      467 2022-04-17 04:29:36.000000 sf-hamilton-1.9.0/tests/resources/extract_columns_execution_count.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      447 2022-04-17 04:29:36.000000 sf-hamilton-1.9.0/tests/resources/functions_with_generics.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1356 2022-05-31 21:09:31.000000 sf-hamilton-1.9.0/tests/resources/layered_decorators.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      195 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/tests/resources/only_import_me.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      998 2022-07-03 00:06:31.000000 sf-hamilton-1.9.0/tests/resources/optional_dependencies.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1955 2022-04-17 04:29:36.000000 sf-hamilton-1.9.0/tests/resources/parametrized_inputs.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      300 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/tests/resources/parametrized_nodes.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      258 2022-05-31 21:09:31.000000 sf-hamilton-1.9.0/tests/resources/tagging.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      393 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/tests/resources/test_default_args.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      915 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/tests/resources/typing_vs_not_typing.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)       35 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0/tests/resources/very_simple_dag.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-13 21:28:33.032377 sf-hamilton-1.9.0rc0/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5502 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1886 2022-04-17 04:29:36.000000 sf-hamilton-1.9.0rc0/CONTRIBUTING.md
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1612 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/LICENSE
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       84 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/MANIFEST.in
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)    12262 2022-07-13 21:28:33.032158 sf-hamilton-1.9.0rc0/PKG-INFO
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)    11036 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0rc0/README.md
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6918 2022-04-17 04:29:36.000000 sf-hamilton-1.9.0rc0/basics.md
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5210 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0rc0/data_quality.md
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)    12472 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0rc0/decorators.md
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3908 2022-07-03 00:06:31.000000 sf-hamilton-1.9.0rc0/developer_setup.md
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-13 21:28:33.011866 sf-hamilton-1.9.0rc0/graph_adapter_tests/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2022-05-31 21:09:37.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/__init__.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-13 21:28:33.012069 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/__init__.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-13 21:28:33.016620 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      571 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/bad_functions.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-13 21:28:33.017133 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/config/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/config/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      111 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/config/default_config.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       47 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/config/default_config_2.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      143 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/config/user_specified_config.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      405 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/config_modifier.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      525 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/cyclic_functions.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      741 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/data_quality.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3443 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/dq_dummy_examples.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      715 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/dummy_functions.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      301 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/example_module.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      306 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/extract_column_nodes.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      467 2022-04-17 04:29:36.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/extract_columns_execution_count.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      447 2022-04-17 04:29:36.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/functions_with_generics.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1356 2022-05-31 21:09:31.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/layered_decorators.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      195 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/only_import_me.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      998 2022-07-03 00:06:31.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/optional_dependencies.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1955 2022-04-17 04:29:36.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/parametrized_inputs.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      300 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/parametrized_nodes.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      258 2022-05-31 21:09:31.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/tagging.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      393 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/test_default_args.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      915 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/typing_vs_not_typing.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       35 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/very_simple_dag.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1306 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/test_h_dask.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-13 21:28:33.017582 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/__init__.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-13 21:28:33.020034 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      571 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/bad_functions.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-13 21:28:33.020570 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/config/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/config/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      111 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/config/default_config.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       47 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/config/default_config_2.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      143 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/config/user_specified_config.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      405 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/config_modifier.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      525 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/cyclic_functions.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      741 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/data_quality.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3443 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/dq_dummy_examples.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      715 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/dummy_functions.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      301 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/example_module.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      306 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/extract_column_nodes.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      467 2022-04-17 04:29:36.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/extract_columns_execution_count.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      447 2022-04-17 04:29:36.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/functions_with_generics.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1356 2022-05-31 21:09:31.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/layered_decorators.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      195 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/only_import_me.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      998 2022-07-03 00:06:31.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/optional_dependencies.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1955 2022-04-17 04:29:36.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/parametrized_inputs.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      300 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/parametrized_nodes.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      258 2022-05-31 21:09:31.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/tagging.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      393 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/test_default_args.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      915 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/typing_vs_not_typing.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       35 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/very_simple_dag.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1173 2022-05-31 21:09:37.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/test_h_ray.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1269 2022-07-03 00:06:31.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/test_h_ray_workflow.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-13 21:28:33.020991 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       57 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/__init__.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-13 21:28:33.023750 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      571 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/bad_functions.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-13 21:28:33.024211 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/config/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/config/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      111 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/config/default_config.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       47 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/config/default_config_2.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      143 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/config/user_specified_config.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      405 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/config_modifier.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      525 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/cyclic_functions.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      741 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/data_quality.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3443 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/dq_dummy_examples.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      715 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/dummy_functions.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      301 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/example_module.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      306 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/extract_column_nodes.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      467 2022-04-17 04:29:36.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/extract_columns_execution_count.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      447 2022-04-17 04:29:36.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/functions_with_generics.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1356 2022-05-31 21:09:31.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/layered_decorators.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      195 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/only_import_me.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      998 2022-07-03 00:06:31.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/optional_dependencies.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1955 2022-04-17 04:29:36.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/parametrized_inputs.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      300 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/parametrized_nodes.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      258 2022-05-31 21:09:31.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/tagging.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      393 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/test_default_args.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      915 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/typing_vs_not_typing.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       35 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/very_simple_dag.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1523 2022-07-03 00:06:31.000000 sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/test_h_spark.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-13 21:28:33.026900 sf-hamilton-1.9.0rc0/hamilton/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/hamilton/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2353 2022-07-04 21:09:35.000000 sf-hamilton-1.9.0rc0/hamilton/ad_hoc_utils.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     7039 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0rc0/hamilton/base.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-13 21:28:33.027442 sf-hamilton-1.9.0rc0/hamilton/data_quality/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0rc0/hamilton/data_quality/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4937 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0rc0/hamilton/data_quality/base.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)    16891 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0rc0/hamilton/data_quality/default_validators.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3061 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0rc0/hamilton/data_quality/pandera_validators.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)    14835 2022-07-03 00:06:31.000000 sf-hamilton-1.9.0rc0/hamilton/driver.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-13 21:28:33.028409 sf-hamilton-1.9.0rc0/hamilton/experimental/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      314 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/hamilton/experimental/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5025 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/hamilton/experimental/h_dask.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6915 2022-05-31 21:09:37.000000 sf-hamilton-1.9.0rc0/hamilton/experimental/h_ray.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5217 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/hamilton/experimental/h_spark.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)    42100 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0rc0/hamilton/function_modifiers.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)    12400 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0rc0/hamilton/function_modifiers_base.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)    23133 2022-07-03 00:06:31.000000 sf-hamilton-1.9.0rc0/hamilton/graph.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      927 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/hamilton/log_setup.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2469 2022-06-02 22:14:26.000000 sf-hamilton-1.9.0rc0/hamilton/models.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5973 2022-06-02 22:14:10.000000 sf-hamilton-1.9.0rc0/hamilton/node.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       27 2022-07-13 21:28:20.000000 sf-hamilton-1.9.0rc0/hamilton/version.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       36 2022-07-03 00:06:31.000000 sf-hamilton-1.9.0rc0/requirements-test.txt
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       64 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/requirements.txt
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       38 2022-07-13 21:28:33.032421 sf-hamilton-1.9.0rc0/setup.cfg
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3034 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0rc0/setup.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-13 21:28:33.029534 sf-hamilton-1.9.0rc0/sf_hamilton.egg-info/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)    12262 2022-07-13 21:28:32.000000 sf-hamilton-1.9.0rc0/sf_hamilton.egg-info/PKG-INFO
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6342 2022-07-13 21:28:33.000000 sf-hamilton-1.9.0rc0/sf_hamilton.egg-info/SOURCES.txt
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        1 2022-07-13 21:28:32.000000 sf-hamilton-1.9.0rc0/sf_hamilton.egg-info/dependency_links.txt
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        1 2022-07-13 21:28:32.000000 sf-hamilton-1.9.0rc0/sf_hamilton.egg-info/not-zip-safe
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      358 2022-07-13 21:28:32.000000 sf-hamilton-1.9.0rc0/sf_hamilton.egg-info/requires.txt
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       35 2022-07-13 21:28:32.000000 sf-hamilton-1.9.0rc0/sf_hamilton.egg-info/top_level.txt
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-13 21:28:33.008646 sf-hamilton-1.9.0rc0/tests/
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-13 21:28:33.031540 sf-hamilton-1.9.0rc0/tests/resources/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/tests/resources/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      571 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/tests/resources/bad_functions.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2022-07-13 21:28:33.031911 sf-hamilton-1.9.0rc0/tests/resources/config/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/tests/resources/config/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      111 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/tests/resources/config/default_config.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       47 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/tests/resources/config/default_config_2.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      143 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/tests/resources/config/user_specified_config.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      405 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/tests/resources/config_modifier.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      525 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/tests/resources/cyclic_functions.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      741 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0rc0/tests/resources/data_quality.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3443 2022-07-13 21:25:30.000000 sf-hamilton-1.9.0rc0/tests/resources/dq_dummy_examples.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      715 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/tests/resources/dummy_functions.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      301 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/tests/resources/example_module.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      306 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/tests/resources/extract_column_nodes.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      467 2022-04-17 04:29:36.000000 sf-hamilton-1.9.0rc0/tests/resources/extract_columns_execution_count.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      447 2022-04-17 04:29:36.000000 sf-hamilton-1.9.0rc0/tests/resources/functions_with_generics.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1356 2022-05-31 21:09:31.000000 sf-hamilton-1.9.0rc0/tests/resources/layered_decorators.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      195 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/tests/resources/only_import_me.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      998 2022-07-03 00:06:31.000000 sf-hamilton-1.9.0rc0/tests/resources/optional_dependencies.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1955 2022-04-17 04:29:36.000000 sf-hamilton-1.9.0rc0/tests/resources/parametrized_inputs.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      300 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/tests/resources/parametrized_nodes.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      258 2022-05-31 21:09:31.000000 sf-hamilton-1.9.0rc0/tests/resources/tagging.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      393 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/tests/resources/test_default_args.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      915 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/tests/resources/typing_vs_not_typing.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       35 2022-04-16 15:59:56.000000 sf-hamilton-1.9.0rc0/tests/resources/very_simple_dag.py
```

### Comparing `sf-hamilton-1.9.0/CODE_OF_CONDUCT.md` & `sf-hamilton-1.9.0rc0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/CONTRIBUTING.md` & `sf-hamilton-1.9.0rc0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/LICENSE` & `sf-hamilton-1.9.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/PKG-INFO` & `sf-hamilton-1.9.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sf-hamilton
-Version: 1.9.0
+Version: 1.9.0rc0
 Summary: Hamilton, the micro-framework for creating dataframes.
 Home-page: https://github.com/stitchfix/hamilton
 Author: Stefan Krawczyk, Elijah ben Izzy
 Author-email: skrawczyk@stitchfix.com,elijah.benizzy@stitchfix.com
 Project-URL: Bug Reports, https://github.com/stitchfix/hamilton/issues
 Project-URL: Source, https://github.com/stitchfix/hamilton
 Keywords: hamilton
@@ -164,15 +164,15 @@
 
 ![hello_world_image](hello_world_image.png)
 
 Congratulations - you just created your Hamilton dataflow that created a dataframe!
 
 ## Example Hamilton Dataflows
 We have a growing list of examples showcasing how one might use Hamilton. You can find them all under the [`examples/`](https://github.com/stitchfix/hamilton/tree/main/examples) directory.
-E.g.
+E.g. 
 
 * [Hello world](https://github.com/stitchfix/hamilton/tree/main/examples/hello_world)
 * Scaling on to [Ray](https://github.com/stitchfix/hamilton/tree/main/examples/ray), [Dask](https://github.com/stitchfix/hamilton/tree/main/examples/dask), or [Pandas on Spark](https://github.com/stitchfix/hamilton/tree/main/examples/spark)
 * Training [a model with scikit-learn](https://github.com/stitchfix/hamilton/tree/main/examples/model_examples)
 * Doing [air quality analysis solely in numpy](https://github.com/stitchfix/hamilton/tree/main/examples/numpy/air-quality-analysis)
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: sf-hamilton Version: 1.9.0 Summary: Hamilton, the
-micro-framework for creating dataframes. Home-page: https://github.com/
+Metadata-Version: 2.1 Name: sf-hamilton Version: 1.9.0rc0 Summary: Hamilton,
+the micro-framework for creating dataframes. Home-page: https://github.com/
 stitchfix/hamilton Author: Stefan Krawczyk, Elijah ben Izzy Author-email:
 skrawczyk@stitchfix.com,elijah.benizzy@stitchfix.com Project-URL: Bug Reports,
 https://github.com/stitchfix/hamilton/issues Project-URL: Source, https://
 github.com/stitchfix/hamilton Keywords: hamilton Classifier: Development Status
 :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: License :: OSI Approved ::
 BSD License Classifier: Programming Language :: Python :: 3 Classifier:
```

### Comparing `sf-hamilton-1.9.0/README.md` & `sf-hamilton-1.9.0rc0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 
 ![hello_world_image](hello_world_image.png)
 
 Congratulations - you just created your Hamilton dataflow that created a dataframe!
 
 ## Example Hamilton Dataflows
 We have a growing list of examples showcasing how one might use Hamilton. You can find them all under the [`examples/`](https://github.com/stitchfix/hamilton/tree/main/examples) directory.
-E.g.
+E.g. 
 
 * [Hello world](https://github.com/stitchfix/hamilton/tree/main/examples/hello_world)
 * Scaling on to [Ray](https://github.com/stitchfix/hamilton/tree/main/examples/ray), [Dask](https://github.com/stitchfix/hamilton/tree/main/examples/dask), or [Pandas on Spark](https://github.com/stitchfix/hamilton/tree/main/examples/spark)
 * Training [a model with scikit-learn](https://github.com/stitchfix/hamilton/tree/main/examples/model_examples)
 * Doing [air quality analysis solely in numpy](https://github.com/stitchfix/hamilton/tree/main/examples/numpy/air-quality-analysis)
```

### Comparing `sf-hamilton-1.9.0/basics.md` & `sf-hamilton-1.9.0rc0/basics.md`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/data_quality.md` & `sf-hamilton-1.9.0rc0/data_quality.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,18 +18,17 @@
 ```
 
 In the above, we run two assertions:
 
 1. That the series has an np.int64 datatype
 2. That every item in the series in between 0 and 100
 
-
+```suggestion
 Furthermore, the workflow does not fail when this dies. Rather, it logs a warning, as specified by the value provided to `importance`. In terms of how this works, if you were to visualize what was being executed (e.g. using `visualize_exection()`) then you'd see extra nodes added to the DAG. So when using `@check_output` an extra computational step will be added to your workflow to run that check.
 
-
 ## Design
 
 To add data quality validation, we run an additional computational step in your workflow after function calculation.
 See comments on the `BaseDataValidationDecorator` class for how it works.
 
 ## Default Validators
```

### Comparing `sf-hamilton-1.9.0/decorators.md` & `sf-hamilton-1.9.0rc0/decorators.md`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/developer_setup.md` & `sf-hamilton-1.9.0rc0/developer_setup.md`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/bad_functions.py` & `sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/bad_functions.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/cyclic_functions.py` & `sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/cyclic_functions.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/data_quality.py` & `sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/data_quality.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/dq_dummy_examples.py` & `sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/dq_dummy_examples.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/dummy_functions.py` & `sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/dummy_functions.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/layered_decorators.py` & `sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/layered_decorators.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/optional_dependencies.py` & `sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/optional_dependencies.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/parametrized_inputs.py` & `sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/parametrized_inputs.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/graph_adapter_tests/h_dask/resources/typing_vs_not_typing.py` & `sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/resources/typing_vs_not_typing.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/graph_adapter_tests/h_dask/test_h_dask.py` & `sf-hamilton-1.9.0rc0/graph_adapter_tests/h_dask/test_h_dask.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/bad_functions.py` & `sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/bad_functions.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/cyclic_functions.py` & `sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/cyclic_functions.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/data_quality.py` & `sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/data_quality.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/dq_dummy_examples.py` & `sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/dq_dummy_examples.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/dummy_functions.py` & `sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/dummy_functions.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/layered_decorators.py` & `sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/layered_decorators.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/optional_dependencies.py` & `sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/optional_dependencies.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/parametrized_inputs.py` & `sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/parametrized_inputs.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/graph_adapter_tests/h_ray/resources/typing_vs_not_typing.py` & `sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/resources/typing_vs_not_typing.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/graph_adapter_tests/h_ray/test_h_ray.py` & `sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/test_h_ray.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/graph_adapter_tests/h_ray/test_h_ray_workflow.py` & `sf-hamilton-1.9.0rc0/graph_adapter_tests/h_ray/test_h_ray_workflow.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/bad_functions.py` & `sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/bad_functions.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/cyclic_functions.py` & `sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/cyclic_functions.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/data_quality.py` & `sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/data_quality.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/dq_dummy_examples.py` & `sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/dq_dummy_examples.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/dummy_functions.py` & `sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/dummy_functions.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/layered_decorators.py` & `sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/layered_decorators.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/optional_dependencies.py` & `sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/optional_dependencies.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/parametrized_inputs.py` & `sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/parametrized_inputs.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/graph_adapter_tests/h_spark/resources/typing_vs_not_typing.py` & `sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/resources/typing_vs_not_typing.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/graph_adapter_tests/h_spark/test_h_spark.py` & `sf-hamilton-1.9.0rc0/graph_adapter_tests/h_spark/test_h_spark.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/hamilton/ad_hoc_utils.py` & `sf-hamilton-1.9.0rc0/hamilton/ad_hoc_utils.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/hamilton/base.py` & `sf-hamilton-1.9.0rc0/hamilton/base.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/hamilton/data_quality/base.py` & `sf-hamilton-1.9.0rc0/hamilton/data_quality/base.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/hamilton/data_quality/default_validators.py` & `sf-hamilton-1.9.0rc0/hamilton/data_quality/default_validators.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/hamilton/data_quality/pandera_validators.py` & `sf-hamilton-1.9.0rc0/hamilton/data_quality/pandera_validators.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/hamilton/driver.py` & `sf-hamilton-1.9.0rc0/hamilton/driver.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/hamilton/experimental/h_dask.py` & `sf-hamilton-1.9.0rc0/hamilton/experimental/h_dask.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/hamilton/experimental/h_ray.py` & `sf-hamilton-1.9.0rc0/hamilton/experimental/h_ray.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/hamilton/experimental/h_spark.py` & `sf-hamilton-1.9.0rc0/hamilton/experimental/h_spark.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/hamilton/function_modifiers.py` & `sf-hamilton-1.9.0rc0/hamilton/function_modifiers.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/hamilton/function_modifiers_base.py` & `sf-hamilton-1.9.0rc0/hamilton/function_modifiers_base.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/hamilton/graph.py` & `sf-hamilton-1.9.0rc0/hamilton/graph.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/hamilton/log_setup.py` & `sf-hamilton-1.9.0rc0/hamilton/log_setup.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/hamilton/models.py` & `sf-hamilton-1.9.0rc0/hamilton/models.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/hamilton/node.py` & `sf-hamilton-1.9.0rc0/hamilton/node.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/setup.py` & `sf-hamilton-1.9.0rc0/setup.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/sf_hamilton.egg-info/PKG-INFO` & `sf-hamilton-1.9.0rc0/sf_hamilton.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sf-hamilton
-Version: 1.9.0
+Version: 1.9.0rc0
 Summary: Hamilton, the micro-framework for creating dataframes.
 Home-page: https://github.com/stitchfix/hamilton
 Author: Stefan Krawczyk, Elijah ben Izzy
 Author-email: skrawczyk@stitchfix.com,elijah.benizzy@stitchfix.com
 Project-URL: Bug Reports, https://github.com/stitchfix/hamilton/issues
 Project-URL: Source, https://github.com/stitchfix/hamilton
 Keywords: hamilton
@@ -164,15 +164,15 @@
 
 ![hello_world_image](hello_world_image.png)
 
 Congratulations - you just created your Hamilton dataflow that created a dataframe!
 
 ## Example Hamilton Dataflows
 We have a growing list of examples showcasing how one might use Hamilton. You can find them all under the [`examples/`](https://github.com/stitchfix/hamilton/tree/main/examples) directory.
-E.g.
+E.g. 
 
 * [Hello world](https://github.com/stitchfix/hamilton/tree/main/examples/hello_world)
 * Scaling on to [Ray](https://github.com/stitchfix/hamilton/tree/main/examples/ray), [Dask](https://github.com/stitchfix/hamilton/tree/main/examples/dask), or [Pandas on Spark](https://github.com/stitchfix/hamilton/tree/main/examples/spark)
 * Training [a model with scikit-learn](https://github.com/stitchfix/hamilton/tree/main/examples/model_examples)
 * Doing [air quality analysis solely in numpy](https://github.com/stitchfix/hamilton/tree/main/examples/numpy/air-quality-analysis)
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: sf-hamilton Version: 1.9.0 Summary: Hamilton, the
-micro-framework for creating dataframes. Home-page: https://github.com/
+Metadata-Version: 2.1 Name: sf-hamilton Version: 1.9.0rc0 Summary: Hamilton,
+the micro-framework for creating dataframes. Home-page: https://github.com/
 stitchfix/hamilton Author: Stefan Krawczyk, Elijah ben Izzy Author-email:
 skrawczyk@stitchfix.com,elijah.benizzy@stitchfix.com Project-URL: Bug Reports,
 https://github.com/stitchfix/hamilton/issues Project-URL: Source, https://
 github.com/stitchfix/hamilton Keywords: hamilton Classifier: Development Status
 :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: License :: OSI Approved ::
 BSD License Classifier: Programming Language :: Python :: 3 Classifier:
```

### Comparing `sf-hamilton-1.9.0/sf_hamilton.egg-info/SOURCES.txt` & `sf-hamilton-1.9.0rc0/sf_hamilton.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/tests/resources/bad_functions.py` & `sf-hamilton-1.9.0rc0/tests/resources/bad_functions.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/tests/resources/cyclic_functions.py` & `sf-hamilton-1.9.0rc0/tests/resources/cyclic_functions.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/tests/resources/data_quality.py` & `sf-hamilton-1.9.0rc0/tests/resources/data_quality.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/tests/resources/dq_dummy_examples.py` & `sf-hamilton-1.9.0rc0/tests/resources/dq_dummy_examples.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/tests/resources/dummy_functions.py` & `sf-hamilton-1.9.0rc0/tests/resources/dummy_functions.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/tests/resources/layered_decorators.py` & `sf-hamilton-1.9.0rc0/tests/resources/layered_decorators.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/tests/resources/optional_dependencies.py` & `sf-hamilton-1.9.0rc0/tests/resources/optional_dependencies.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/tests/resources/parametrized_inputs.py` & `sf-hamilton-1.9.0rc0/tests/resources/parametrized_inputs.py`

 * *Files identical despite different names*

### Comparing `sf-hamilton-1.9.0/tests/resources/typing_vs_not_typing.py` & `sf-hamilton-1.9.0rc0/tests/resources/typing_vs_not_typing.py`

 * *Files identical despite different names*

