# Comparing `tmp/opteryx-0.9.2.tar.gz` & `tmp/opteryx-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opteryx-0.9.2.tar", last modified: Tue Feb 28 12:34:19 2023, max compression
+gzip compressed data, was "opteryx-0.9.3.tar", last modified: Sat Mar  4 12:46:48 2023, max compression
```

## Comparing `opteryx-0.9.2.tar` & `opteryx-0.9.3.tar`

### file list

```diff
@@ -1,213 +1,213 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.056806 opteryx-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-02-28 12:34:02.000000 opteryx-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14897 2023-02-28 12:34:19.056806 opteryx-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14627 2023-02-28 12:34:02.000000 opteryx-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.032806 opteryx-0.9.2/opteryx/
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/attribute_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.036806 opteryx-0.9.2/opteryx/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.036806 opteryx-0.9.2/opteryx/components/binder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/components/binder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/components/binder/binder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.036806 opteryx-0.9.2/opteryx/components/logical_planner/
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/components/logical_planner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19967 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/components/logical_planner/builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/components/logical_planner/custom_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/components/logical_planner/logical_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)    17770 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/components/logical_planner/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/components/query_planner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.036806 opteryx-0.9.2/opteryx/components/sql_rewriter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/components/sql_rewriter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/components/sql_rewriter/sql_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/components/sql_rewriter/temporal_extraction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.036806 opteryx-0.9.2/opteryx/components/tree_rewriter/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/components/tree_rewriter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.036806 opteryx-0.9.2/opteryx/components/tree_rewriter/rules/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/components/tree_rewriter/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/components/tree_rewriter/rules/rule_apply_demorgans_law.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/components/tree_rewriter/rules/rule_constant_evaluations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/components/tree_rewriter/rules/rule_defragment_morsels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/components/tree_rewriter/rules/rule_eliminate_negations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/components/tree_rewriter/rules/rule_function_evaluations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/components/tree_rewriter/rules/rule_move_literal_join_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/components/tree_rewriter/rules/rule_predicate_pushdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/components/tree_rewriter/rules/rule_split_conjunctive_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/components/tree_rewriter/rules/rule_use_heap_sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.036806 opteryx-0.9.2/opteryx/components/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/components/v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.036806 opteryx-0.9.2/opteryx/components/v2/logical_planner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/components/v2/logical_planner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/components/v2/logical_planner/planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9731 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.040806 opteryx-0.9.2/opteryx/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/connectors/arrow_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/connectors/aws_s3_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.040806 opteryx-0.9.2/opteryx/connectors/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/connectors/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/connectors/base/base_blob_storage_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/connectors/base/base_document_storage_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.040806 opteryx-0.9.2/opteryx/connectors/capabilities/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/connectors/capabilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/connectors/capabilities/predicate_pushable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/connectors/disk_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/connectors/gcp_cloudstorage_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/connectors/gcp_firestore_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/connectors/hadro_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/connectors/mongodb_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/connectors/sql_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.040806 opteryx-0.9.2/opteryx/functions/
--rw-r--r--   0 runner    (1001) docker     (123)     9659 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/functions/binary_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/functions/date_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/functions/number_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/functions/other_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6869 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/functions/string_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/functions/unary_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/functions/v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.040806 opteryx-0.9.2/opteryx/managers/
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/managers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.040806 opteryx-0.9.2/opteryx/managers/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/managers/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/managers/cache/memcached.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/managers/cache/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.040806 opteryx-0.9.2/opteryx/managers/expression/
--rw-r--r--   0 runner    (1001) docker     (123)    16220 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/managers/expression/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.040806 opteryx-0.9.2/opteryx/managers/kvstores/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/managers/kvstores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/managers/kvstores/base_kv_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/managers/kvstores/kv_firestore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.040806 opteryx-0.9.2/opteryx/managers/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/managers/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/managers/metadata/data_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.040806 opteryx-0.9.2/opteryx/managers/schemes/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/managers/schemes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/managers/schemes/base_partition_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/managers/schemes/default_partitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/managers/schemes/mabel_partitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.044806 opteryx-0.9.2/opteryx/models/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11280 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/models/columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/models/execution_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/models/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/models/query_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.044806 opteryx-0.9.2/opteryx/operators/
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15060 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/operators/aggregate_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/operators/base_plan_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    15535 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/operators/blob_reader_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/operators/build_statistics_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/operators/collection_reader_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/operators/column_filter_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/operators/cross_join_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/operators/distinct_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/operators/explain_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/operators/file_reader_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/operators/function_dataset_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/operators/heap_sort_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/operators/inner_join_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/operators/internal_dataset_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/operators/limit_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/operators/morsel_defragment_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/operators/offset_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/operators/outer_join_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/operators/projection_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/operators/selection_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    11768 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/operators/show_columns_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/operators/show_create_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/operators/show_functions_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/operators/show_stores_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/operators/show_value_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/operators/show_variables_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/operators/sort_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/operators/sql_reader_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.048806 opteryx-0.9.2/opteryx/samples/
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36761 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/samples/astronaut_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/samples/no_table_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13319 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/samples/planet_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10962 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/samples/satellite_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.048806 opteryx-0.9.2/opteryx/shared/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/shared/buffer_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/shared/materialized_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/shared/query_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.048806 opteryx-0.9.2/opteryx/storage/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.048806 opteryx-0.9.2/opteryx/third_party/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/third_party/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.048806 opteryx-0.9.2/opteryx/third_party/cityhash/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/third_party/cityhash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19319 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/third_party/cityhash/city.cc
--rw-r--r--   0 runner    (1001) docker     (123)   237362 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/third_party/cityhash/cityhash.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/third_party/cityhash/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.048806 opteryx-0.9.2/opteryx/third_party/distogram/
--rw-r--r--   0 runner    (1001) docker     (123)    15445 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/third_party/distogram/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.048806 opteryx-0.9.2/opteryx/third_party/fastlogging/
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/third_party/fastlogging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/third_party/fastlogging/console.py
--rw-r--r--   0 runner    (1001) docker     (123)    21205 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/third_party/fastlogging/fastlogging.py
--rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/third_party/fastlogging/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/third_party/fastlogging/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/third_party/fastlogging/pyorcy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/third_party/fastlogging/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.048806 opteryx-0.9.2/opteryx/third_party/fuzzy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/third_party/fuzzy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   218370 2023-02-28 12:34:17.000000 opteryx-0.9.2/opteryx/third_party/fuzzy/csoundex.c
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/third_party/fuzzy/soundex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.052806 opteryx-0.9.2/opteryx/third_party/levenshtein/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/third_party/levenshtein/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   223529 2023-02-28 12:34:17.000000 opteryx-0.9.2/opteryx/third_party/levenshtein/clevenshtein.c
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/third_party/levenshtein/levenshtein.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/third_party/mbleven.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.052806 opteryx-0.9.2/opteryx/third_party/pyarrow_ops/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/third_party/pyarrow_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   918624 2023-02-28 12:34:18.000000 opteryx-0.9.2/opteryx/third_party/pyarrow_ops/cjoin.c
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/third_party/pyarrow_ops/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/third_party/pyarrow_ops/join.py
--rw-r--r--   0 runner    (1001) docker     (123)    10819 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/third_party/pyarrow_ops/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.052806 opteryx-0.9.2/opteryx/third_party/query_builder/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/third_party/query_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/third_party/query_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/third_party/query_builder/test_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.052806 opteryx-0.9.2/opteryx/third_party/sqloxide/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/third_party/sqloxide/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.052806 opteryx-0.9.2/opteryx/third_party/travers/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/third_party/travers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13850 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/third_party/travers/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.056806 opteryx-0.9.2/opteryx/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/utils/arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)     8778 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/utils/arrow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.056806 opteryx-0.9.2/opteryx/utils/bitarray/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/utils/bitarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/utils/bitarray/bitarray.py
--rw-r--r--   0 runner    (1001) docker     (123)   197743 2023-02-28 12:34:18.000000 opteryx-0.9.2/opteryx/utils/bitarray/cbitarray.c
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/utils/bloom_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7733 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/utils/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/utils/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/utils/file_decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/utils/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/utils/intervals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/utils/lru_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/utils/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/utils/resource_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-02-28 12:34:02.000000 opteryx-0.9.2/opteryx/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.036806 opteryx-0.9.2/opteryx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14897 2023-02-28 12:34:18.000000 opteryx-0.9.2/opteryx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-02-28 12:34:19.000000 opteryx-0.9.2/opteryx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 12:34:18.000000 opteryx-0.9.2/opteryx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-28 12:34:18.000000 opteryx-0.9.2/opteryx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 12:34:18.000000 opteryx-0.9.2/opteryx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-28 12:34:18.000000 opteryx-0.9.2/opteryx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-28 12:34:18.000000 opteryx-0.9.2/opteryx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-02-28 12:34:02.000000 opteryx-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 12:34:19.056806 opteryx-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-02-28 12:34:02.000000 opteryx-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 12:34:19.056806 opteryx-0.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-02-28 12:34:04.000000 opteryx-0.9.2/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.913301 opteryx-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-03-04 12:46:33.000000 opteryx-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14229 2023-03-04 12:46:48.913301 opteryx-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13959 2023-03-04 12:46:33.000000 opteryx-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.885301 opteryx-0.9.3/opteryx/
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/attribute_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.885301 opteryx-0.9.3/opteryx/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.885301 opteryx-0.9.3/opteryx/components/binder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/components/binder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/components/binder/binder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.885301 opteryx-0.9.3/opteryx/components/logical_planner/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/components/logical_planner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19967 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/components/logical_planner/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/components/logical_planner/custom_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/components/logical_planner/logical_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17770 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/components/logical_planner/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/components/query_planner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.885301 opteryx-0.9.3/opteryx/components/sql_rewriter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/components/sql_rewriter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/components/sql_rewriter/sql_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/components/sql_rewriter/temporal_extraction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.889301 opteryx-0.9.3/opteryx/components/tree_rewriter/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/components/tree_rewriter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.889301 opteryx-0.9.3/opteryx/components/tree_rewriter/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/components/tree_rewriter/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/components/tree_rewriter/rules/rule_apply_demorgans_law.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/components/tree_rewriter/rules/rule_constant_evaluations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/components/tree_rewriter/rules/rule_defragment_morsels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/components/tree_rewriter/rules/rule_eliminate_negations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/components/tree_rewriter/rules/rule_function_evaluations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/components/tree_rewriter/rules/rule_move_literal_join_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/components/tree_rewriter/rules/rule_predicate_pushdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/components/tree_rewriter/rules/rule_split_conjunctive_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/components/tree_rewriter/rules/rule_use_heap_sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.889301 opteryx-0.9.3/opteryx/components/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/components/v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.889301 opteryx-0.9.3/opteryx/components/v2/logical_planner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/components/v2/logical_planner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/components/v2/logical_planner/planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9731 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.889301 opteryx-0.9.3/opteryx/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/connectors/arrow_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/connectors/aws_s3_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.893301 opteryx-0.9.3/opteryx/connectors/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/connectors/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/connectors/base/base_blob_storage_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/connectors/base/base_document_storage_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.893301 opteryx-0.9.3/opteryx/connectors/capabilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/connectors/capabilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/connectors/capabilities/predicate_pushable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/connectors/disk_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/connectors/gcp_cloudstorage_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/connectors/gcp_firestore_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/connectors/hadro_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/connectors/mongodb_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/connectors/sql_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.893301 opteryx-0.9.3/opteryx/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)     9679 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/functions/binary_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/functions/date_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/functions/number_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/functions/other_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6869 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/functions/string_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/functions/unary_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/functions/v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.893301 opteryx-0.9.3/opteryx/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/managers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.893301 opteryx-0.9.3/opteryx/managers/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/managers/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/managers/cache/memcached.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/managers/cache/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.893301 opteryx-0.9.3/opteryx/managers/expression/
+-rw-r--r--   0 runner    (1001) docker     (123)    16220 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/managers/expression/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.893301 opteryx-0.9.3/opteryx/managers/kvstores/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/managers/kvstores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/managers/kvstores/base_kv_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/managers/kvstores/kv_firestore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.893301 opteryx-0.9.3/opteryx/managers/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/managers/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/managers/metadata/data_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.893301 opteryx-0.9.3/opteryx/managers/schemes/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/managers/schemes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/managers/schemes/base_partition_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/managers/schemes/default_partitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/managers/schemes/mabel_partitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.897301 opteryx-0.9.3/opteryx/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11280 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/models/columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/models/execution_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/models/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/models/query_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.901301 opteryx-0.9.3/opteryx/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15060 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/operators/aggregate_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/operators/base_plan_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15535 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/operators/blob_reader_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/operators/build_statistics_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/operators/collection_reader_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/operators/column_filter_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/operators/cross_join_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/operators/distinct_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/operators/explain_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/operators/file_reader_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/operators/function_dataset_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/operators/heap_sort_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/operators/inner_join_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/operators/internal_dataset_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/operators/limit_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/operators/morsel_defragment_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/operators/offset_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/operators/outer_join_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/operators/projection_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/operators/selection_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11768 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/operators/show_columns_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/operators/show_create_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/operators/show_functions_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/operators/show_stores_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/operators/show_value_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/operators/show_variables_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/operators/sort_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/operators/sql_reader_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.901301 opteryx-0.9.3/opteryx/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36761 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/samples/astronaut_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/samples/no_table_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13319 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/samples/planet_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10962 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/samples/satellite_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.901301 opteryx-0.9.3/opteryx/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/shared/buffer_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/shared/materialized_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/shared/query_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.901301 opteryx-0.9.3/opteryx/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.901301 opteryx-0.9.3/opteryx/third_party/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/third_party/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.905301 opteryx-0.9.3/opteryx/third_party/cityhash/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/third_party/cityhash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19319 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/third_party/cityhash/city.cc
+-rw-r--r--   0 runner    (1001) docker     (123)   237362 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/third_party/cityhash/cityhash.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/third_party/cityhash/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.905301 opteryx-0.9.3/opteryx/third_party/distogram/
+-rw-r--r--   0 runner    (1001) docker     (123)    15497 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/third_party/distogram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.905301 opteryx-0.9.3/opteryx/third_party/fastlogging/
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/third_party/fastlogging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/third_party/fastlogging/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21205 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/third_party/fastlogging/fastlogging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/third_party/fastlogging/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/third_party/fastlogging/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/third_party/fastlogging/pyorcy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/third_party/fastlogging/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.905301 opteryx-0.9.3/opteryx/third_party/fuzzy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/third_party/fuzzy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   218370 2023-03-04 12:46:47.000000 opteryx-0.9.3/opteryx/third_party/fuzzy/csoundex.c
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/third_party/fuzzy/soundex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.905301 opteryx-0.9.3/opteryx/third_party/levenshtein/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/third_party/levenshtein/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   223529 2023-03-04 12:46:47.000000 opteryx-0.9.3/opteryx/third_party/levenshtein/clevenshtein.c
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/third_party/levenshtein/levenshtein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/third_party/mbleven.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.909301 opteryx-0.9.3/opteryx/third_party/pyarrow_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/third_party/pyarrow_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   918624 2023-03-04 12:46:48.000000 opteryx-0.9.3/opteryx/third_party/pyarrow_ops/cjoin.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/third_party/pyarrow_ops/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/third_party/pyarrow_ops/join.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10819 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/third_party/pyarrow_ops/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.909301 opteryx-0.9.3/opteryx/third_party/query_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/third_party/query_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/third_party/query_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/third_party/query_builder/test_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.909301 opteryx-0.9.3/opteryx/third_party/sqloxide/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/third_party/sqloxide/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.909301 opteryx-0.9.3/opteryx/third_party/travers/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/third_party/travers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13850 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/third_party/travers/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.909301 opteryx-0.9.3/opteryx/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/utils/arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8778 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/utils/arrow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.909301 opteryx-0.9.3/opteryx/utils/bitarray/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/utils/bitarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/utils/bitarray/bitarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)   197743 2023-03-04 12:46:48.000000 opteryx-0.9.3/opteryx/utils/bitarray/cbitarray.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/utils/bloom_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7733 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/utils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/utils/file_decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/utils/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/utils/intervals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/utils/lru_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/utils/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/utils/resource_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-03-04 12:46:33.000000 opteryx-0.9.3/opteryx/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.885301 opteryx-0.9.3/opteryx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14229 2023-03-04 12:46:48.000000 opteryx-0.9.3/opteryx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-03-04 12:46:48.000000 opteryx-0.9.3/opteryx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-04 12:46:48.000000 opteryx-0.9.3/opteryx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-04 12:46:48.000000 opteryx-0.9.3/opteryx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-04 12:46:48.000000 opteryx-0.9.3/opteryx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-04 12:46:48.000000 opteryx-0.9.3/opteryx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-04 12:46:48.000000 opteryx-0.9.3/opteryx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-04 12:46:33.000000 opteryx-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-04 12:46:48.913301 opteryx-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-03-04 12:46:33.000000 opteryx-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 12:46:48.909301 opteryx-0.9.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-04 12:46:34.000000 opteryx-0.9.3/tests/test_version.py
```

### Comparing `opteryx-0.9.2/LICENSE` & `opteryx-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/PKG-INFO` & `opteryx-0.9.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opteryx
-Version: 0.9.2
+Version: 0.9.3
 Summary: Python SQL Query Engine
 Home-page: https://github.com/mabel-dev/opteryx/
 Author: @joocer
 Author-email: justin.joyce@joocer.com
 Maintainer: @joocer
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -13,14 +13,15 @@
 
 ![Opteryx](https://raw.githubusercontent.com/mabel-dev/opteryx/main/opteryx-word-small.png)
 ## Query your data, where it lives.
 </div>
 
 <h3 align="center">
 
+
 Opteryx is a SQL Engine designed for embedded and cloud-native environments, and with command-line skills.
 
 [Documentation](https://opteryx.dev/latest) |
 [Examples](#examples) |
 [Contributing](https://opteryx.dev/latest/contributing/contributing/)
 
 [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Easily%20query%20your%data%20with%20Opteryx&url=https://mabel-dev.github.io/opteryx/&hashtags=python,sql)
@@ -30,63 +31,55 @@
 [![Downloads](https://pepy.tech/badge/opteryx)](https://pepy.tech/project/opteryx)
 [![last_commit](https://img.shields.io/github/last-commit/mabel-dev/opteryx)](https://github.com/mabel-dev/opteryx/commits)
 [![codecov](https://codecov.io/gh/mabel-dev/opteryx/branch/main/graph/badge.svg?token=sIgKpzzd95)](https://codecov.io/gh/mabel-dev/opteryx)
 [![PyPI Latest Release](https://img.shields.io/badge/Python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue?logo=python)](https://pypi.org/project/opteryx/)
 
 </h3>
 
-## Use Cases
+## What is Opteryx?
+
+Opteryx is a Python library for data wrangling and analytics. It creates a common interface to interact with various data platforms, enabling users to transform and explore data anywhere.
 
 - Using SQL to query data files written by another process - such as logs.
 - As a command line tool - Run SQL directly on files - bring the power and flexibility of SQL to filter, transform and combine files, or as a command line viewer and converter for Parquet, ORC or Avro format files.
 - As an embeddable engine - a low-cost option to allow hundreds of analysts to each have part-time databases.
 - Adding SQL to existing familar tools like pandas and Polars, Executing SQL against and returning result sets as Polars and pandas DataFrames
 
-## Features
-
-### __Feature Rich__
+## Why Use Opteryx?
 
-Supports most of the base [SQL92 standard](https://opteryx.dev/latest/get-started/external-standards/sql92/) and multiple extensions from modern SQL platforms like [Snowflake](https://www.snowflake.com/en/) and [Trino](https://trino.io/).
+### __Familiar Interface__
 
-### __High Availability__
+Opteryx supports key parts of the Python ADODB and [SQL92 standard](https://opteryx.dev/latest/get-started/external-standards/sql92/) standards which many analysts and engineers will already know how to use.
 
-[Shared Nothing](https://en.wikipedia.org/wiki/Shared-nothing_architecture)/[Shared Disk](https://en.wikipedia.org/wiki/Shared-disk_architecture) design means each query can run in a separate container instance making it nearly impossible for a rogue query to affect any other users. _(compute and storage can be shared)_
+### __Consistent Syntax__
 
-If a cluster, region or datacentre is unavailable, if you have instances able to run in another location, Opteryx will keep responding to queries. _(inflight queries may not be recovered)_
+Opteryx creates a common SQL-layer over multiple data platforms, allowing backend systems to be upgraded, migrated or consolidated without changing any Opteryx code.
 
-### __Query In Place__
+### __Bring your own Data__
 
 ![Opteryx](https://github.com/mabel-dev/opteryx.dev/raw/main/assets/data-stores.png)
 
-Opteryx queries your data in the systems you store them in saving you from the cost and effort of maintaining duplicates your data into a common store for analytics.
-
-You can store your data in Parquet, ORC or Avro files on disk or Cloud Storage, in MongoDB or Firestore, and in Postgres and access all of these data in the same query.
+Opteryx supports multiple query engines, dataframe APIs and storage formats. You can mix-and-match sources in a single query, so one dataset can be in Parquet, and another MySQL, and Opteryx is able to JOIN across them.
 
-### __Bring your own Data__
-
-Opteryx is able to read and process data from multiple sources, including data on local or cloud storage in popular data formats (including Parquet, ORC, Avro and JSONL), data in a SQL database like MySQL or Postgres. You can mix-and-match source, so one dataset can be in Parquet, and another MySQL, and Opteryx is able to JOIN across them.
+Opteryx queries your data in the systems you store them in saving you from the cost and effort of maintaining duplicates your data into a common store for analytics.
 
-Opteryx also allows you to execute SQL over pandas and Polars dataframes and return results of queries as arrow, pandas or Polars dataframes.
+Opteryx is able to push parts of your query to the source query engine, meaning queries run at the speed of the backend, not your local computer.
 
 ### __Consumption-Based Billing Friendly__
 
 Opteryx is well-suited for deployments to environments which are pay-as-you-use, like Google Cloud Run. Great for situations where you low-volume usage, or many environments, where the costs of many traditional database deployment can quickly add up.
 
 ### __Python Native__
 
 Opteryx is Open Source Python, it quickly and easily integrates into Python code, including Jupyter Notebooks, so you can start querying your data within a few minutes. You can even use Opteryx to run SQL against pandas DataFrames, and even execute a join with an in-memory DataFrame with a remote dataset.
 
 ### __Time Travel__
 
 Designed for data analytics in environments where decisions need to be replayable, Opteryx allows you to query data as at a point in time in the past to replay decision algorithms against facts as they were known in the past. _(data must be structured to enable temporal queries)_
 
-### __Schema Evolution__
-
-Opteryx supports some change to schemas and paritioning without requiring any existing data to be updated. _(data types can only be changed to compatitble types)_
-
 ### __Fast__
 
 Benchmarks on M1 Pro Mac running an ad hoc `GROUP BY` over 1Gb of data via the CLI in 1/5th of a second. _(different systems will have different performance characteristics)_
 
 Rows    | Columns | File Size | Query Time
 ------- | ------- | --------- | ----------
 561225  | 81      | 1Gb       | 0.22sec
```

### Comparing `opteryx-0.9.2/README.md` & `opteryx-0.9.3/opteryx.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,27 @@
+Metadata-Version: 2.1
+Name: opteryx
+Version: 0.9.3
+Summary: Python SQL Query Engine
+Home-page: https://github.com/mabel-dev/opteryx/
+Author: @joocer
+Author-email: justin.joyce@joocer.com
+Maintainer: @joocer
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
 
 ![Opteryx](https://raw.githubusercontent.com/mabel-dev/opteryx/main/opteryx-word-small.png)
 ## Query your data, where it lives.
 </div>
 
 <h3 align="center">
 
+
 Opteryx is a SQL Engine designed for embedded and cloud-native environments, and with command-line skills.
 
 [Documentation](https://opteryx.dev/latest) |
 [Examples](#examples) |
 [Contributing](https://opteryx.dev/latest/contributing/contributing/)
 
 [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Easily%20query%20your%data%20with%20Opteryx&url=https://mabel-dev.github.io/opteryx/&hashtags=python,sql)
@@ -19,63 +31,55 @@
 [![Downloads](https://pepy.tech/badge/opteryx)](https://pepy.tech/project/opteryx)
 [![last_commit](https://img.shields.io/github/last-commit/mabel-dev/opteryx)](https://github.com/mabel-dev/opteryx/commits)
 [![codecov](https://codecov.io/gh/mabel-dev/opteryx/branch/main/graph/badge.svg?token=sIgKpzzd95)](https://codecov.io/gh/mabel-dev/opteryx)
 [![PyPI Latest Release](https://img.shields.io/badge/Python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue?logo=python)](https://pypi.org/project/opteryx/)
 
 </h3>
 
-## Use Cases
+## What is Opteryx?
+
+Opteryx is a Python library for data wrangling and analytics. It creates a common interface to interact with various data platforms, enabling users to transform and explore data anywhere.
 
 - Using SQL to query data files written by another process - such as logs.
 - As a command line tool - Run SQL directly on files - bring the power and flexibility of SQL to filter, transform and combine files, or as a command line viewer and converter for Parquet, ORC or Avro format files.
 - As an embeddable engine - a low-cost option to allow hundreds of analysts to each have part-time databases.
 - Adding SQL to existing familar tools like pandas and Polars, Executing SQL against and returning result sets as Polars and pandas DataFrames
 
-## Features
+## Why Use Opteryx?
 
-### __Feature Rich__
+### __Familiar Interface__
 
-Supports most of the base [SQL92 standard](https://opteryx.dev/latest/get-started/external-standards/sql92/) and multiple extensions from modern SQL platforms like [Snowflake](https://www.snowflake.com/en/) and [Trino](https://trino.io/).
+Opteryx supports key parts of the Python ADODB and [SQL92 standard](https://opteryx.dev/latest/get-started/external-standards/sql92/) standards which many analysts and engineers will already know how to use.
 
-### __High Availability__
+### __Consistent Syntax__
 
-[Shared Nothing](https://en.wikipedia.org/wiki/Shared-nothing_architecture)/[Shared Disk](https://en.wikipedia.org/wiki/Shared-disk_architecture) design means each query can run in a separate container instance making it nearly impossible for a rogue query to affect any other users. _(compute and storage can be shared)_
+Opteryx creates a common SQL-layer over multiple data platforms, allowing backend systems to be upgraded, migrated or consolidated without changing any Opteryx code.
 
-If a cluster, region or datacentre is unavailable, if you have instances able to run in another location, Opteryx will keep responding to queries. _(inflight queries may not be recovered)_
-
-### __Query In Place__
+### __Bring your own Data__
 
 ![Opteryx](https://github.com/mabel-dev/opteryx.dev/raw/main/assets/data-stores.png)
 
-Opteryx queries your data in the systems you store them in saving you from the cost and effort of maintaining duplicates your data into a common store for analytics.
-
-You can store your data in Parquet, ORC or Avro files on disk or Cloud Storage, in MongoDB or Firestore, and in Postgres and access all of these data in the same query.
-
-### __Bring your own Data__
+Opteryx supports multiple query engines, dataframe APIs and storage formats. You can mix-and-match sources in a single query, so one dataset can be in Parquet, and another MySQL, and Opteryx is able to JOIN across them.
 
-Opteryx is able to read and process data from multiple sources, including data on local or cloud storage in popular data formats (including Parquet, ORC, Avro and JSONL), data in a SQL database like MySQL or Postgres. You can mix-and-match source, so one dataset can be in Parquet, and another MySQL, and Opteryx is able to JOIN across them.
+Opteryx queries your data in the systems you store them in saving you from the cost and effort of maintaining duplicates your data into a common store for analytics.
 
-Opteryx also allows you to execute SQL over pandas and Polars dataframes and return results of queries as arrow, pandas or Polars dataframes.
+Opteryx is able to push parts of your query to the source query engine, meaning queries run at the speed of the backend, not your local computer.
 
 ### __Consumption-Based Billing Friendly__
 
 Opteryx is well-suited for deployments to environments which are pay-as-you-use, like Google Cloud Run. Great for situations where you low-volume usage, or many environments, where the costs of many traditional database deployment can quickly add up.
 
 ### __Python Native__
 
 Opteryx is Open Source Python, it quickly and easily integrates into Python code, including Jupyter Notebooks, so you can start querying your data within a few minutes. You can even use Opteryx to run SQL against pandas DataFrames, and even execute a join with an in-memory DataFrame with a remote dataset.
 
 ### __Time Travel__
 
 Designed for data analytics in environments where decisions need to be replayable, Opteryx allows you to query data as at a point in time in the past to replay decision algorithms against facts as they were known in the past. _(data must be structured to enable temporal queries)_
 
-### __Schema Evolution__
-
-Opteryx supports some change to schemas and paritioning without requiring any existing data to be updated. _(data types can only be changed to compatitble types)_
-
 ### __Fast__
 
 Benchmarks on M1 Pro Mac running an ad hoc `GROUP BY` over 1Gb of data via the CLI in 1/5th of a second. _(different systems will have different performance characteristics)_
 
 Rows    | Columns | File Size | Query Time
 ------- | ------- | --------- | ----------
 561225  | 81      | 1Gb       | 0.22sec
```

### Comparing `opteryx-0.9.2/opteryx/__init__.py` & `opteryx-0.9.3/opteryx/__init__.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/__main__.py` & `opteryx-0.9.3/opteryx/__main__.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/attribute_types.py` & `opteryx-0.9.3/opteryx/attribute_types.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/components/binder/binder.py` & `opteryx-0.9.3/opteryx/components/binder/binder.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/components/logical_planner/__init__.py` & `opteryx-0.9.3/opteryx/components/logical_planner/__init__.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/components/logical_planner/builders.py` & `opteryx-0.9.3/opteryx/components/logical_planner/builders.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/components/logical_planner/custom_builders.py` & `opteryx-0.9.3/opteryx/components/logical_planner/custom_builders.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/components/logical_planner/logical_planner.py` & `opteryx-0.9.3/opteryx/components/logical_planner/logical_planner.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/components/logical_planner/queries.py` & `opteryx-0.9.3/opteryx/components/logical_planner/queries.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/components/query_planner.py` & `opteryx-0.9.3/opteryx/components/query_planner.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/components/sql_rewriter/sql_rewriter.py` & `opteryx-0.9.3/opteryx/components/sql_rewriter/sql_rewriter.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/components/sql_rewriter/temporal_extraction.py` & `opteryx-0.9.3/opteryx/components/sql_rewriter/temporal_extraction.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/components/tree_rewriter/__init__.py` & `opteryx-0.9.3/opteryx/components/tree_rewriter/__init__.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/components/tree_rewriter/rules/__init__.py` & `opteryx-0.9.3/opteryx/components/tree_rewriter/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/components/tree_rewriter/rules/rule_apply_demorgans_law.py` & `opteryx-0.9.3/opteryx/components/tree_rewriter/rules/rule_apply_demorgans_law.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/components/tree_rewriter/rules/rule_constant_evaluations.py` & `opteryx-0.9.3/opteryx/components/tree_rewriter/rules/rule_constant_evaluations.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/components/tree_rewriter/rules/rule_defragment_morsels.py` & `opteryx-0.9.3/opteryx/components/tree_rewriter/rules/rule_defragment_morsels.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/components/tree_rewriter/rules/rule_eliminate_negations.py` & `opteryx-0.9.3/opteryx/components/tree_rewriter/rules/rule_eliminate_negations.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/components/tree_rewriter/rules/rule_function_evaluations.py` & `opteryx-0.9.3/opteryx/components/tree_rewriter/rules/rule_function_evaluations.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/components/tree_rewriter/rules/rule_move_literal_join_filters.py` & `opteryx-0.9.3/opteryx/components/tree_rewriter/rules/rule_move_literal_join_filters.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/components/tree_rewriter/rules/rule_predicate_pushdown.py` & `opteryx-0.9.3/opteryx/components/tree_rewriter/rules/rule_predicate_pushdown.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/components/tree_rewriter/rules/rule_split_conjunctive_predicates.py` & `opteryx-0.9.3/opteryx/components/tree_rewriter/rules/rule_split_conjunctive_predicates.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/components/tree_rewriter/rules/rule_use_heap_sort.py` & `opteryx-0.9.3/opteryx/components/tree_rewriter/rules/rule_use_heap_sort.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/components/v2/logical_planner/planner.py` & `opteryx-0.9.3/opteryx/components/v2/logical_planner/planner.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/config.py` & `opteryx-0.9.3/opteryx/config.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/connection.py` & `opteryx-0.9.3/opteryx/connection.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/connectors/__init__.py` & `opteryx-0.9.3/opteryx/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/connectors/arrow_connector.py` & `opteryx-0.9.3/opteryx/connectors/arrow_connector.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/connectors/aws_s3_connector.py` & `opteryx-0.9.3/opteryx/connectors/aws_s3_connector.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/connectors/base/base_blob_storage_adapter.py` & `opteryx-0.9.3/opteryx/connectors/base/base_blob_storage_adapter.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/connectors/base/base_document_storage_adapter.py` & `opteryx-0.9.3/opteryx/connectors/base/base_document_storage_adapter.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/connectors/capabilities/__init__.py` & `opteryx-0.9.3/opteryx/connectors/capabilities/__init__.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/connectors/capabilities/predicate_pushable.py` & `opteryx-0.9.3/opteryx/connectors/capabilities/predicate_pushable.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/connectors/disk_connector.py` & `opteryx-0.9.3/opteryx/connectors/disk_connector.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/connectors/gcp_cloudstorage_connector.py` & `opteryx-0.9.3/opteryx/connectors/gcp_cloudstorage_connector.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/connectors/gcp_firestore_connector.py` & `opteryx-0.9.3/opteryx/connectors/gcp_firestore_connector.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/connectors/hadro_connector.py` & `opteryx-0.9.3/opteryx/connectors/hadro_connector.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/connectors/mongodb_connector.py` & `opteryx-0.9.3/opteryx/connectors/mongodb_connector.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/connectors/sql_connector.py` & `opteryx-0.9.3/opteryx/connectors/sql_connector.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/exceptions.py` & `opteryx-0.9.3/opteryx/exceptions.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/functions/__init__.py` & `opteryx-0.9.3/opteryx/functions/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
 
 
 # fmt:off
 # Function definitions optionally include the type and the function.
 # The type is needed particularly when returning Python objects that
 # the first entry is NONE.
 FUNCTIONS = {
-    "VERSION": _repeat_no_parameters(get_version),
+    "VERSION": _repeat_no_parameters(get_version), # *
 
     # TYPE CONVERSION
     "TIMESTAMP": cast("TIMESTAMP"),
     "BOOLEAN": cast("BOOLEAN"),
     "NUMERIC": cast("NUMERIC"),
     "VARCHAR": cast("VARCHAR"),
     "STRING": cast("VARCHAR"),  # alias for VARCHAR
@@ -241,17 +241,17 @@
     "ABS": compute.abs,
     "ABSOLUTE": compute.abs,
     "SIGN": compute.sign,
     "SIGNUM": compute.sign,
     "SQRT": compute.sqrt,
     "TRUNC": compute.trunc,
     "TRUNCATE": compute.trunc,
-    "PI": _repeat_no_parameters(number_functions.pi),
-    "PHI": _repeat_no_parameters(number_functions.phi),
-    "E": _repeat_no_parameters(number_functions.e),
+    "PI": _repeat_no_parameters(number_functions.pi), # *
+    "PHI": _repeat_no_parameters(number_functions.phi), # *
+    "E": _repeat_no_parameters(number_functions.e), # *
     "INT": _iterate_single_parameter(int),
     "INTEGER": _iterate_single_parameter(int),
     "FLOAT": _iterate_single_parameter(float),
     "POWER": compute.power,
     "LN": compute.ln,
     "LOG10": compute.log10,
     "LOG2": compute.log2,
@@ -259,15 +259,15 @@
 
     # DATES & TIMES
     "DATE_TRUNC": _iterate_double_parameter_field_second(dates.date_trunc),
     "TIME_BUCKET": date_functions.date_floor,
     "DATEDIFF": date_functions.date_diff,
     "DATEPART": date_functions.date_part,
     "DATE_FORMAT": date_functions.date_format,
-    "CURRENT_TIME": _repeat_no_parameters(date_functions.get_now),
+    "CURRENT_TIME": _repeat_no_parameters(date_functions.get_now), # *
     "NOW": _repeat_no_parameters(date_functions.get_now),
     "CURRENT_DATE": _repeat_no_parameters(date_functions.get_today),
     "TODAY": _repeat_no_parameters(date_functions.get_today),
     "TIME": _repeat_no_parameters(date_functions.get_time),
     "YESTERDAY": _repeat_no_parameters(date_functions.get_yesterday),
     "DATE": _iterate_single_parameter(date_functions.get_date),
     "YEAR": compute.year,
```

### Comparing `opteryx-0.9.2/opteryx/functions/binary_operators.py` & `opteryx-0.9.3/opteryx/functions/binary_operators.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/functions/date_functions.py` & `opteryx-0.9.3/opteryx/functions/date_functions.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/functions/number_functions.py` & `opteryx-0.9.3/opteryx/functions/number_functions.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/functions/other_functions.py` & `opteryx-0.9.3/opteryx/functions/other_functions.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/functions/string_functions.py` & `opteryx-0.9.3/opteryx/functions/string_functions.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/functions/unary_operations.py` & `opteryx-0.9.3/opteryx/functions/unary_operations.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/functions/v2.py` & `opteryx-0.9.3/opteryx/functions/v2.py`

 * *Files 11% similar despite different names*

```diff
@@ -86,14 +86,44 @@
     style = _FunctionStyle.CONSTANT
     cost = 1
 
     def _func(self) -> datetime.time:
         return datetime.datetime.utcnow().time()
 
 
+class E(_BaseFunction):
+    """Return Euler's number."""
+
+    style = _FunctionStyle.CONSTANT
+    cost = 1
+
+    def _func(self) -> float:
+        return 2.71828182845904523536028747135266249775724709369995
+
+
+class Phi(_BaseFunction):
+    """Return the golden ratio."""
+
+    style = _FunctionStyle.CONSTANT
+    cost = 1
+
+    def _func(self) -> float:
+        return 1.61803398874989484820458683436563811772030917980576
+
+
+class Pi(_BaseFunction):
+    """Return Pi."""
+
+    style = _FunctionStyle.CONSTANT
+    cost = 1
+
+    def _func(self) -> float:
+        return 3.14159265358979323846264338327950288419716939937510
+
+
 class Version(_BaseFunction):
     """Return the version of the query engine."""
 
     style = _FunctionStyle.CONSTANT
     cost = 1
 
     def _func(self) -> str:
@@ -101,11 +131,11 @@
 
         return opteryx.__version__
 
 
 FUNCTIONS = get_functions()
 
 if __name__ == "__main__":  # pragma: no cover
-    func = FUNCTIONS["CURRENT_TIME"]()
+    func = FUNCTIONS["E"]()
     print(func)
     print(func())
     print(func.style)
```

### Comparing `opteryx-0.9.2/opteryx/managers/__init__.py` & `opteryx-0.9.3/opteryx/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/managers/cache/memcached.py` & `opteryx-0.9.3/opteryx/managers/cache/memcached.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/managers/cache/memory.py` & `opteryx-0.9.3/opteryx/managers/cache/memory.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/managers/expression/__init__.py` & `opteryx-0.9.3/opteryx/managers/expression/__init__.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/managers/kvstores/__init__.py` & `opteryx-0.9.3/opteryx/managers/kvstores/__init__.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/managers/kvstores/base_kv_store.py` & `opteryx-0.9.3/opteryx/managers/kvstores/base_kv_store.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/managers/kvstores/kv_firestore.py` & `opteryx-0.9.3/opteryx/managers/kvstores/kv_firestore.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/managers/metadata/data_catalog.py` & `opteryx-0.9.3/opteryx/managers/metadata/data_catalog.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/managers/schemes/__init__.py` & `opteryx-0.9.3/opteryx/managers/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/managers/schemes/base_partition_scheme.py` & `opteryx-0.9.3/opteryx/managers/schemes/base_partition_scheme.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/managers/schemes/default_partitions.py` & `opteryx-0.9.3/opteryx/managers/schemes/default_partitions.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/managers/schemes/mabel_partitions.py` & `opteryx-0.9.3/opteryx/managers/schemes/mabel_partitions.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/models/__init__.py` & `opteryx-0.9.3/opteryx/models/__init__.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/models/columns.py` & `opteryx-0.9.3/opteryx/models/columns.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/models/execution_tree.py` & `opteryx-0.9.3/opteryx/models/execution_tree.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/models/node.py` & `opteryx-0.9.3/opteryx/models/node.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/models/query_properties.py` & `opteryx-0.9.3/opteryx/models/query_properties.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/operators/__init__.py` & `opteryx-0.9.3/opteryx/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/operators/aggregate_node.py` & `opteryx-0.9.3/opteryx/operators/aggregate_node.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/operators/base_plan_node.py` & `opteryx-0.9.3/opteryx/operators/base_plan_node.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,17 +20,16 @@
 class BasePlanNode(abc.ABC):
     _producers = None
 
     def __init__(self, properties: QueryProperties, **config):
         """
         This is the base class for nodes in the execution plan.
 
-        The initializer accepts a QueryStatistics node which is populated by
-        different nodes differently to record what happened during the query
-        execution.
+        The initializer accepts a QueryStatistics node which is populated by different nodes
+        differently to record what happened during the query execution.
         """
         self.properties = properties
         self.statistics = QueryStatistics(properties.qid)
 
     def set_producers(self, producers):
         self._producers = producers
```

### Comparing `opteryx-0.9.2/opteryx/operators/blob_reader_node.py` & `opteryx-0.9.3/opteryx/operators/blob_reader_node.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/operators/build_statistics_node.py` & `opteryx-0.9.3/opteryx/operators/build_statistics_node.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/operators/collection_reader_node.py` & `opteryx-0.9.3/opteryx/operators/collection_reader_node.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/operators/column_filter_node.py` & `opteryx-0.9.3/opteryx/operators/column_filter_node.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/operators/cross_join_node.py` & `opteryx-0.9.3/opteryx/operators/cross_join_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # limitations under the License.
 
 """
 Cross Join Node
 
 This is a SQL Query Execution Plan Node.
 
-This performs a CROSS JOIN - CROSS JOIN is not natively supported by
-PyArrow so this is written out rather than calling the join() functions
+This performs a CROSS JOIN - CROSS JOIN is not natively supported by PyArrow so this is written
+here rather than calling the join() functions
 """
 from typing import Iterable
 
 import numpy
 import pyarrow
 
 from opteryx.exceptions import SqlError
```

### Comparing `opteryx-0.9.2/opteryx/operators/distinct_node.py` & `opteryx-0.9.3/opteryx/operators/distinct_node.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/operators/explain_node.py` & `opteryx-0.9.3/opteryx/operators/explain_node.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/operators/file_reader_node.py` & `opteryx-0.9.3/opteryx/operators/file_reader_node.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/operators/function_dataset_node.py` & `opteryx-0.9.3/opteryx/operators/function_dataset_node.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/operators/heap_sort_node.py` & `opteryx-0.9.3/opteryx/operators/heap_sort_node.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/operators/inner_join_node.py` & `opteryx-0.9.3/opteryx/operators/inner_join_node.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/operators/internal_dataset_node.py` & `opteryx-0.9.3/opteryx/operators/internal_dataset_node.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/operators/limit_node.py` & `opteryx-0.9.3/opteryx/operators/limit_node.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/operators/morsel_defragment_node.py` & `opteryx-0.9.3/opteryx/operators/morsel_defragment_node.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,41 +11,42 @@
 # limitations under the License.
 
 """
 Morsel Defragment Node
 
 This is a SQL Query Execution Plan Node.
 
-    Orignally implemented to test if datasets have any records as they pass through
-    the DAG, this function normalizes the number of bytes per morsel.
+    Orignally implemented to test if datasets have any records as they pass through the DAG, this
+    function normalizes the number of bytes per morsel.
 
     This is to balance two competing demands:
-        - operate in a low memory environment, if the morsels are too large they may
-          cause the process to fail.
-        - operate quickly, if we spend our time doing SIMD on morsel with few records
-          we're not working as fast as we can.
-
-    The low-water mark is 75% of the target size, less than this we look to merge
-    morsels together. This is more common following the implementation of projection
-    push down, one column doesn't take up a lot of memory so we consolidate tens of
-    morsels into a single morsel.
-
-    The high-water mark is 199% of the target size, more than this we split the morsel.
-    Splitting at a size any less than this will end up with morsels less that the
-    target morsel size.
+        - operate in a low memory environment, if the morsels are too large they may cause the
+          process to fail.
+        - operate quickly, if we spend our time doing Vecorization/SIMD on morsel with few records
+           we're not working as fast as we can.
+
+    The low-water mark is 75% of the target size, less than this we look to merge morsels together.
+    This is more common following the implementation of projection push down, one column doesn't
+    take up a lot of memory so we consolidate tens of morsels into a single morsel.
 
+    The high-water mark is 199% of the target size, more than this we split the morsel. Splitting
+    at a size any less than this will end up with morsels less that the target morsel size.
+
+    We also have a record count limit, this is because of quirks with PyArrow, it changes long
+    arrays into ChunkedArrays which behave differently to Arrays in some circumstances.
 """
 import time
 from typing import Iterable
 
 import pyarrow
 
 from opteryx.operators import BasePlanNode
 
-MORSEL_SIZE = 64 * 1024 * 1024  # 64Mb
+MORSEL_SIZE_BYTES: int = 64 * 1024 * 1024  # 64Mb
+MORSEL_SIZE_COUNT: int = 500000  # hard record count limit, half a million
 HIGH_WATER: float = 1.99  # Split morsels over 199% of MORSEL_SIZE
 LOW_WATER: float = 0.75  # Merge morsels under 75% of MORSEL_SIZE
 
 
 class MorselDefragmentNode(BasePlanNode):
     @property
     def name(self):  # pragma: no cover
@@ -78,40 +79,44 @@
                 self.statistics.time_defragmenting += time.monotonic_ns() - start
 
                 # work out some stats about what we have
                 morsel_bytes = morsel.nbytes
                 morsel_records = morsel.num_rows
 
                 # if we're more than double the target size, let's do something
-                if morsel_bytes > (MORSEL_SIZE * HIGH_WATER):  # pragma: no cover
+                if (
+                    morsel_bytes > (MORSEL_SIZE_BYTES * HIGH_WATER)
+                    or morsel_records > MORSEL_SIZE_COUNT
+                ):  # pragma: no cover
                     start = time.monotonic_ns()
 
                     average_record_size = morsel_bytes / morsel_records
-                    new_row_count = int(MORSEL_SIZE / average_record_size)
+                    new_row_count = min(
+                        int(MORSEL_SIZE_BYTES / average_record_size), MORSEL_SIZE_COUNT
+                    )
                     row_counter += new_row_count
                     self.statistics.chunk_splits += 1
                     new_morsel = morsel.slice(offset=0, length=new_row_count)
                     at_least_one_morsel = True
                     collected_rows = morsel.slice(offset=new_row_count)
 
                     self.statistics.time_defragmenting += time.monotonic_ns() - start
 
                     yield new_morsel
-                # if we're less than 75% of the morsel size, save hold what we have so
-                # far and go collect the next morsel
-                elif morsel_bytes < (MORSEL_SIZE * LOW_WATER):
+                # if we're less than 75% of the morsel size, save hold what we have so far and go
+                # collect the next morsel
+                elif morsel_bytes < (MORSEL_SIZE_BYTES * LOW_WATER):
                     collected_rows = morsel
                 # otherwise the morsel size is okay so we can emit the current morsel
                 else:
                     row_counter += morsel_records
                     yield morsel
                     at_least_one_morsel = True
             elif not at_least_one_morsel:
-                # we have to emit something to the next step, but don't emit
-                # multiple empty morsels
+                # we have to emit something to the next step, but don't emit multiple empty morsels
                 yield morsel
                 at_least_one_morsel = True
 
         # if we're at the end and haven't emitted all the records, emit them now
         if collected_rows:
             row_counter += collected_rows.num_rows
             yield collected_rows
```

### Comparing `opteryx-0.9.2/opteryx/operators/offset_node.py` & `opteryx-0.9.3/opteryx/operators/offset_node.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/operators/outer_join_node.py` & `opteryx-0.9.3/opteryx/operators/outer_join_node.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/operators/projection_node.py` & `opteryx-0.9.3/opteryx/operators/projection_node.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/operators/selection_node.py` & `opteryx-0.9.3/opteryx/operators/selection_node.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/operators/show_columns_node.py` & `opteryx-0.9.3/opteryx/operators/show_columns_node.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/operators/show_create_node.py` & `opteryx-0.9.3/opteryx/operators/show_create_node.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/operators/show_functions_node.py` & `opteryx-0.9.3/opteryx/operators/show_functions_node.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/operators/show_stores_node.py` & `opteryx-0.9.3/opteryx/operators/show_stores_node.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/operators/show_value_node.py` & `opteryx-0.9.3/opteryx/operators/show_value_node.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/operators/show_variables_node.py` & `opteryx-0.9.3/opteryx/operators/show_variables_node.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/operators/sort_node.py` & `opteryx-0.9.3/opteryx/operators/sort_node.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/operators/sql_reader_node.py` & `opteryx-0.9.3/opteryx/operators/sql_reader_node.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/samples/__init__.py` & `opteryx-0.9.3/opteryx/samples/__init__.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/samples/astronaut_data.py` & `opteryx-0.9.3/opteryx/samples/astronaut_data.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/samples/no_table_data.py` & `opteryx-0.9.3/opteryx/samples/no_table_data.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/samples/planet_data.py` & `opteryx-0.9.3/opteryx/samples/planet_data.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/samples/satellite_data.py` & `opteryx-0.9.3/opteryx/samples/satellite_data.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/shared/__init__.py` & `opteryx-0.9.3/opteryx/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/shared/buffer_pool.py` & `opteryx-0.9.3/opteryx/shared/buffer_pool.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/shared/materialized_datasets.py` & `opteryx-0.9.3/opteryx/shared/materialized_datasets.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/shared/query_statistics.py` & `opteryx-0.9.3/opteryx/shared/query_statistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,17 +14,16 @@
 
 
 @dataclass
 class _QueryStatistics:
     """
     Data object to collect information during query execution.
 
-    Implemented as a singleton rather than having to pass the Statistics modeal around
-    the plan and execution, you only need the query id (qid) and the stats model can be
-    returned.
+    Implemented as a singleton rather than having to pass the Statistics modeal around the plan
+    and execution, you only need the query id (qid) and the stats model can be returned.
     """
 
     def __init__(self):
         self._messages = []
 
         self.count_blobs_found: int = 0
         self.count_data_blobs_read: int = 0
```

### Comparing `opteryx-0.9.2/opteryx/third_party/cityhash/city.cc` & `opteryx-0.9.3/opteryx/third_party/cityhash/city.cc`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/third_party/cityhash/cityhash.cpp` & `opteryx-0.9.3/opteryx/third_party/cityhash/cityhash.cpp`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/third_party/cityhash/setup.py` & `opteryx-0.9.3/opteryx/third_party/cityhash/setup.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/third_party/distogram/__init__.py` & `opteryx-0.9.3/opteryx/third_party/distogram/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,33 +88,35 @@
         # and add this to the distogram.
         # Histogram gives us n+1 values, so we average consecutive values.
         # This ends up being an approximation of an approximation but 1000x faster.
         # The accuracy of this approach is poor on datasets with very low record counts,
         # but even if a bad decision is made on a table with 500 rows, the consequence
         # is minimal, if a bad decision is made on a table with 5m rows, it starts to
         # matter.
+        if len(values) == 0:
+            return
         bin_values, counts = numpy.unique(values, return_counts=True)
         if len(bin_values) > (self._bin_count * 5):
             counts, bin_values = numpy.histogram(values, self._bin_count * 5, density=False)
             bin_values = [bin_values[i] + bin_values[i + 1] / 2 for i in range(len(bin_values) - 1)]
         for index, count in enumerate(counts):
             if count > 0:
                 update(
                     self,
                     value=bin_values[index],
                     count=count,
                 )
 
         # we need to overwrite any range values as we've approximated the dataset
         if self.min is None:
-            self.min = min(values)
-            self.max = max(values)
+            self.min = values.min()
+            self.max = values.max()
         else:
-            self.min = min(self.min, min(values))
-            self.max = max(self.max, max(values))
+            self.min = min(self.min, values.min())
+            self.max = max(self.max, values.max())
 
     def count(self):
         return sum(f for _, f in self.bins)
 
     @property
     def max_bin_count(self):
         return self._bin_count
```

### Comparing `opteryx-0.9.2/opteryx/third_party/fastlogging/__init__.py` & `opteryx-0.9.3/opteryx/third_party/fastlogging/__init__.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/third_party/fastlogging/console.py` & `opteryx-0.9.3/opteryx/third_party/fastlogging/console.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/third_party/fastlogging/fastlogging.py` & `opteryx-0.9.3/opteryx/third_party/fastlogging/fastlogging.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/third_party/fastlogging/network.py` & `opteryx-0.9.3/opteryx/third_party/fastlogging/network.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/third_party/fastlogging/optimize.py` & `opteryx-0.9.3/opteryx/third_party/fastlogging/optimize.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/third_party/fastlogging/pyorcy.py` & `opteryx-0.9.3/opteryx/third_party/fastlogging/pyorcy.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/third_party/fastlogging/setup.py` & `opteryx-0.9.3/opteryx/third_party/fastlogging/setup.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/third_party/fuzzy/csoundex.c` & `opteryx-0.9.3/opteryx/third_party/fuzzy/csoundex.c`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/third_party/levenshtein/clevenshtein.c` & `opteryx-0.9.3/opteryx/third_party/levenshtein/clevenshtein.c`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/third_party/mbleven.py` & `opteryx-0.9.3/opteryx/third_party/mbleven.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/third_party/pyarrow_ops/cjoin.c` & `opteryx-0.9.3/opteryx/third_party/pyarrow_ops/cjoin.c`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/third_party/pyarrow_ops/helpers.py` & `opteryx-0.9.3/opteryx/third_party/pyarrow_ops/helpers.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/third_party/pyarrow_ops/join.py` & `opteryx-0.9.3/opteryx/third_party/pyarrow_ops/join.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/third_party/pyarrow_ops/ops.py` & `opteryx-0.9.3/opteryx/third_party/pyarrow_ops/ops.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/third_party/query_builder/builder.py` & `opteryx-0.9.3/opteryx/third_party/query_builder/builder.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/third_party/query_builder/test_builder.py` & `opteryx-0.9.3/opteryx/third_party/query_builder/test_builder.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/third_party/travers/graph.py` & `opteryx-0.9.3/opteryx/third_party/travers/graph.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/utils/__init__.py` & `opteryx-0.9.3/opteryx/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,14 @@
     This is roughly twice as fast as the previous implementation which was roughly
     twice as fast as it's previous implementation.
 
     This has more room for improvement, particularly in the Base64 encoding part,
     but this currently isn't identified as a performance bottleneck, the last
     rewrite was incidental when writing tests for a hasher.
     """
-    import random
     import struct
     from base64 import b64encode
 
     words: int = int(-(width * 0.75) // -8) + 1
 
     bytestring = struct.pack("=" + "Q" * words, *[random.getrandbits(64)] * words)
     return b64encode(bytestring).decode()[:width]
```

### Comparing `opteryx-0.9.2/opteryx/utils/arrays.py` & `opteryx-0.9.3/opteryx/utils/arrays.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/utils/arrow.py` & `opteryx-0.9.3/opteryx/utils/arrow.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/utils/bitarray/cbitarray.c` & `opteryx-0.9.3/opteryx/utils/bitarray/cbitarray.c`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/utils/bloom_filter.py` & `opteryx-0.9.3/opteryx/utils/bloom_filter.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/utils/colors.py` & `opteryx-0.9.3/opteryx/utils/colors.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/utils/dates.py` & `opteryx-0.9.3/opteryx/utils/dates.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/utils/display.py` & `opteryx-0.9.3/opteryx/utils/display.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/utils/file_decoders.py` & `opteryx-0.9.3/opteryx/utils/file_decoders.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/utils/formatter.py` & `opteryx-0.9.3/opteryx/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/utils/intervals.py` & `opteryx-0.9.3/opteryx/utils/intervals.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/utils/paths.py` & `opteryx-0.9.3/opteryx/utils/paths.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/utils/resource_monitor.py` & `opteryx-0.9.3/opteryx/utils/resource_monitor.py`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/opteryx/version.py` & `opteryx-0.9.3/opteryx/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 """
 Store the version here so:
 1) we don't load dependencies by storing it in __init__.py
 2) we can import it in setup.py for the same reason
 """
 
 # __version__ = "0.4.0-alpha.6"
-__version__ = "0.9.2"
+__version__ = "0.9.3"
```

### Comparing `opteryx-0.9.2/opteryx.egg-info/PKG-INFO` & `opteryx-0.9.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,16 @@
-Metadata-Version: 2.1
-Name: opteryx
-Version: 0.9.2
-Summary: Python SQL Query Engine
-Home-page: https://github.com/mabel-dev/opteryx/
-Author: @joocer
-Author-email: justin.joyce@joocer.com
-Maintainer: @joocer
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
 
 ![Opteryx](https://raw.githubusercontent.com/mabel-dev/opteryx/main/opteryx-word-small.png)
 ## Query your data, where it lives.
 </div>
 
 <h3 align="center">
 
+
 Opteryx is a SQL Engine designed for embedded and cloud-native environments, and with command-line skills.
 
 [Documentation](https://opteryx.dev/latest) |
 [Examples](#examples) |
 [Contributing](https://opteryx.dev/latest/contributing/contributing/)
 
 [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Easily%20query%20your%data%20with%20Opteryx&url=https://mabel-dev.github.io/opteryx/&hashtags=python,sql)
@@ -30,63 +20,55 @@
 [![Downloads](https://pepy.tech/badge/opteryx)](https://pepy.tech/project/opteryx)
 [![last_commit](https://img.shields.io/github/last-commit/mabel-dev/opteryx)](https://github.com/mabel-dev/opteryx/commits)
 [![codecov](https://codecov.io/gh/mabel-dev/opteryx/branch/main/graph/badge.svg?token=sIgKpzzd95)](https://codecov.io/gh/mabel-dev/opteryx)
 [![PyPI Latest Release](https://img.shields.io/badge/Python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue?logo=python)](https://pypi.org/project/opteryx/)
 
 </h3>
 
-## Use Cases
+## What is Opteryx?
+
+Opteryx is a Python library for data wrangling and analytics. It creates a common interface to interact with various data platforms, enabling users to transform and explore data anywhere.
 
 - Using SQL to query data files written by another process - such as logs.
 - As a command line tool - Run SQL directly on files - bring the power and flexibility of SQL to filter, transform and combine files, or as a command line viewer and converter for Parquet, ORC or Avro format files.
 - As an embeddable engine - a low-cost option to allow hundreds of analysts to each have part-time databases.
 - Adding SQL to existing familar tools like pandas and Polars, Executing SQL against and returning result sets as Polars and pandas DataFrames
 
-## Features
+## Why Use Opteryx?
 
-### __Feature Rich__
+### __Familiar Interface__
 
-Supports most of the base [SQL92 standard](https://opteryx.dev/latest/get-started/external-standards/sql92/) and multiple extensions from modern SQL platforms like [Snowflake](https://www.snowflake.com/en/) and [Trino](https://trino.io/).
+Opteryx supports key parts of the Python ADODB and [SQL92 standard](https://opteryx.dev/latest/get-started/external-standards/sql92/) standards which many analysts and engineers will already know how to use.
 
-### __High Availability__
+### __Consistent Syntax__
 
-[Shared Nothing](https://en.wikipedia.org/wiki/Shared-nothing_architecture)/[Shared Disk](https://en.wikipedia.org/wiki/Shared-disk_architecture) design means each query can run in a separate container instance making it nearly impossible for a rogue query to affect any other users. _(compute and storage can be shared)_
+Opteryx creates a common SQL-layer over multiple data platforms, allowing backend systems to be upgraded, migrated or consolidated without changing any Opteryx code.
 
-If a cluster, region or datacentre is unavailable, if you have instances able to run in another location, Opteryx will keep responding to queries. _(inflight queries may not be recovered)_
-
-### __Query In Place__
+### __Bring your own Data__
 
 ![Opteryx](https://github.com/mabel-dev/opteryx.dev/raw/main/assets/data-stores.png)
 
-Opteryx queries your data in the systems you store them in saving you from the cost and effort of maintaining duplicates your data into a common store for analytics.
-
-You can store your data in Parquet, ORC or Avro files on disk or Cloud Storage, in MongoDB or Firestore, and in Postgres and access all of these data in the same query.
-
-### __Bring your own Data__
+Opteryx supports multiple query engines, dataframe APIs and storage formats. You can mix-and-match sources in a single query, so one dataset can be in Parquet, and another MySQL, and Opteryx is able to JOIN across them.
 
-Opteryx is able to read and process data from multiple sources, including data on local or cloud storage in popular data formats (including Parquet, ORC, Avro and JSONL), data in a SQL database like MySQL or Postgres. You can mix-and-match source, so one dataset can be in Parquet, and another MySQL, and Opteryx is able to JOIN across them.
+Opteryx queries your data in the systems you store them in saving you from the cost and effort of maintaining duplicates your data into a common store for analytics.
 
-Opteryx also allows you to execute SQL over pandas and Polars dataframes and return results of queries as arrow, pandas or Polars dataframes.
+Opteryx is able to push parts of your query to the source query engine, meaning queries run at the speed of the backend, not your local computer.
 
 ### __Consumption-Based Billing Friendly__
 
 Opteryx is well-suited for deployments to environments which are pay-as-you-use, like Google Cloud Run. Great for situations where you low-volume usage, or many environments, where the costs of many traditional database deployment can quickly add up.
 
 ### __Python Native__
 
 Opteryx is Open Source Python, it quickly and easily integrates into Python code, including Jupyter Notebooks, so you can start querying your data within a few minutes. You can even use Opteryx to run SQL against pandas DataFrames, and even execute a join with an in-memory DataFrame with a remote dataset.
 
 ### __Time Travel__
 
 Designed for data analytics in environments where decisions need to be replayable, Opteryx allows you to query data as at a point in time in the past to replay decision algorithms against facts as they were known in the past. _(data must be structured to enable temporal queries)_
 
-### __Schema Evolution__
-
-Opteryx supports some change to schemas and paritioning without requiring any existing data to be updated. _(data types can only be changed to compatitble types)_
-
 ### __Fast__
 
 Benchmarks on M1 Pro Mac running an ad hoc `GROUP BY` over 1Gb of data via the CLI in 1/5th of a second. _(different systems will have different performance characteristics)_
 
 Rows    | Columns | File Size | Query Time
 ------- | ------- | --------- | ----------
 561225  | 81      | 1Gb       | 0.22sec
```

### Comparing `opteryx-0.9.2/opteryx.egg-info/SOURCES.txt` & `opteryx-0.9.3/opteryx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opteryx-0.9.2/setup.py` & `opteryx-0.9.3/setup.py`

 * *Files identical despite different names*

